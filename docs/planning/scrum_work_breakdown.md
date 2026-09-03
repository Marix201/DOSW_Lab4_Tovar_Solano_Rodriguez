# 📄 Planeación del Sistema

## Desglose de trabajo: Épicas, Historias de Usuario y Tareas



### 1. Épica:

| Campo | Descripción |
| --- | --- |
| **ID** | DOSW-1 |
| **Título** | Registro y gestión de torneos y equipos en TechCup |
| **Descripción** | TechCup necesita permitir que los organizadores creen torneos y que los capitanes registren equipos y paguen su inscripción, ya que sin esta base no puede existir ninguna otra operación del sistema (validación de pagos, reportes) |
| **Stakeholder** | Decanatura de Ingeniería de Sistemas / Organizadores del torneo |

### 2. Historias de usuario:

| Campo | Descripción |
| --- | --- |
| **ID** | DOSW-14|
| **Título** | Creación de torneo |
| **Descripción** | Como organizador, quiero crear un torneo especificando sus reglas básicas (fechas, tarifa de inscripción), para habilitar la etapa de inscripciones de equipos |
| **Prioridad** | Alta |
| **Estimación** | 8 puntos |

| Campo | Descripción |
| --- | --- |
| **ID** | DOSW-15 |
| **Título** | Registro e inscripción de equipo a un torneo |
| **Descripción** | Como capitán, quiero registrar mi equipo en el torneo activo y pagar la tarifa de inscripción mediante PSE, para formalizar la participación de mi equipo en el torneo |
| **Prioridad** | Alta |
| **Estimación** | 8 puntos |

| Campo | Descripción |
|---|---|
| **ID** | DOSW-9 |
| **Título** | Consulta de equipos registrados en un torneo |
| **Descripción** | Como organizador, quiero visualizar la lista de equipos registrados en un torneo, para verificar el estado de las inscripciones y hacer seguimiento antes de que inicie el torneo |
| **Prioridad** | Media |
| **Estimación** | 3 puntos |

| Campo | Descripción |
| --- | --- |
| **ID** | DOSW-2 |
| **Título** | Validación de pago de inscripción |
| **Descripción** | Como organizador, quiero validar y aprobar (o rechazar) el pago de inscripción de un equipo, para asegurar que solo equipos con pago confirmado participen en el torneo |
| **Prioridad** | Media |
| **Estimación** |5 puntos |

### 3. Tareas:


| Campo | Descripción |
| --- | --- |
| **ID** | DOSW-16 |
| **Título** | Diseñar modelo de datos del torneo |
| **ID de la Historia de Uso asociada** | DOSW-14 |
| **Descripción** | Como desarrollador, quiero diseñar el modelo de datos del torneo (ID de 5 dígitos, fechas, tarifa, estado), para tener una base clara antes de implementar la funcionalidad |
| **Tareas requisito** | Ninguna |

| Campo | Descripción |
| --- | --- |
| **ID** | DOSW-17 |
| **Título** | Implementar creación y cambio de estado del torneo |
| **ID de la Historia de Uso asociada** | DOSW-14 |
| **Descripción** | Como desarrollador, quiero implementar la creación de torneos y el cambio de sus estados (Pendiente, Activo, En progreso, Cerrado, Cancelado), para que el organizador pueda gestionarlos correctamente |
| **Tareas requisito** | DOSW-16 |

| Campo | Descripción |
| --- | --- |
| **ID** | DOSW-18 |
| **Título** | Validar regla de torneo único activo |
| **ID de la Historia de Uso asociada** | DOSW-14 |
| **Descripción** | Como desarrollador, quiero implementar la validación que garantiza que solo un torneo esté Activo a la vez, para cumplir con la regla de negocio del caso de estudio |
| **Tareas requisito** | DOSW-17 |

| Campo | Descripción |
| --- | --- |
| **ID** | DOSW-19 |
| **Título** | Diseñar flujo de registro de equipo |
| **ID de la Historia de Uso asociada** | DOSW-15 |
| **Descripción** | Como desarrollador, quiero diseñar la lógica y estructura de datos para registrar un equipo en el torneo activo, para tener una base clara antes de implementar la funcionalidad |
| **Tareas requisito** | Ninguna |

