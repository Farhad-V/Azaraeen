# Diagram Catalog

## Access request and publication requirements

```mermaid
flowchart LR
  Visitor --> Composer[Prepared email composer]
  Composer --> Receipt[Receive request and acknowledge]
  Receipt --> Approval[Owner approval]
  Approval --> Delivery[Deliver access link and password]
```

This proposed flow maps to FR-10 and FR-11. Verify receipt and delivery feasibility before selecting a provider.
