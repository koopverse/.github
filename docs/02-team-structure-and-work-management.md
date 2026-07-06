# Team Structure and Work Management

Platform teams at Koopverse treat application and product squads as their primary customers.

## Customer model

- Product squads consume platform capabilities as reusable products
- Platform teams gather demand signals from delivery friction and service onboarding
- Success is measured through adoption, lead time, and reliability

## Centralised vs embedded model

- **Centralised governance** provides standards, controls, and reusable architecture
- **Golden path enablement** offers standardised templates and workflows
- **Embedded platform engineering** supports squads directly when complexity is high

## Diagram: team topology

```mermaid
flowchart LR
    A[Platform Governance Team] --> B[Golden Path Team]
    A --> C[Security and Compliance]
    B --> D[Product Squad A]
    B --> E[Product Squad B]
    F[Embedded Platform Engineer] --> D
    F --> E
```
