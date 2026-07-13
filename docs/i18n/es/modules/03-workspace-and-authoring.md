# 03. Workspace y Authoring

El workspace de Azure ML es el hogar del proyecto: datos, jobs, modelos y endpoints.

## Enlaces Rapidos

- Fundamentos de modelos: [Modulo 01](01-machine-learning-basics.md)
- Construccion de modelos: [Modulo 05](05-build-your-first-model.md)
- Despliegue de modelos: [Modulo 06](06-deploy-and-score.md)

## Componentes del Workspace

![Componentes del workspace](../assets/img/workspace-components.svg)

### Data Assets

Referencias versionadas de datasets para repetir experimentos de forma consistente.

### Compute

- **Compute instance**: VM para trabajo interactivo.
- **Compute cluster**: escalado automatico para jobs.
- **Serverless**: recursos bajo demanda.
- **Kubernetes**: opcion de despliegue robusto.

### Jobs

Cada ejecucion de entrenamiento queda registrada con parametros, metricas y salidas.

### Environments

Versiones fijas de paquetes para reproducibilidad.

![Taxonomia de environment](../assets/img/azure-ml-environment-taxonomy.svg)

### Model Registry

Almacen de modelos versionados con metadata de origen.

### Endpoints

API HTTP para predicciones online o batch.

![Taxonomia Azure ML](../assets/img/azure-machine-learning-taxonomy.svg)

## Opciones de Authoring

### Notebooks

Ejecucion por celdas para iterar rapido y aprender paso a paso.

### AutoML

Prueba algoritmos y configuraciones de forma automatica para obtener una buena base.

![AutoML](../assets/img/automl_diagram.svg)
![Proceso AutoML](../assets/img/automl_process_what_to_expect.svg)

### Designer

Interfaz visual de pipelines por bloques.

## Vocabulario

| Termino | Significado |
|------|----------|
| **Experiment** | Grupo de ejecuciones relacionadas. |
| **Run** | Una ejecucion concreta. |
| **Pipeline** | Secuencia de pasos conectados. |
| **Output files** | Archivos de salida: modelo, metricas, logs. |
| **Project history** | Registro de que datos/codigo/entorno creo el modelo. |

![Flujo de entrenamiento](../assets/img/training_testing_data_flow.svg)

## Conexion Completa

Workspace organiza, compute ejecuta, jobs entrenan, environment asegura consistencia, registry guarda modelos y endpoint los publica.
