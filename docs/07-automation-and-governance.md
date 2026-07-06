# Automation and Governance

Automation is the operational backbone of the platform, with governance enforced through code and rulesets.

## GitHub Actions as the control plane

- Reusable workflows codify build, deploy, and verification paths
- Custom actions encapsulate recurring platform logic
- Infrastructure provisioning and security testing are automatically triggered from repository events

## IssueOps and AI

- GitHub Issues are used as an interface for infrastructure requests
- IssueOps workflows validate, route, and execute approved operations
- GitHub Copilot support accelerates workflow and pipeline authoring

## Policy as Code

- Rules are stored in version control and reviewed like application code
- Enterprise rulesets apply non-overridable controls for compliance
- Policy checks execute continuously across repositories

## Diagram: automation and governance flow

Source: [docs/diagrams/automation-governance-flow.mmd](diagrams/automation-governance-flow.mmd) (keep this snippet in sync with the source).

```mermaid
    A[Developer Push or Issue Request] --> B[GitHub Actions Workflow]
    B --> C[Provisioning and Delivery Automation]
    B --> D[Security and Compliance Checks]
    D --> E[Policy as Code Decision]
    E -->|Pass| F[Deploy via GitOps]
    E -->|Fail| G[Block and Report]
    H[Copilot Assistance] --> B
```
