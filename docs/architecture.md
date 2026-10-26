# Arquitectura

## Modelo de ejecución

Assay se ejecuta íntegramente en la infraestructura de quien lo utiliza. Conjecture 56 no recibe código, datos, prompts, trazas ni resultados operativos.

```text
Infraestructura del usuario
├── Repositorio o datos bajo evaluación
├── Runner de Assay
│   ├── Definiciones de tareas (versionadas)
│   ├── Adaptadores de agente / modelo
│   ├── Sandbox de ejecución
│   ├── Herramientas autorizadas (permit lists)
│   ├── Registro de acciones y costos
│   ├── Pruebas de seguridad (gates + canaries)
│   └── Generador de reportes locales
└── Almacenamiento local de resultados

Exportación opcional, decidida por el usuario:
métricas agregadas y evidencia sanitizada → fuera del entorno
```

## Componentes

| Componente | Responsabilidad |
|---|---|
| Definiciones de tareas | Describir tareas representativas con criterios de aceptación verificables, establecidos antes de ejecutar |
| Adaptadores de agente | Uniformar la interacción con distintas herramientas de agentes y proveedores de modelos, locales o remotos |
| Sandbox | Aislar la ejecución: sistema de archivos, red, credenciales temporales de alcance mínimo |
| Registro de acciones | Capturar qué hizo el agente, qué consumió y qué costo generó |
| Pruebas de seguridad | Ejecutar gates de permisos, exfiltración, injection y aprobaciones, incluyendo canaries |
| Evaluador | Calcular métricas y comparar modalidades bajo condiciones documentadas |
| Reportes | Producir resultados reproducibles y distinguir evidencia observada de expectativa |
| Exportación de evidencia | Convertir resultados en paquetes sanitizados, solo cuando el usuario lo decide |

## Límites del modelo

- **Assay no intermedía proveedores externos.** Si el usuario configura un modelo remoto, los flujos hacia ese proveedor existen; la herramienta debe registrarlos y hacerlos visibles, no ocultarlos.
- **"Todo permanece local"** es una configuración verificable, no una promesa por defecto: requiere agente, modelos, herramientas, logs y almacenamiento locales, más control de salida de red.
- **La exportación es optativa y explícita.** El caso de estudio público típico usa repositorios públicos, donde la exportación completa es segura; en entornos confidenciales, solo métricas agregadas.
- **Sin telemetría, sin cuentas, sin control plane.** Ningún componente del core requiere conectarse a infraestructura de Conjecture 56.

## Entornos de referencia

El desarrollo y los casos públicos se realizan sobre repositorios open source con tests verificables. Los entornos confidenciales se soportan por diseño (ejecución local, exportación sanitizada) pero se validan primero en entornos públicos.
