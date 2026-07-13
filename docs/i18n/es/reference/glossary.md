# Glosario (Español)

Definiciones claras para términos clave usados en Machine Learning 101.

## Fundamentos de ML

- **Machine Learning (ML)**: técnica para aprender patrones desde datos y predecir.
- **Modelo**: patron aprendido que transforma entradas en salidas.
- **Feature**: variable de entrada (edad, precio, temperatura).
- **Target/Label**: valor que el modelo debe predecir.
- **Entrenamiento**: etapa donde el modelo aprende con ejemplos.
- **Inferencia**: uso del modelo entrenado en datos nuevos.
- **Overfitting**: memoriza datos de entrenamiento y falla en datos nuevos.
- **Underfitting**: modelo muy simple; no aprende suficiente.

## Conceptos de Software

- **Software**: instrucciones escritas en código para resolver tareas.
- **Software engineer**: diseÃ±a, construye y mantiene sistemas de software.
- **Script**: programa corto para automatizar pasos.
- **API**: forma estandar de comunicación entre sistemas.
- **Endpoint**: URL que recibe solicitudes y devuelve respuestas.
- **Backend**: parte servidor donde corre la logica principal.
- **Frontend**: parte visual con la que interactua el usuario.
- **Repositorio (repo)**: carpeta con código e historial de cambios.
- **Git**: herramienta de control de versiones.
- **Logs**: registro de eventos para observabilidad y debug.

## Plataforma Azure ML

- **Workspace**: contenedor principal del proyecto en Azure ML.
- **Compute instance**: VM unica para desarrollo interactivo.
- **Compute cluster**: conjunto escalable para jobs de entrenamiento.
- **Environment**: versión fija de runtime y paquetes.
- **Data asset**: referencia versionada de datos.
- **Job**: una ejecución registrada de código.
- **Model registry**: almacénamiento versionado de modelos.
- **Project history**: trazabilidad de datos, código, entorno y despliegue.

## Evaluación

- **MAE**: error absoluto medio.
- **RMSE**: error cuadratico medio (penaliza más errores grandes).
- **R2**: porcentaje de variacion explicado por el modelo.
- **Accuracy**: porcentaje total de aciertos.
- **Precision**: de positivos predichos, cuantos eran positivos reales.
- **Recall**: de positivos reales, cuantos fueron detectados.
- **F1**: equilibrio entre precision y recall.

## Operacion

- **Monitoreo**: seguimiento de calidad y estabilidad del modelo.
- **Data drift**: los datos actuales cambian respecto al entrenamiento.
- **Canary**: liberar una nueva versión con poco trafico primero.
- **Blue/Green**: dos versiones en paralelo para cambio seguro.
