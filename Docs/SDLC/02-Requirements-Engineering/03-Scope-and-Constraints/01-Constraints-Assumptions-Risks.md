## Constraints, assumptions and risks

## Constraints and assumptions

- Existing azaraeen.de domain and Hetzner Level 1 hosting are the baseline, subject to technical suitability.
- Application archiving is manual in MVP; automatic handling of access-request acknowledgements and approved access delivery is a separate requirement.
- English is the default language; German translation requires owner approval.
- Personal scheduling and numerical budgets are not specified.

## Open decisions, dependencies and risks

- Validate hosting runtime/database/deployment capabilities and private file delivery.
- Define email receipt detection, acknowledgement, approval UI and reliable automatic delivery without assuming inbox synchronization.
- Translation service, cost and treatment of confidential text sent externally remain unresolved.
- Design secure credential storage and the requested copy/delivery workflow; never expose credentials in public content or logs.
- Define backup/restoration, archive deletion/retention, authentication protection and privacy notices during requirements/analysis.
- Application-specific resume availability before a file is uploaded needs explicit behavior; no unrelated resume should silently replace it.
- Clarify exact document types/limits and case-study count during content requirements; the spoken count was ambiguous.
- Expiry cannot retract content already downloaded, captured or rendered.

These are unresolved items, not implemented solutions. The project-wide risk overview remains in [Project Planning](../../01-Project-Planning/01-Project-Definition/01-Project-Plan.md); this document records their implications for requirements.
