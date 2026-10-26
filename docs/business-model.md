# Modelo de negocio

Restricción permanente: **Conjecture 56 nunca recibe ni procesa datos de clientes.** Todo el modelo se sostiene sobre distribuir metodología y software, no sobre operar infraestructura de terceros.

## Capa gratuita

- **Core open source:** runner local, definiciones de tareas, adaptadores, métricas, pruebas de seguridad básicas y reportes locales.
- **Documentación base completa y legible por agentes:** instalación, configuración, esquemas, ejemplos reproducibles y referencia técnica. Es el mecanismo de adopción y reputación; se mantiene libre sin excepciones.
- **Casos de estudio públicos:** evidencia comparada sobre repositorios open source.
- Sin telemetría obligatoria, sin cuentas, sin control plane.

## Contenido pago: paquetes de documentación avanzada

Paquetes versionados, sin datos de clientes, mantenidos por Conjecture 56:

- Escenarios especializados por dominio: prompt injection, permisos y acciones prohibidas, protección de secretos, fallos de herramientas, reintentos e idempotencia, flujos de análisis de datos.
- Playbooks de evaluación: interpretación de métricas, diseño de conjuntos de tareas, configuración de controles.
- Guías de integración con agentes y modelos específicos.
- Actualizaciones continuas de los paquetes ante cambios del ecosistema.

**Distribución:** repositorios privados vinculados a tiers de GitHub Sponsors (sponsors-only repositories). GitHub gestiona invitaciones y revocaciones automáticamente; no se requiere infraestructura propia de licencias ni pagos.

**Contribuidores:** quienes aporten al menos un pull request aceptado acceden sin costo mientras permanezcan activos. Beneficios adicionales no monetarios: créditos, participación en decisiones sobre nuevos paquetes.

## Primera unidad vendible

**Implementación guiada de evaluación (alcance fijo):**

1. Instalación de la herramienta en infraestructura del cliente.
2. Capacitación del responsable interno.
3. Configuración y ejecución de un conjunto de tareas (10–20) por parte del equipo del cliente.
4. Generación del reporte, que permanece en el entorno del cliente.
5. Interpretación conjunta de las métricas que el cliente decida compartir.
6. Protocolo documentado para repetir la evaluación.

Se vende metodología, instalación, capacitación, paquetes e interpretación — **no acceso a activos del cliente**.

## Extensiones posteriores

- Paquetes por organización (licencias por equipo).
- Marca blanca u OEM para consultoras y plataformas.
- Capacitación y certificación de operadores de la metodología.

## Lo que este modelo no ofrece

- **Soporte con SLA** en esta etapa: la carga operativa se resuelve con documentación; los problemas reproducibles solo con datos privados pertenecen al cliente.
- **Auditoría independiente:** sin acceso a evidencia, el servicio es una evaluación autogestionada verificable o una implementación guiada. El lenguaje comercial respeta esta distinción.
- **Garantías de seguridad absolutas:** se comunican controles observados y riesgos residuales, nunca certificaciones implícitas.
