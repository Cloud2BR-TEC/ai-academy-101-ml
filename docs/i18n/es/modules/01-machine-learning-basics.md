# 01. Fundamentos de aprendizaje automático

Machine learning es una forma de ensenar computadoras con ejemplos, en lugar de escribir todas las reglas manualmente.

## Enlaces Rápidos

- Construir el primer modelo: [Módulo 05](05-build-your-first-model.md)
- Desplegar modelo: [Módulo 06](06-deploy-and-score.md)
- Cierre del curso: [Módulo 09](09-wrap-up-and-next-steps.md)

## Qué Es y Que No Es ML

Machine learning **si es**:

- Metodo para encontrar patrones en datos.
- Forma de predecir casos nuevos.
- Proceso con entrenamiento, prueba y evaluación.

Machine learning **no es**:

- Reemplazo de definir bien el problema.
- Garantia de respuesta perfecta.
- Tarea de una sola vez.

## Programacion Tradicional vs ML

En programacion tradicional, se codifican reglas explicitas.
En ML, se entregan ejemplos y el sistema aprende patrones.

![Comparacion Programacion vs ML](../assets/img/programming-vs-ml.svg)

## Cómo Aprende un Modelo

Un modelo toma entradas y genera una predicción.
Durante entrenamiento, compara su predicción con la respuesta correcta y ajusta sus parámetros para reducir error.

![Cómo predice un modelo](../assets/img/how-model-predicts.svg)

## Vocabulario Clave

| Término | Significado |
|------|----------|
| **Data** | Conjunto de ejemplos para entrenar o predecir. |
| **Característica** | Variable de entrada (edad, precio, temperatura). |
| **Variable objetivo / Etiqueta** | Valor que el modelo debe predecir. |
| **Entrenamiento** | Etapa donde el modelo aprende con ejemplos. |
| **Prueba** | Evaluación con datos no vistos. |
| **Modelo** | Función aprendida que transforma entradas en salida. |
| **Predicción** | Salida del modelo para un caso nuevo. |
| **Algoritmo** | Método de aprendizaje (árboles, regresión, redes). |

## Características y Variable Objetivo

Todo problema de ML tiene entradas (características) y salida (variable objetivo).

![Características vs variable objetivo](../assets/img/feature-target-explained.svg)

## Tipos de Machine Learning

- **Supervisado**: datos con etiqueta.
- **No supervisado**: descubre estructura sin etiqueta.
- **Refuerzo**: aprende por recompensa/castigo.

![Tres tipos de ML](../assets/img/three-ml-types.svg)
![Tipos de ML](../assets/img/machine_learning_types.svg)

## Calidad de Datos

La calidad del modelo depende de la calidad del dato.
Problemas comunes:

- Valores faltantes.
- Etiquetas incorrectas.
- Sesgo de muestreo.
- Variables irrelevantes.

![Ingeniería de características](../assets/img/feature_engineering_collect_data.svg)

## Proceso de Punta a Punta

1. Definir problema.
2. Recolectar y preparar datos.
3. Entrenar modelo.
4. Evaluar con datos no vistos.
5. Desplegar.
6. Monitorear y reentrenar.

![Proceso por etapas](../assets/img/ml_process_by_stages.svg)
![Workflow ML](../assets/img/ml_workflow_stages.svg)

## Ejemplo: Precio de Casas

- **Características**: m2, dormitorios, barrio, antigüedad.
- **Variable objetivo**: precio.
- **Algoritmo**: regresión lineal.

![Regresion lineal](../assets/img/linear-regression-fit.svg)

## Relacion con Software Engineering

Los proyectos de ML también son proyectos de software:

- Se usa código, repositorio, control de versiones y logs.
- Se exponen modelos por APIs.
- Se mantiene calidad en produccion.

## Perspectiva Final

ML es aprender de ejemplos, validar con honestidad y aplicar el patron a datos nuevos para apoyar decisiones reales.
