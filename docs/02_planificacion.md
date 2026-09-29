# 2. Planificación del proyecto

## 2.1. Metodología de trabajo
Para la ejecución de este proyecto se adopta una metodología de trabajo **Ágil basada en iteraciones**, estructurada en fases secuenciales de análisis, diseño, implementación y validación. Este enfoque permite adaptar los requisitos a medida que se despliegan las infraestructuras y corregir desviaciones mediante pruebas continuas.

Las reuniones de seguimiento y el control de versiones se gestionan a través de **GitHub**, utilizando *commits* descriptivos y un flujo de integración continua (*CI/CD*) para la actualización del portal de documentación.

## 2.2. Recursos necesarios

### Recursos Hardware
- **Servidor de Virtualización:** Equipo anfitrión con procesamiento multihilo y capacidad de memoria RAM suficiente para alojar el entorno de laboratorio.
- **Electrónica de Red:** Dispositivos de conmutación y enrutamiento (Cisco / MikroTik) para la segmentación física y lógica de las VLANs.
- **Puestos de cliente:** Equipos de trabajo para pruebas de acceso, administración remota y desarrollo web.

### Recursos Software
- **Hypervisor:** VMware Workstation / Proxmox VE para la orquestación de máquinas virtuales.
- **Sistemas Operativos:** Windows Server (Active Directory / DNS / DHCP) y Ubuntu Server (Servicios web y monitorización).
- **Herramientas de desarrollo y documentación:** Visual Studio Code, Git, GitHub Actions y MkDocs.

### Recursos Humanos
- **Administrador de Sistemas e Infraestructuras (Estudiante de ASIR):** Responsable de la planificación, despliegue, configuración de red, seguridad y documentación técnica del proyecto.

## 2.3. Cronograma (Diagrama de Gantt)

A continuación se detalla la estimación temporal de las fases del proyecto distribuida a lo largo del curso académico:

| Fase / Actividad | Duración estimada | Semanas |
|---|---|---|
| **Fase 1: Análisis y Caracterización del Reto** | 2 semanas | Semanas 1 - 2 |
| **Fase 2: Diseño de Red y Topología** | 3 semanas | Semanas 3 - 5 |
| **Fase 3: Despliegue de Servidores Base y Dominio** | 4 semanas | Semanas 6 - 9 |
| **Fase 4: Servicios Avanzados, Monitorización y Seguridad** | 4 semanas | Semanas 10 - 13 |
| **Fase 5: Pruebas de Integración y Documentación Final** | 3 semanas | Semanas 14 - 16 |
