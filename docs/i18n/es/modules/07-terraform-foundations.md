# 07. Fundamentos de Terraform

Terraform permite crear infraestructura cloud mediante archivos de código en lugar de clicks manuales.

## Enlaces Rápidos

- Fundamentos de modelos: [Módulo 01](01-machine-learning-basics.md)
- Ciclo de Azure ML: [Módulo 02](02-azure-ml-overview.md)
- Endpoints y deploy: [Módulo 06](06-deploy-and-score.md)

Este módulo presenta primero lo esencial para principiantes.

![Herramientas de infraestructura](../assets/img/ml-infrastructure-tools-for-production.svg)

## Problema que Resuelve

Sin IaC:

- Ambientes distintos entre equipos.
- Sin historial claro de configuracion.
- Repeticion manual propensa a errores.

Con Terraform:

- Estado deseado en archivos `.tf`.
- Cambios previsibles con `plan`.
- Historial en control de versiones.

## Flujo Terraform

```mermaid
flowchart LR
    A[Write .tf files] --> B[terraform init]
    B --> C[terraform plan]
    C --> D{Review changes}
    D -->|approve| E[terraform apply]
    D -->|reject| C
    E --> F[Resources created in Azure]
    F --> G[terraform destroy when done]
```

![Flujo de despliegue](../assets/img/ml_deployment_flow.svg)

## Cuatro Comandos Clave

### `terraform init`

Inicializa providers necesarios.

### `terraform plan`

Muestra cambios antes de aplicar.

### `terraform apply`

Aplica cambios en Azure.

### `terraform destroy`

Elimina recursos administrados por Terraform.

## Vocabulario Básico

| Término | Significado |
|------|----------|
| **Provider** | Plugin para conectarse al cloud (ej. Azure). |
| **Resource** | Pieza de infraestructura (storage, workspace). |
| **State** | Archivo con recursos administrados por Terraform. |
| **Variable** | Entrada reutilizable de configuracion. |
| **Output** | Valor mostrado al finalizar `apply`. |
| **Module** | Bloque reutilizable de Terraform. |
| **Backend** | Lugar donde se guarda el state (local o remoto). |

## Estructura de Archivos

```text
src/
â”œâ”€â”€ main.tf
â”œâ”€â”€ variables.tf
â”œâ”€â”€ terraform.tfvars
â”œâ”€â”€ provider.tf
â”œâ”€â”€ outputs.tf
â””â”€â”€ remote-storage.tf
```

## Conceptos Avanzados (Opcional)

- Remote state compartido.
- Locking de estado.
- Multi-ambiente (dev/test/prod).
- Módulos reutilizables.

## Seguridad de Costos

Al terminar práctica:

1. Confirmar subscripcion/workspace correctos.
2. Ejecutar `terraform destroy -var-file terraform.tfvars`.
3. Verificar recursos eliminados.
