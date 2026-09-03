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
| --- | --- |
| **ID** | HU-03 |
| **Título** ||
| **Descripción** | |
| **Prioridad** | |
| **Estimación** | |

| Campo | Descripción |
| --- | --- |
| **ID** | HU-04 |
| **Título** | Validación de pago de inscripción |
| **Descripción** | Como organizador, quiero validar y aprobar (o rechazar) el pago de inscripción de un equipo, para asegurar que solo equipos con pago confirmado participen en el torneo |
| **Prioridad** |Media |
| **Estimación** |5 puntos de historia |

### 3. Tareas:

| Campo | Descripción |
| --- | --- |
| **ID** | TR-10 |
| **Título** | Diseñar el flujo de validación de pago |
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | Diseñar el flujo completo de validación, incluyendo el caso de rechazo y la notificación al capitán |
| **Tareas requisito** | ninguna |

| Campo | Descripción |
| --- | --- |
| **ID** | TR-11 |
| **Título** | Implementar cambio de estado del pago |
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | Implementar el cambio de estado del pago (pendiente → aprobado/rechazado) según la decisión del organizador |
| **Tareas requisito** | TR-10 |

| Campo | Descripción |
| --- | --- |
| **ID** | TR-12 |
| **Título** | Implementar notificación de rechazo |
| **ID de la Historia de Uso asociada** | HU-04 |
| **Descripción** | Implementar la notificación al capitán del equipo cuando su pago sea rechazado |
| **Tareas requisito** | TR-10, TR-11 |