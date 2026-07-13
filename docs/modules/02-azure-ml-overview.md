# 02. Azure ML Overview

Azure Machine Learning is the cloud workspace where you build, train, deploy, and monitor machine learning solutions.

![End-to-end workflow](../assets/img/ml-e2e-workflow.svg)

## What Azure ML Provides

- One place for your data references, code, runs, and models.
- Repeatable workflows so results are not random.
- Visual and code-based ways to build solutions.

![Azure ML taxonomy](../assets/img/azure-machine-learning-taxonomy.svg)

## End-to-End Lifecycle in Simple Words

1. Define the business question.
2. Prepare data.
3. Train model.
4. Check quality.
5. Deploy model.
6. Monitor and improve.

![Training vs deployment](../assets/img/training_vs_deployment_model.svg)

```mermaid
flowchart LR
    A[Problem] --> B[Data]
    B --> C[Train]
    C --> D[Evaluate]
    D --> E[Deploy]
    E --> F[Monitor]
    F --> C
```

## Core Terms in Azure ML

- Workspace: your main project area.
- Compute: the machines that run your jobs.
- Job: one execution (training, scoring, processing).
- Model registry: saved versions of trained models.
- Endpoint: URL for prediction requests.

![Azure ML environment taxonomy](../assets/img/azure-ml-environment-taxonomy.svg)

## Why Monitoring Exists

Real-world data changes over time.

- Model that worked in March may degrade in July.
- Monitoring catches drops in quality early.

![Score to decision](../assets/img/score-to-decision.svg)

## Visual Recap

![ML deployment flow](../assets/img/ml_deployment_flow.svg)
