# 03. Workspace y Authoría

El workspace de Azure ML es el hogar del proyecto: datos, jobs, modelos y endpoints.

## Enlaces Rápidos

- Fundamentos de modelos: [Módulo 01](01-machine-learning-basics.md)
- Construcción de modelos: [Módulo 05](05-build-your-first-model.md)
- Despliegue de modelos: [Módulo 06](06-deploy-and-score.md)

## Componentes del Workspace

![Componentes del workspace](../assets/img/workspace-components.svg)

### Activos de datos

Referencias versionadas de datasets para repetir experimentos de forma consistente.

### Cómputo

- **Instancia de cómputo**: VM para trabajo interactivo.
- **Clúster de cómputo**: escalado automático para trabajos.
- **Serverless**: recursos bajo demanda.
- **Kubernetes**: opcion de despliegue robusto.

### Trabajos

Cada ejecución de entrenamiento queda registrada con parámetros, métricas y salidas.

### Entornos

Versiones fijas de paquetes para reproducibilidad.

![Taxonomía de environment](../assets/img/azure-ml-environment-taxonomy.svg)

### Registro de modelos

Almacén de modelos versionados con metadata de origen.

### Puntos de conexión

API HTTP para predicciones online o batch.

![Taxonomía Azure ML](../assets/img/azure-machine-learning-taxonomy.svg)

## Opciones de Authoría

### Cuadernos (Notebooks)

Ejecución por celdas para iterar rápido y aprender paso a paso.

### AutoML (Aprendizaje automático automatizado)

Prueba algoritmos y configuraciones de forma automatica para obtener una buena base.

![AutoML](../assets/img/automl_diagram.svg)
![Proceso AutoML](../assets/img/automl_process_what_to_expect.svg)

### Diseñador visual (Designer)

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
