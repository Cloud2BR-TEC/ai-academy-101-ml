# 04. Assets and Lifecycle

In Azure ML, "assets" are the important pieces you save and reuse.

![ML math pipeline](../assets/img/ml-math-pipeline.svg)

## Core Assets Explained Simply

- Data asset: where your input data lives.
- Environment: package list and runtime setup.
- Job: a run that executes code.
- Model: trained result.
- Endpoint: deployed API for predictions.

![Logic implementation schema](../assets/img/logic_schema_model_implementation.svg)

## Why Asset Tracking Matters

Without tracking, you cannot answer:

- Which dataset trained this model?
- Which code version produced this result?
- Which dependency version was used?

![Training testing flow](../assets/img/training_testing_data_flow.svg)

## Lifecycle View

```mermaid
graph TD
    D[Data] --> J[Job]
    E[Environment] --> J
    J --> M[Model]
    M --> EP[Endpoint]
    EP --> MON[Monitoring]
```

## Practical Analogy

Imagine baking:

- Data = ingredients.
- Environment = kitchen setup.
- Job = cooking session.
- Model = final cake.
- Endpoint = serving counter where people request slices.

## Visual Summary

![Model implementation](../assets/img/ml_workflow_stages.svg)
