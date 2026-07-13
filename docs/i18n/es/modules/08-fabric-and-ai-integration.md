# 08. Fabric e Integración con AI

Microsoft Fabric unifica analítica de datos y complementa Azure ML.

Visión para principiantes: Fabric prepara datos y reportes; Azure ML entrena y despliega modelos.

## Enlaces Rápidos

- Fundamentos de modelos: [Módulo 01](01-machine-learning-basics.md)
- Construcción de modelos: [Módulo 05](05-build-your-first-model.md)
- Despliegue de endpoints: [Módulo 06](06-deploy-and-score.md)

![Datos y targets](../assets/img/collect_data_init_primary_second_targets.svg)

## Qué es Microsoft Fabric

- **OneLake**: lugar unificado de datos.
- **Data Factory**: movimiento y transformación de datos.
- **Data Engineering**: preparación de datos a gran escala.
- **Data Science**: notebooks para experimentos.
- **Power BI**: dashboards y reportes.

## Fabric + Azure ML

| Etapa | Fabric | Azure ML |
|-------|--------|----------|
| Ingesta de datos | ✓ | |
| Transformación de datos | ✓ | |
| Feature engineering a escala | ✓ (Spark) | |
| Entrenamiento y tracking | | ✓ |
| Deploy y endpoints | | ✓ |
| Batch scoring a gran escala | ✓ | ✓ |
| Reporting de predicciones | ✓ | |

![Guía de tamaño de dataset](../assets/img/msft-dataset-size-guidance.svg)

## LangChain y SynapseML

- **SynapseML**: librería para ML a gran escala en Spark.
- **LangChain**: orquesta flujos con prompts, herramientas y LLM.

Son opcionales para principiantes. Primero dominar: datos, entrenamiento, evaluación y deploy.

## Conexión Azure OpenAI en Fabric

```python
import os
from langchain_openai import AzureChatOpenAI

os.environ["OPENAI_API_VERSION"] = "2024-02-01"
os.environ["AZURE_OPENAI_ENDPOINT"] = "https://your-resource.openai.azure.com"
os.environ["AZURE_OPENAI_API_KEY"] = "your-key"

llm = AzureChatOpenAI(deployment_name="gpt-4o", temperature=0.2)
response = llm.invoke("Resume riesgos clave del reporte: ...")
```

No es necesario memorizar este código ahora; el objetivo es entender la integración.

![Python dtype](../assets/img/python_dtype.svg)

## Guía de Decisión

**Usa Fabric cuando:**

- Tu cuello de botella es preparación/analítica de datos.
- Necesitas procesamiento distribuido y reportes.

**Usa Azure ML cuando:**

- Tu foco es entrenar, evaluar y desplegar modelos.
- Necesitas versionado, historial de proyecto y monitoreo.
- Necesitas endpoints online con objetivos de tiempo de respuesta.

**Usa ambos cuando:**

- Preparas datos en Fabric y despliegas modelos en Azure ML.
