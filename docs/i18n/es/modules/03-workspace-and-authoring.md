# 03. Workspace y Authoring

El workspace de Azure ML es el hogar del proyecto: datos, jobs, modelos y endpoints.

## Enlaces Rápidos

- Fundamentos de modelos: [Módulo 01](01-machine-learning-basics.md)
- Construcción de modelos: [Módulo 05](05-build-your-first-model.md)
- Despliegue de modelos: [Módulo 06](06-deploy-and-score.md)

## Componentes del Workspace

![Componentes del workspace](../assets/img/workspace-components.svg)

### Data Assets

Referencias versionadas de datasets para repetir experimentos de forma consistente.

### Compute

- **Compute instance**: VM para trabajo interactivo.
- **Compute cluster**: escalado automático para jobs.
- **Serverless**: recursos bajo demanda.
- **Kubernetes**: opcion de despliegue robusto.

### Jobs

Cada ejecución de entrenamiento queda registrada con parámetros, métricas y salidas.

### Environments

Versiones fijas de paquetes para reproducibilidad.

![Taxonomía de environment](../assets/img/azure-ml-environment-taxonomy.svg)

### Model Registry

Almacén de modelos versionados con metadata de origen.

### Endpoints

API HTTP para predicciones online o batch.

![Taxonomía Azure ML](../assets/img/azure-machine-learning-taxonomy.svg)

## Opciones de Authoring

### Notebooks

Ejecución por celdas para iterar rápido y aprender paso a paso.

### AutoML

Prueba algoritmos y configuraciones de forma automatica para obtener una buena base.

![AutoML](../assets/img/automl_diagram.svg)
![Proceso AutoML](../assets/img/automl_process_what_to_expect.svg)

### Designer

Interfaz visual de pipelines por bloques.

## Vocabulario

| Término | Significado |
|------|----------|
| **Experiment** | Grupo de ejecuciónes relacionadas. |
| **Run** | Una ejecución concreta. |
| **Pipeline** | Secuencia de pasos conectados. |
| **Output files** | Archivos de salida: modelo, métricas, logs. |
| **Project history** | Registro de que datos/código/entorno creo el modelo. |

![Flujo de entrenamiento](../assets/img/training_testing_data_flow.svg)

## Conexión Completa

Workspace organiza, compute ejecuta, jobs entrenan, environment asegura consistencia, registry guarda modelos y endpoint los publica.
