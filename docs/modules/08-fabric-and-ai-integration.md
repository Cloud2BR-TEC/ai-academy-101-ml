# 08. Fabric and AI Integration

This module explains when Microsoft Fabric helps your ML workflow.

![Collect data and targets](../assets/img/collect_data_init_primary_second_targets.svg)

## Operating Model

- Fabric: strong for data engineering and analytics collaboration.
- Azure ML: strong for model lifecycle and deployment.

Use both when your data work and model work need to connect smoothly.

## Integration Use Cases

- Data prepared in Fabric, model trained in Azure ML.
- Batch text enrichment with LLM workflows.
- Shared analytics + ML pipeline reporting.

![Dataset size guidance](../assets/img/msft-dataset-size-guidance.svg)

## Common Decision Point

"Which tool should I use first?"

Start where your biggest current bottleneck exists:

- Data preparation bottleneck -> begin in Fabric.
- Model training/deployment bottleneck -> begin in Azure ML.

![Python dtype reference](../assets/img/python_dtype.svg)

## Decision Checklist

- Need strong BI + collaborative analytics -> Fabric.
- Need training/deployment lifecycle control -> Azure ML.
- Need both -> integrate with clear ownership by stage.