| Campo | Descripción |
| --- | --- |
| **ID** | DOSW-20 |
| **Título** | Implementar registro de equipo |
| **ID de la Historia de Uso asociada** | DOSW-15 |
| **Descripción** | Como desarrollador, quiero implementar el registro de un equipo en el torneo activo, para que el capitán pueda formalizar la participación de su equipo |
| **Tareas requisito** | DOSW-19 |

| Campo | Descripción |
| --- | --- |
| **ID** | DOSW-21 |
| **Título** | Integrar pago de inscripción por PSE |
| **ID de la Historia de Uso asociada** | DOSW-15 |
| **Descripción** | Como desarrollador, quiero integrar el pago de la tarifa de inscripción mediante PSE, dejando el pago en estado pendiente hasta su validación, para completar el flujo de registro del equipo |
| **Tareas requisito** | DOSW-20 |

| Campo | Descripción |
|---|---|
| **ID** | DOSW-11 |
| **Título** | Diseñar consulta de equipos por torneo |
| **ID de la Historia de Uso asociada** |DOSW-9 |
| **Descripción** | Como desarrollador, quiero diseñar la lógica y estructura de datos para obtener los equipos asociados a un torneo, para tener una base sólida antes de implementar el endpoint  |
| **Tareas requisito** | Ninguna |

| Campo | Descripción |
|---|---|
| **ID** | DOSW-12 |
| **Título** | Implementar endpoint/vista de listado |
| **ID de la Historia de Uso asociada** | DOSW-9 |
| **Descripción** | Como desarrollador, quiero implementar el endpoint o vista que devuelve la lista de equipos registrados filtrados por torneo, para que el organizador pueda consultarlos desde la interfaz  |
| **Tareas requisito** | DOSW-11 |

| Campo | Descripción |
|---|---|
| **ID** | DOSW-13 |
| **Título** | Pruebas de la funcionalidad de listado |
| **ID de la Historia de Uso asociada** | DOSW-9 |
| **Descripción** | Como desarrollador, quiero probar la funcionalidad de listado con distintos escenarios (torneo con equipos, torneo vacío, acceso no autorizado), para garantizar que funcione correctamente antes de entregarla  |
| **Tareas requisito** | DOSW-12 |

| Campo | Descripción |
| --- | --- |
| **ID** | DOSW-6 |
| **Título** | Diseñar el flujo de validación de pago |
| **ID de la Historia de Uso asociada** | DOSW-2 |
| **Descripción** | Como desarrollador, quiero diseñar el flujo de validación de pago, para tener una base clara antes de implementar la funcionalidad |
| **Tareas requisito** | ninguna |

| Campo | Descripción |
| --- | --- |
| **ID** | DOSW-7 |
| **Título** | Implementar cambio de estado del pago |
| **ID de la Historia de Uso asociada** | DOSW-2 |
| **Descripción** | Como desarrollador, quiero implementar el cambio de estado del pago, para que el sistema refleje la decisión del organizador |
| **Tareas requisito** | DOSW-6 |

| Campo | Descripción |
| --- | --- |
| **ID** | DOSW-8 |
| **Título** | Implementar notificación de rechazo |
| **ID de la Historia de Uso asociada** | DOSW-2 |
| **Descripción** | Como desarrollador, quiero implementar la notificación al capitán cuando su pago sea rechazado, para que el equipo se entere y pueda corregir su inscripción |
| **Tareas requisito** | DOSW-6, DOSW-7 |

### 4. Justificación de prioridades (Product Owner)

- **HU-01 (Alta):** Sin un torneo creado no puede existir ningún otro flujo del sistema.
- **HU-02 (Alta):** El registro y pago de equipos es la segunda base indispensable; sin equipos inscritos no hay nada que validar ni listar.
- **HU-03 (Media):** Es una consulta de apoyo para los organizadores, útil pero no bloqueante para el flujo principal.
- **HU-04 (Media):** Depende de que ya existan pagos registrados (HU-02), por lo que no es urgente en el arranque del sprint.
