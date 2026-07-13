# 01. Machine Learning Basics

Machine learning (ML) means teaching a computer to learn from examples instead of writing every rule manually.

![Overview ML flow](../assets/img/Overview_ML_flow.svg)

## Definition

- Traditional programming: you write rules, computer follows them.
- Machine learning: you show examples, computer discovers patterns.

Think of ML like teaching a child with examples:

- You show many photos of cats and dogs.
- The learner starts noticing differences.
- Later, it can guess if a new photo is a cat or a dog.

![ML workflow stages](../assets/img/ml_workflow_stages.svg)

## Key Terms

- Data: information used to learn.
- Feature: one piece of information (example: age, income, clicks).
- Label/Target: the answer we want to predict.
- Model: the learned pattern.
- Prediction: the model's answer for new data.
- Training: the learning step.
- Testing: the checking step on unseen data.

![Training test split](../assets/img/training_test_split.svg)

## Common ML Types

- Supervised learning: has correct answers in data.
- Unsupervised learning: no correct answers, model groups or finds structure.
- Reinforcement learning: learns by rewards/penalties.

![Machine learning types](../assets/img/machine_learning_types.svg)

## Everyday Examples

- Spam filtering in email.
- Recommending products or videos.
- Detecting unusual bank activity.
- Predicting sales for next month.

![Types of ML by objective](../assets/img/types_of_ml_based_in_objective.svg)

## Why Data Quality Matters

If input data is confusing, missing, or wrong, the model learns the wrong lesson.

- Good data -> better learning.
- Poor data -> poor predictions.

![Feature engineering and data collection](../assets/img/feature_engineering_collect_data.svg)

## Simple End-to-End Steps

1. Define the problem.
2. Collect and clean data.
3. Train a model.
4. Evaluate model quality.
5. Deploy and monitor.

![ML process by stages](../assets/img/ml_process_by_stages.svg)

## Applied Example

Goal: predict house price.

- Features: number of rooms, size, neighborhood.
- Target: house price.
- Model: learns relationship between features and price.
- Prediction: estimated price for a new house.

![Linear regression fit](../assets/img/linear-regression-fit.svg)
