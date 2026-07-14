
# Glossary

Clear definitions for key terms used in Machine Learning Fundamentals.

## Machine learning basics

- **Machine learning (ML)**: A way for computers to learn patterns from data so they can make predictions.
- **Model**: The learned pattern that takes input data and produces an output.
- **Feature**: An input value used by a model, such as age, price, or temperature.
- **Label / target**: The value you want the model to predict.
- **Training**: The process where a model learns from examples.
- **Inference**: Using a trained model to make predictions on new data.
- **Supervised learning**: Learning from labeled examples.
- **Unsupervised learning**: Finding patterns in unlabeled data.
- **Reinforcement learning**: Learning by trial and error using rewards.
- **Overfitting**: When a model memorizes training data and performs poorly on new data.
- **Underfitting**: When a model is too simple and misses important patterns.
- **Data leakage**: When future or hidden information accidentally appears in training data.

## Software and engineering concepts

- **Software**: Instructions written in code that tell a computer what to do.
- **Software engineer**: A person who designs, builds, tests, and maintains software systems.
- **Script**: A short program that automates steps, such as data cleaning or deployment.
- **API**: A defined way for one software system to request data or actions from another.
- **Endpoint**: A URL where an API receives requests and returns responses.
- **Backend**: The server-side part of a system where data processing and logic run.
- **Frontend**: The user-facing part of a system, such as a website or app screen.
- **Repository (repo)**: A folder that stores project code, files, and change history.
- **Version control**: A system that tracks file changes over time.
- **Git**: A popular version control tool.
- **Debugging**: Finding and fixing errors in code or system behavior.
- **Log**: A time-ordered record of what happened in a program or service.
- **Deployment**: Releasing software or a model so others can use it.
- **Automation**: Running repeated tasks with scripts or tools instead of manual steps.

## Azure ML platform

- **Workspace**: The main Azure ML project space where assets are organized.
- **Compute instance**: A single VM for interactive development.
- **Compute cluster**: Multiple machines that scale up/down for training jobs.
- **Environment**: A saved runtime setup (Python version + packages) for consistent execution.
- **Datastore**: A connected storage location used by Azure ML.
- **Data asset / dataset**: A versioned reference to data used in experiments.
- **Job**: One tracked execution of code in Azure ML.
- **Model registry**: A versioned store of trained models.
- **Lineage**: The trace from data to job to model to deployment.
- **RBAC**: Role-based access control that limits who can do what.

## Modeling and evaluation

- **Loss function**: A formula that measures prediction error during training.
- **Gradient descent**: A method that updates model parameters to reduce loss.
- **Hyperparameter**: A setting chosen before training, like learning rate.
- **Cross-validation**: Repeated train/validate splits for more reliable evaluation.
- **Threshold**: A cutoff used to convert prediction scores into decisions.
- **Accuracy**: Percentage of correct predictions.
- **Precision**: Of predicted positives, how many are truly positive.
- **Recall**: Of real positives, how many the model found.
- **F1 score**: A balance between precision and recall.
- **MAE / RMSE**: Common regression error measurements.

## Operations and MLOps

- **MLOps**: Practices that help teams build, deploy, monitor, and maintain ML systems.
- **Online endpoint**: Real-time prediction service.
- **Batch endpoint**: Scheduled or large-scale prediction processing.
- **Drift**: Data patterns changing over time compared with training data.
- **Canary deployment**: Sending a small amount of traffic to a new model first.
- **Blue/green deployment**: Running old and new versions side by side for safer release.
- **Readiness probe**: Check that a service is ready to receive traffic.
- **Liveness probe**: Check that a service is healthy and should keep running.
- **Model card**: A summary document with model data, metrics, limitations, and operating notes.

