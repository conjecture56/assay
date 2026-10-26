# Assay — Evaluación de flujos de trabajo con agentes de IA

Assay es un proyecto de investigación aplicada de [Conjecture 56](https://github.com/conjecture56). Su objetivo es evaluar, de manera **reproducible y verificable**, si incorporar agentes de IA a un flujo de trabajo real produce valor medible sin exceder límites sobre código, datos, permisos y costos.

Assay no es otra plataforma de observabilidad ni un benchmark genérico. Es una metodología y una herramienta para responder, con evidencia, la pregunta que toda organización enfrenta hoy:

> ¿Este agente mejora realmente nuestro trabajo? ¿En qué tareas? ¿Cuánto cuesta? ¿Qué riesgos introduce? ¿Qué controles necesitamos?

## Características

- **Self-hosted:** se ejecuta en la infraestructura de quien lo usa. Conjecture 56 no opera servidores que reciban ni procesen código, datos, prompts, trazas o resultados de terceros.
- **Sin custodia de datos:** ni cuentas obligatorias, ni telemetría, ni control plane externo.
- **Verificación antes que volumen:** la seguridad es un criterio de aprobación, no una métrica más. Un agente que completa tareas pero filtra secretos falla la evaluación.
- **Evidencia reproducible:** tareas, condiciones, costos y limitaciones se documentan para cada comparación.
- **Legible por agentes:** la documentación base está escrita para que tanto personas como agentes puedan operar la herramienta sin asistencia externa.

## Estado

Proyecto en definición. Esta etapa establece objetivos, alcance, modelo de medición, arquitectura conceptual y modelo de negocio. Aún no existe código ejecutable.

## Documentación

| Documento | Contenido |
|---|---|
| [Objetivos](docs/objectives.md) | Propósito del proyecto y preguntas de investigación |
| [Alcance](docs/scope.md) | Qué incluye y qué excluye explícitamente |
| [Métricas](docs/metrics.md) | Dimensiones de valor y criterios de seguridad |
| [Arquitectura](docs/architecture.md) | Componentes y modelo de ejecución local |
| [Modelo de negocio](docs/business-model.md) | Cómo se sostiene sin servicios con custodia de datos |
| [Roadmap](docs/roadmap.md) | Fases y criterios de avance |

## Relación con Conjecture 56

Assay aplica las dos líneas de investigación definidas en el [charter](https://github.com/conjecture56/charter):

- **Agentic Engineering Lab:** cómo organizar y evaluar el trabajo realizado por personas y agentes.
- **Agent Systems Lab:** permisos, aislamiento, confiabilidad y economía de la ejecución.

Conjecture 56 conserva su carácter de investigación aplicada independiente: el objetivo no es promocionar agentes, sino medirlos.
