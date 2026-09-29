# 1. Introducción

## 1.1. Título del Reto
**Implantación y gestión de la infraestructura de red, servicios centralizados y aula informática para "Autoescuela MotorClass"**

## 1.2. Justificación y Alcance
La **Autoescuela MotorClass** es un centro de formación vial profesional que cuenta con una zona de recepción (2 puestos de trabajo), un despacho de dirección, un aula informática equipada con 20 ordenadores para la realización de test por parte de los alumnos, y una plantilla docente compuesta por 1 profesor de teórica y 4 profesores de práctica a cargo de la flota de vehículos.

Debido al crecimiento de la actividad y la necesidad de cumplir con la normativa de protección de datos y eficiencia operativa, el centro requiere actualizar su arquitectura tecnológica para dar respuesta a las siguientes necesidades:
* **Seguridad y aislamiento de red:** Separar el tráfico de la gestión administrativa (donde se manejan datos personales, expedientes de la DGT y facturación) de la red del aula informática y la red Wi-Fi ofrecida a los alumnos.
* **Control y restricciones en el aula:** Garantizar mediante políticas de grupo centralizadas que los 20 equipos del aula permanezcan congelados/restringidos, impidiendo la instalación de software, cambios en el sistema o descargas no autorizadas.
* **Gestión centralizada de recursos:** Configurar un controlador de dominio para la autenticación de usuarios, servicios de red (DHCP y DNS) y almacenamiento compartido con control de acceso basado en roles para las recepcionistas y la dirección.
* **Continuidad de negocio:** Desplegar un plan de copias de seguridad automáticas y periódicas para proteger las bases de datos de expedientes y la información contable frente a pérdidas de datos o fallos de hardware.

## 1.3. Objetivos del Proyecto
* **Diseñar y segmentar la red en VLANs:** Implementar una topología estructurada en cuatro VLANs (Administración, Aula, Wi-Fi Invitados y Gestión).
* **Desplegar un Servidor de Dominio:** Centralizar la gestión de identidades y aplicar políticas de seguridad (GPOs) sobre los equipos del aula.
* **Implementar servicios de red y almacenamiento:** Configurar asignación dinámica de IP (DHCP), resolución de nombres local (DNS) y un recurso compartido con permisos segmentados.
* **Automatizar las copias de seguridad:** Diseñar una rutina de respaldo automático para garantizar la integridad y disponibilidad de la información crítica.
