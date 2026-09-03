# 📄 Planeación del Sistema

## Desglose de trabajo: Épicas, Historias de Usuario y Tareas



### 1. Épica:

| Campo | Descripción |
| --- | --- |
| **ID** | EP-01 |
| **Título** | Registro y gestión de torneos y equipos en TechCup |
| **Descripción** | TechCup necesita permitir que los organizadores creen torneos y que los capitanes registren equipos y paguen su inscripción, ya que sin esta base no puede existir ninguna otra operación del sistema (validación de pagos, reportes) |
| **Stakeholder** | Decanatura de Ingeniería de Sistemas / Organizadores del torneo |

### 2. Historias de usuario:

| Campo | Descripción |
| --- | --- |
| **ID** | HU-01 |
| **Título** | |
| **Descripción** | |
| **Prioridad** | |
| **Estimación** | |

| Campo | Descripción |
| --- | --- |
| **ID** | HU-02 |
| **Título** | |
| **Descripción** | |
| **Prioridad** | |
| **Estimación** | |

| Campo | Descripción |
|---|---|
| **ID** | HU-03 |
| **Título** | Consulta de equipos registrados en un torneo |
| **Descripción** | Como organizador, quiero visualizar la lista de equipos registrados en un torneo, para verificar el estado de las inscripciones y hacer seguimiento antes de que inicie el torneo |
| **Prioridad** | Media |
| **Estimación** | 3 puntos |

| Campo | Descripción |
| --- | --- |
| **ID** | HU-04 |
| **Título** | Validación de pago de inscripción |
| **Descripción** | Como organizador, quiero validar y aprobar (o rechazar) el pago de inscripción de un equipo, para asegurar que solo equipos con pago confirmado participen en el torneo |
| **Prioridad** | Media |
| **Estimación** |5 puntos de historia |

### 3. Tareas:


| Campo | Descripción |
|---|---|
| **ID** | TR-07 |
| **Título** | Diseñar consulta de equipos por torneo |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Definir la lógica y estructura de datos para obtener todos los equipos asociados a un torneo específico |
| **Tareas requisito** | Ninguna |

| Campo | Descripción |
|---|---|
| **ID** | TR-08 |
| **Título** | Implementar endpoint/vista de listado |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Desarrollar la funcionalidad backend (y/o vista) que devuelve la lista de equipos registrados, con filtro por torneo |
| **Tareas requisito** | TR-07 |

| Campo | Descripción |
|---|---|
| **ID** | TR-09 |
| **Título** | Pruebas de la funcionalidad de listado |
| **ID de la Historia de Uso asociada** | HU-03 |
| **Descripción** | Escribir pruebas unitarias que validen el listado correcto (torneo con equipos, torneo vacío, acceso restringido a organizador) |
| **Tareas requisito** | TR-08 |

| Campo | Descripción |
| --- | --- |
| **ID** | TR-10 |
| **Título** | Diseñar el flujo de validación de pago |
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | Como desarrollador, quiero diseñar el flujo de validación de pago, para tener una base clara antes de implementar la funcionalidad |
| **Tareas requisito** | ninguna |

| Campo | Descripción |
| --- | --- |
| **ID** | TR-11 |
| **Título** | Implementar cambio de estado del pago |
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | Como desarrollador, quiero implementar el cambio de estado del pago, para que el sistema refleje la decisión del organizador |
| **Tareas requisito** | TR-10 |

| Campo | Descripción |
| --- | --- |
| **ID** | TR-12 |
| **Título** | Implementar notificación de rechazo |
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | Como desarrollador, quiero implementar la notificación al capitán cuando su pago sea rechazado, para que el equipo se entere y pueda corregir su inscripción |
| **Tareas requisito** | TR-10, TR-11 |
