# Repository Landscape

Koopverse organises repositories by capability, ownership boundary, and reuse level.

## Core repository types

- Golden path starter kit repositories
- Shared module repositories (Terraform and Helm)
- Internal Developer Portal repositories
- Automation repositories for reusable workflows and actions
- Policy repositories for enterprise governance controls

## Diagram: repository landscape

Source: [docs/diagrams/repository-landscape.mmd](diagrams/repository-landscape.mmd) (keep this snippet in sync with the source).

```mermaid
    A[Golden Path Starter Kits] --> D[Product Service Repositories]
    B[Shared Terraform Modules] --> D
    C[Shared Helm Charts] --> D
    E[IDP Configuration and UI] --> D
    F[Reusable Actions and Workflows] --> D
    G[Policy as Code Repositories] --> D
```
