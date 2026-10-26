# Roadmap

Cada fase tiene criterios de salida explícitos. El avance hacia la fase siguiente requiere cumplirlos, no declararlos.

## Fase 0 — Definición *(actual)*

- Documentación de objetivos, alcance, métricas, arquitectura, modelo de negocio y roadmap.
- **Criterio de salida:** definiciones estables y revisadas; ninguna afirmación sin fuente o verificación pendiente marcada.

## Fase 1 — Núcleo ejecutable

- Runner local mínimo: definiciones de tareas, al menos un adaptador de agente, evaluador de correctitud, registro de acciones y costos, reporte local.
- Gates de seguridad básicos: verificación de permisos y canaries de secretos.
- Documentación base legible por agentes (instalación, esquemas, ejemplos) publicada desde el inicio del código, no después.
- **Criterio de salida:** una persona externa puede ejecutar una evaluación completa sobre un repositorio público siguiendo solo la documentación.

## Fase 2 — Casos públicos

- 2–3 estudios comparativos sobre repositorios open source: flujo base vs. agente, con métricas completas, limitaciones e incertidumbre.
- Publicación con datos reproducibles; comunicación en redes sociales como evidencia documentada, no como publicidad.
- Contacto temprano con equipos para validar hipótesis de demanda: qué agentes usan, qué tareas delegan, qué decisión necesitan tomar.
- **Criterio de salida:** al menos un estudio revisado o reproducido por un tercero; demanda concreta identificada.

## Fase 3 — Primeros ingresos

- GitHub Sponsors activo con tiers; primer paquete de documentación avanzada en repositorio sponsors-only.
- Programa de acceso para contribuidores.
- Primera implementación guiada de evaluación (alcance fijo, equipo externo).
- **Criterio de salida:** primer cobro efectivo → **nivel 5 de la escala de Conjecture 56** para este proyecto.

## Fase 4 — Recurrencia

- Paquetes actualizados periódicamente; segundo paquete si la demanda lo justifica.
- Segunda y tercera implementación guiada.
- Evaluación de necesidad real de capacidades empresariales (multi-proyecto, SSO, políticas versionadas): se construyen solo si varios clientes las piden.
- **Criterio de salida:** ingresos recurrentes o repetidos de más de un cliente.

## Fase 5 — Consolidación

- Licencias por organización si hay demanda demostrada.
- Decisión sobre capacidades avanzadas del core vs. paquetes.
- Eventual incorporación de colaboradores, manteniendo la restricción de custodia cero.

## Fuera de horizonte inmediato

- Datos regulados (clínicos, financieros): solo con socio institucional, revisión jurídica y controles maduros.
- Producto SaaS gestionado: incompatible con la restricción de custodia cero.
- Framework generalista de agentes: fuera del enfoque de evaluación.
