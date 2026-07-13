# 07. Terraform Foundations

Terraform is a tool to create cloud resources from code files.

![Infrastructure tools](../assets/img/ml-infrastructure-tools-for-production.svg)

## Definition

Instead of clicking many buttons in the portal:

- You write desired resources in files.
- Terraform creates them consistently.

## Why This Matters

- Repeatable setup.
- Easier teamwork.
- Fewer manual mistakes.

![Deployment flow](../assets/img/ml_deployment_flow.svg)

## Four Commands You Need First

- `terraform init`: prepare project.
- `terraform plan`: preview changes.
- `terraform apply`: create/update resources.
- `terraform destroy`: clean up resources.

```mermaid
graph TD
    A[init] --> B[plan]
    B --> C[apply]
    C --> D[validate]
    D --> E[destroy when done]
```

## Core Vocabulary

- Provider: plugin to talk to Azure.
- State: record of managed resources.
- Variable: reusable input value.
- Output: values shown after deployment.

## Practical Warning

Cloud resources cost money. Use `destroy` after practice labs.
