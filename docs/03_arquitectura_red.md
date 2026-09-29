# 3. Arquitectura de Red y Requisitos Técnicos

## 3.1. Requisitos Técnicos de la Infraestructura
Para responder a las necesidades operativas de **GamerCore Studios S.L.**, la infraestructura de red debe garantizar alta disponibilidad, seguridad perimetral, aislamiento de tráficos y escalabilidad. 

Los requisitos fundamentales son:
- **Segmentación lógica (VLANs):** Aislamiento del tráfico de producción, administración, servidores y zona desmilitarizada (DMZ).
- **Gestión centralizada de identidades:** Dominio Active Directory para el control de accesos y directivas de grupo (GPOs).
- **Resolución de nombres y direccionamiento dinámico:** Servicios DNS y DHCP jerarquizados.
- **Seguridad perimetral:** Firewall/Router para filtrado de tráfico inter-VLAN y control de acceso a Internet.

## 3.2. Plan de Direccionamiento IP y Segmentación (VLANs)

Se adopta el direccionamiento privado de clase C / B bajo la red base `192.168.0.0/16`, dividida en subredes `/24` según el rol operativo:

| Nombre de VLAN | ID VLAN | Red / Máscara | Rango útil IP | Pasarela (Gateway) | Descripción / Propósito |
|---|---|---|---|---|---|
| **VLAN_MGT** | `VLAN 10` | `192.168.10.0/24` | `192.168.10.2 - 192.168.10.254` | `192.168.10.1` | Gestión de hipervisores, switches y PDU. |
| **VLAN_SRV** | `VLAN 20` | `192.168.20.0/24` | `192.168.20.2 - 192.168.20.254` | `192.168.20.1` | Servidores de infraestructura (AD DC, DNS, DHCP). |
| **VLAN_CLI** | `VLAN 30` | `192.168.30.0/24` | `192.168.30.50 - 192.168.30.200` | `192.168.30.1` | Puestos de trabajo de los desarrolladores y empleados. |
| **VLAN_DMZ** | `VLAN 40` | `192.168.40.0/24` | `192.168.40.2 - 192.168.40.254` | `192.168.40.1` | Servidores públicos (Web, repositorio de juegos, servicios externos). |

## 3.3. Asignación de Servidores y Servicios

| Nombre del Equipo | Función / Rol principal | Sistema Operativo | Dirección IP | VLAN Asociada |
|---|---|---|---|---|
| **`GW-ROUTER`** | Firewall / Router (pNode) | pfSense / RouterOS | `192.168.X.1` | Trunk (Todas) |
| **`DC01-GAMER`** | Controlador de Dominio, DNS y DHCP | Windows Server 2022 | `192.168.20.10` | VLAN 20 (SRV) |
| **`SRV-WEB01`** | Servidor Web de la Compañía (MkDocs / Nginx) | Ubuntu Server 22.04 LTS | `192.168.40.10` | VLAN 40 (DMZ) |
| **`SRV-MON01`** | Servidor de Monitorización (Zabbix / Grafana) | Ubuntu Server 22.04 LTS | `192.168.10.15` | VLAN 10 (MGT) |
