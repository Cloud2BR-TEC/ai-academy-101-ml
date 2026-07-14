# Comandos CLI (Español)

Guía práctica de comandos usados en Machine Learning Fundamentals.

## Cómo leer ejemplos

- Valores como `<sub-id>` o `<run-id>` son placeholders.
- Ejecuta un comando a la vez.
- Si falla, revisa el error y los logs.

## Setup de entorno (conda + pip)

```console
conda env create --name aml-env --file environment.yml
conda activate aml-env
pip install -r requirements.txt
```

- `conda env create`: crea un entorno aislado.
- `conda activate`: activa ese entorno.
- `pip install -r`: instala dependencias.

Validación:

```console
conda env list
python --versión
pip show scikit-learn
python -m pip install ...
python -m ipykernel install --user --name aml-env --display-name "AML Env"
```

## Azure ML CLI (v2)

```bash
az login
az account set --subscription "<sub-id>"
az configure --defaults group=<rg> workspace=<ws>

az ml data create --name fraud-train --versión 1 --path ./data --type uri_folder
az ml environment create --name fraud-infer --versión 2 --file env.yml

az ml job create --file job.yml
az ml job list --query "[].{name:name,status:status}" -o table
az ml job stream --name <run-id>

az ml model create --name fraud-model --versión 3 --path ./model --type mlflow_model
az ml model list --name fraud-model -o table
```

## Despliegue (punto de conexión en línea administrado)

```bash
az ml online-endpoint create --name fraud-endpoint
az ml online-deployment create --file deployment.yml --all-traffic

az ml online-endpoint update --name fraud-endpoint --traffic "blue=90 green=10"

az ml online-endpoint invoke --name fraud-endpoint --request-file sample.json
az ml online-deployment get-logs --name green --endpoint-name fraud-endpoint
```

## Kubernetes (depuración básica)

```bash
kubectl versión --client
kubectl get pods -n <namespace>
kubectl describe pod <pod-name> -n <namespace>
kubectl logs <pod-name> -n <namespace>
kubectl logs <pod-name> -n <namespace> --previous
kubectl get events --sort-by=.lastTimestamp
kubectl get svc
kubectl get endpoints <service-name>
kubectl port-forward svc/<service-name> 8080:80
```

Local:

```bash
kind create cluster
minikube start
```
