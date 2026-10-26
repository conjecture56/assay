# Objetivos

## Objetivo general

Producir evaluaciones reproducibles de flujos de trabajo con agentes de IA que midan valor real — corrección, costo, tiempo, esfuerzo de revisión y seguridad — sin exceder límites sobre código, datos, permisos y proveedores.

## Pregunta central

> ¿En qué tareas este agente aporta valor real a este equipo y bajo qué controles conviene utilizarlo?

## Objetivos específicos

- Definir un formato común de tareas evaluables, con criterios de corrección establecidos antes de ejecutar.
- Comparar, bajo condiciones documentadas, el flujo actual de un equipo contra flujos asistidos o delegados a agentes.
- Medir trabajo correcto y mantenible por unidad de tiempo, costo y riesgo, incluyendo el costo de revisión humana.
- Verificar que la ejecución respeta límites de permisos, aislamiento y salida de información, mediante pruebas observables y señuelos (canaries).
- Determinar qué tareas conviene asistir, delegar o mantener bajo ejecución humana, con recomendaciones explícitas de adoptar, limitar, cambiar o descartar.
- Publicar casos de estudio sobre repositorios públicos con datos suficientes para reproducción independiente.

## Relación con las líneas de Conjecture 56

Assay materializa las dos líneas definidas en el [charter](https://github.com/conjecture56/charter):

| Línea | Aporte de Assay |
|---|---|
| Agentic Engineering Lab | Metodología para organizar, medir y evaluar el trabajo de ingeniería realizado por personas y agentes |
| Agent Systems Lab | Evaluación de permisos, aislamiento, confiabilidad y costo de la ejecución de agentes |

## Principios

- **Evidencia antes que promoción:** los resultados se comunican con limitaciones explícitas; no hay publicidad simulada.
- **Verificación antes que volumen:** más tareas completadas no implica mayor productividad.
- **Responsabilidad humana:** quien adopta un resultado debe poder explicarlo, verificarlo y sostenerlo.
- **Independencia de proveedores:** los métodos se evalúan separadamente de las capacidades promocionadas por cada herramienta.
- **Adopción condicionada por el contexto:** no existe un único nivel de autonomía adecuado para todas las tareas.
