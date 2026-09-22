# 1. Introducción

## 1.1. Título del reto
Infraestructura IT de Alta Disponibilidad, Observabilidad y Seguridad Avanzada para GamerCore Studios

## 1.2. Contexto
GamerCore Studios S.L. es una startup dedicada al desarrollo de videojuegos de alta fidelidad gráfica. Tras una primera fase en la que se desplegó la infraestructura básica de red, servidores de dominio y base de datos, el crecimiento del equipo y la necesidad de proteger la propiedad intelectual exigen evolucionar la plataforma técnica hacia un entorno de producción de alta disponibilidad, monitorización en tiempo real y arquitectura de red robusta.

## 1.3. Problemática o necesidad
Actualmente, la infraestructura del estudio presenta una serie de deficiencias críticas que impiden su correcto escalado y ponen en riesgo la continuidad del negocio:

- **Riesgo de pérdida de información y tiempos de parada:** La ausencia de mecanismos de redundancia en los servicios centrales provoca que cualquier fallo en el hardware principal detenga por completo el trabajo del equipo creativo.
- **Falta de visibilidad sobre el sistema:** No existe un sistema centralizado que alerte en tiempo real sobre caídas de servicios, saturación de red o intentos de acceso no autorizados.
- **Vulnerabilidad de la propiedad intelectual:** El intercambio de archivos pesados y el acceso de usuarios externos sin políticas de aislamiento estrictas exponen los recursos críticos de la empresa a posibles fugas de datos.
- **Gestión ineficiente de recursos:** La falta de automatización en el despliegue de entornos provoca retrasos en las entregas del equipo de desarrollo.

- ## 1.4. Objetivos

### Objetivo general
Evolucionar y consolidar la infraestructura informática de GamerCore Studios S.L. mediante el despliegue de servicios en alta disponibilidad, sistemas de observabilidad y un portal de documentación técnica web automatizado.

### Objetivos específicos
- Diseñar una topología de red redundante y segmentada que garantice la continuidad del tráfico de producción.
- Desplegar mecanismos de monitorización en tiempo real para anticipar fallos de rendimiento y seguridad.
- Centralizar la gestión de identidades y permisos de los empleados del estudio.
- Automatizar la generación y publicación de la documentación técnica mediante integración continua.

## 1.5. Interesados

| Interesado | Relación con el proyecto | Necesidad principal |
|---|---|---|
| Equipo de Dirección | Promotores del proyecto | Garantizar la continuidad del negocio y la protección de los datos. |
| Desarrolladores y Diseñadores | Usuarios finales internos | Disponer de almacenamiento rápido, baja latencia y alta disponibilidad. |
| Equipo de Administración / IT | Operadores del sistema | Contar con monitorización centralizada, alertas y despliegues automatizados. |
| Inversores y Clientes | Usuarios externos | Acceder a un portal web corporativo ágil y con documentación actualizada. |
