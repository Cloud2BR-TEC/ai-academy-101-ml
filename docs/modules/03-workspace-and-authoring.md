# 03. Workspace and Authoring

Think of Azure ML workspace as your ML project home.

![Azure ML environment taxonomy](../assets/img/azure-ml-environment-taxonomy.svg)

## What Exists Inside a Workspace

- Data references.
- Compute resources.
- Experiment runs.
- Registered models.
- Endpoints for prediction.

![Azure ML taxonomy](../assets/img/azure-machine-learning-taxonomy.svg)

## Authoring Options

- Notebooks: easiest place to start learning and testing code.
- AutoML: platform tries many models for you.
- Designer: visual drag-and-drop pipelines.

![AutoML diagram](../assets/img/automl_diagram.svg)

## Recommended Starting Path

Start with notebooks because you can:

- Learn each step clearly.
- See outputs immediately.
- Fix errors quickly.

Then use AutoML to compare with your manual approach.

![AutoML process](../assets/img/automl_process_what_to_expect.svg)

## Core Vocabulary

- Experiment: a logical group of runs.
- Run: one attempt with specific settings.
- Pipeline: connected sequence of steps.
- Artifact: saved output (model, metrics, logs).

![Training data flow](../assets/img/training_testing_data_flow.svg)

## Summary

Workspace is the project container, compute is the execution engine, and jobs are the runs executed with that engine.
