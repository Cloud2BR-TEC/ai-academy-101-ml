# 08. Fabric and AI Integration

Microsoft Fabric is a unified analytics platform that brings together data engineering, data warehousing, data science, real-time analytics, and business intelligence in a single environment. It complements Azure ML by handling the data side of the workflow.

![Collect data and targets](../assets/img/collect_data_init_primary_second_targets.svg)

## What Microsoft Fabric Is

Fabric organizes data work into experiences:

- **OneLake**: a single shared data lake for the entire organization. All data is stored once and accessed by every experience.
- **Data Factory**: data movement and transformation pipelines.
- **Synapse Data Engineering**: large-scale Spark-based data preparation.
- **Data Science**: notebook-based ML experiments, including SynapseML integration.
- **Power BI**: interactive dashboards and reports built on the same data.

## How Fabric and Azure ML Work Together

| Stage | Fabric | Azure ML |
|-------|--------|----------|
| Raw data ingestion | ✓ | |
| Data transformation | ✓ | |
| Feature engineering at scale | ✓ (Spark) | |
| Model training and tracking | | ✓ |
| Model deployment and endpoints | | ✓ |
| Batch scoring on large datasets | ✓ (can trigger Azure ML batch) | ✓ |
| BI and reporting on predictions | ✓ (Power BI) | |

![Dataset size guidance](../assets/img/msft-dataset-size-guidance.svg)

## LangChain and SynapseML for AI Workflows

**SynapseML** is an open-source library that runs on Spark and makes it easy to apply large language models at scale. It integrates directly with Azure OpenAI so you can process millions of rows of text with LLM-powered transformations in Fabric notebooks.

**LangChain** enables building multi-step reasoning chains that connect prompts, tools, and LLM calls. Combined with Azure OpenAI in Fabric, it powers use cases like:

- Document summarization across a large document store.
- Question-answering over a PDF library.
- Automated report generation from structured data.

## How to Connect Azure OpenAI in Fabric

```python
import os
from langchain_openai import AzureChatOpenAI

os.environ["OPENAI_API_VERSION"] = "2024-02-01"
os.environ["AZURE_OPENAI_ENDPOINT"] = "https://your-resource.openai.azure.com"
os.environ["AZURE_OPENAI_API_KEY"] = "your-key"

llm = AzureChatOpenAI(deployment_name="gpt-4o", temperature=0.2)
response = llm.invoke("Summarize the key risks in this report: ...")
```

![Python dtype reference](../assets/img/python_dtype.svg)

## Decision Guide: When to Use Which Platform

**Use Fabric when:**

- Your primary bottleneck is data preparation, transformation, or analytics.
- You need Spark-scale processing on very large datasets.
- You need business intelligence reports alongside your data work.

**Use Azure ML when:**

- Your primary bottleneck is model training, experimentation, or deployment.
- You need full MLOps features: versioning, lineage, staged deployment, and monitoring.
- You need online endpoints with latency SLAs.

**Use both when:**

- Data preparation happens at Fabric scale, and trained models are deployed as Azure ML endpoints.
- The Fabric Data Science experience is used for initial exploration, and Azure ML is used for production-grade training and deployment.
