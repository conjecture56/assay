# Alcance

## Dentro del alcance

- Runner local de evaluaciones, ejecutado en la infraestructura de quien lo utiliza.
- Definición versionable de tareas con criterios de aceptación verificables.
- Adaptadores para agentes y modelos, incluyendo ejecución local.
- Métricas de corrección, tiempo, intervención humana, costo y esfuerzo de revisión.
- Pruebas de seguridad observables: verificación de permisos, detección de exfiltración mediante canaries, ataques de prompt injection, acciones no autorizadas.
- Generación de reportes locales reproducibles.
- Casos de estudio públicos sobre repositorios open source y datos sintéticos.
- Documentación base completa, legible por personas y agentes, de acceso gratuito.

## Fuera del alcance

- **Servidores de Conjecture 56 que reciban o procesen datos de clientes.** Esta restricción es permanente: ni código fuente, ni datasets, ni prompts, ni trazas, ni resultados operativos de terceros atraviesan infraestructura de Conjecture 56.
- **Auditorías independientes sobre sistemas del cliente.** Sin acceso directo a la evidencia, el servicio correcto es una implementación guiada o una evaluación autogestionada verificable, no una auditoría.
- **Datos regulados en fases tempranas.** Información clínica, financiera u otra categoría sensible requiere base legal, contratos con subprocesadores, evaluación formal de riesgos y revisión jurídica por jurisdicción. No se contempla en las primeras fases.
- **Acuerdos de nivel de servicio de soporte.** En esta etapa el soporte se cubre con documentación completa; los problemas que solo pueden reproducirse con datos privados pertenecen al entorno del cliente.
- **Plataforma genérica de observabilidad.** El espacio de dashboards de trazas y costos ya está cubierto por otros productos; Assay no compite allí.

## Perfiles de datos

| Perfil | Contenido | Adecuado para |
|---|---|---|
| Público | Repositorios open source, datos sintéticos o públicos | Fases tempranas, casos de estudio, desarrollo del core |
| Confidencial | Código o datos privados del cliente | Ejecución íntegramente en infraestructura del cliente, con exportación únicamente de evidencia sanitizada |
| Regulado | Información clínica, financiera o personal protegida | Diferido; requiere socio institucional, revisión jurídica y controles maduros |

## Distinciones que no deben difuminarse

- **Self-hosted** significa que los datos no llegan a Conjecture 56. No significa que nada salga del cliente: si quien lo usa configura proveedores de modelos o herramientas externas, esos flujos existen y deben ser visibles en la herramienta.
- **"Todo permanece local"** solo puede afirmarse cuando agente, modelos, herramientas, logs y almacenamiento son locales y existe control de salida de red.
- **Controles observados** no equivalen a garantía de seguridad futura: el reporte distingue controles verificados, configuración comprobada, compromisos contractuales de proveedores y riesgos residuales.
