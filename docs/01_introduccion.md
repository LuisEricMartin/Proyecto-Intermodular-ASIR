# 1. Introducción

## 1.1. Título del reto
Implantación y gestión de la infraestructura de red, servicios centralizados, base de datos y portal web para Autoescuela MotorClass.

## 1.2. Contexto
La Autoescuela MotorClass es un centro de formación vial que cuenta con una zona de recepción (2 puestos de trabajo), un despacho de dirección, un aula informática equipada con 20 ordenadores para la realización de test por parte de los alumnos, y una plantilla docente compuesta por 1 profesor de teórica y 4 profesores de práctica a cargo de la flota de vehículos.

## 1.3. Problemática o necesidad
Debido al crecimiento de la actividad y la necesidad de cumplir con la normativa de protección de datos y eficiencia operativa, el centro requiere resolver las siguientes necesidades operativas y tecnológicas desde cero:
* **Seguridad y aislamiento de la información:** Necesidad de separar el tráfico de gestión administrativa del acceso a internet del aula y de la red Wi-Fi ofrecida a los alumnos.
* **Control y restricciones en el aula:** Necesidad de garantizar que los 20 equipos del aula permanezcan protegidos frente a modificaciones no autorizadas por parte de los alumnos.
* **Gestión de datos y expedientes:** Necesidad de almacenar y consultar de forma estructurada y segura la información de alumnos, matrículas, profesores, vehículos y clases.
* **Presencia web y servicios en línea:** Necesidad de disponer de una plataforma web pública para promocionar los servicios de la autoescuela y permitir el contacto o acceso a servicios de los alumnos.
* **Gestión de identidades y recursos compartidos:** Necesidad de centralizar el acceso de los empleados a la información y disponer de almacenamiento compartido con permisos diferenciados.
* **Continuidad de negocio:** Necesidad de proteger la información crítica (base de datos, expedientes y contabilidad) mediante copias de respaldo frente a posibles fallos técnicos.

## 1.4. Objetivos

### Objetivo general
Diseñar e implantar desde cero una infraestructura tecnológica integral, segura y centralizada para la Autoescuela MotorClass que incluya red, servidores, gestión de base de datos, servicio web y aula de alumnos.

### Objetivos específicos
* Segmentar la red en zonas independientes según el tipo de uso (Administración, Aula, Wi-Fi e Infraestructura).
* Diseñar e implementar una base de datos relacional para la gestión integral de alumnos, expedientes, vehículos y clases.
* Desplegar y configurar un servidor web para alojar el sitio web corporativo de la autoescuela.
* Centralizar la gestión de usuarios y aplicar directivas de seguridad uniformes en todos los equipos informáticos.
* Desplegar servicios clave de red y un almacenamiento de archivos con control de acceso por roles.
* Establecer un sistema automatizado de copias de seguridad para garantizar la disponibilidad de los datos y bases de datos.

## 1.5. Interesados
| Interesado | Relación con el proyecto | Necesidad principal |
|---|---|---|
| Dirección de la autoescuela | Propietario / Cliente | Garantizar la seguridad de los datos, la presencia web, la continuidad del negocio y el control global de la infraestructura. |
| Recepcionistas | Usuarios internos | Disponer de un entorno ágil para gestionar matriculaciones, expedientes en la base de datos y archivos compartidos. |
| Alumnos | Usuarios externos | Contar con un aula informática funcional, acceso al portal web e internet estable sin interferir en la red privada. |
| Administrador de Sistemas (Tú) | Diseñador e implementador | Desplegar una infraestructura robusta, escalable y fácil de mantener desde cero. |
