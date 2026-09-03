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
