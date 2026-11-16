## Documentation structure

Phase -> primary category -> named topic document. Category folders have no README files. This tree records the current documentation organization; outlines do not imply completed work.

```text
SDLC/
|-- 01-Project-Planning/
|   |-- 01-Project-Definition/
|   |   |-- 01-Project-Plan.md
|   |   |-- 02-Purpose-and-Objectives.md
|   |-- 02-Scope-and-Deliverables/
|   |   |-- 01-MVP-Scope-and-Deliverables.md
|   |   |-- 02-Work-Breakdown-and-Dependencies.md
|   |-- 03-Governance-and-Collaboration/
|   |   |-- 01-Roles-Changes-and-Communication.md
|   |-- 04-Delivery-and-Quality-Approach/
|   |   |-- 01-Lifecycle-Dependencies-and-Quality.md
|   |   |-- 02-Documentation-Structure.md
|   |   |-- 03-Documentation-Coverage-Review.md
|   |   |-- 04-SDLC-Documentation-Guide.md
|   |-- 05-Resources-and-Cost-Considerations/
|   |   |-- 01-Resources-and-Costs.md
|   |-- 06-Risks-and-Constraints/
|   |   |-- 01-Project-Risks-and-Constraints.md
|   |-- 07-Feasibility/
|   |   |-- 01-Technical-Operational-and-Cost-Feasibility.md
|-- 02-Requirements/
|   |-- 01-Discovery/
|   |   |-- 01-Discovery-and-Research.md
|   |   |-- 02-Stakeholders-and-Users.md
|   |   |-- 03-Business-Needs-and-Value.md
|   |-- 02-Requirement-Specification/
|   |   |-- 01-Functional-Requirements.md
|   |   |-- 02-Non-Functional-Requirements.md
|   |   |-- 03-Epics-and-User-Stories.md
|   |-- 03-Scope-and-Constraints/
|   |   |-- 01-Constraints-Assumptions-Risks.md
|   |   |-- 02-Prioritization-and-Scope.md
|   |-- 04-Acceptance-and-Traceability/
|   |   |-- 01-Acceptance-Criteria-and-Traceability.md
|-- 03-System-Analysis/
|   |-- 01-System-Context/
|   |   |-- 01-System-Overview-and-Context.md
|   |   |-- 02-Current-State-and-Gaps.md
|   |-- 02-Behavior-and-Processes/
|   |   |-- 01-Processes-and-User-Scenarios.md
|   |   |-- 02-Use-Cases-and-Roles.md
|   |   |-- 03-Business-Rules-and-State-Transitions.md
|   |   |-- 04-Validation-and-Error-Handling.md
|   |-- 03-Domain-and-Data/
|   |   |-- 01-Data-and-Relationships.md
|   |   |-- 02-Domain-Glossary.md
|   |   |-- 03-Data-Flows.md
|   |-- 04-System-Interactions/
|   |   |-- 01-Reports-Notifications-and-Integrations.md
|-- 04-System-Design/
|   |-- 01-Architecture/
|   |   |-- 01-System-Architecture.md
|   |   |-- 02-Software-Architecture.md
|   |   |-- 03-Architecture-Decisions.md
|   |   |-- 04-Component-and-Runtime-Design.md
|   |-- 02-Technology/
|   |   |-- 01-Technology-Stack-and-Paradigms.md
|   |-- 03-Data-Design/
|   |   |-- 01-Database-and-Data-Architecture.md
|   |   |-- 02-File-Storage-and-Versioning.md
|   |-- 04-Interfaces-and-Integrations/
|   |   |-- 01-API-and-Interfaces.md
|   |   |-- 02-Email-and-Translation-Integrations.md
|   |-- 05-Security/
|   |   |-- 01-Security-Design.md
|   |   |-- 02-Privacy-and-Data-Protection.md
|   |-- 06-Infrastructure/
|   |   |-- 01-Hosting-and-Observability.md
|   |   |-- 02-Backup-and-Recovery-Design.md
|-- 05-UX-UI-Design/
|   |-- 01-Structure-and-Interaction/
|   |   |-- 01-Information-Architecture.md
|   |   |-- 02-User-Flows.md
|   |-- 02-Interface-Design/
|   |   |-- 01-Wireframes.md
|   |   |-- 02-Visual-Design.md
|   |   |-- 03-Components-and-Interaction-States.md
|   |-- 03-Prototyping-and-Evaluation/
|   |   |-- 01-Prototypes-and-Usability-Evaluation.md
|   |-- 04-Content-and-Accessibility/
|   |   |-- 01-Bilingual-Content-and-Accessibility.md
|-- 06-Implementation/
|   |-- 01-Design-and-Development-Collaboration/
|   |   |-- 01-Design-Handoff.md
|   |   |-- 02-Development-Collaboration.md
|   |-- 02-Engineering-Practices/
|   |   |-- 01-Coding-Standards-and-Patterns.md
|   |   |-- 02-Local-Development-and-Tooling.md
|   |   |-- 03-Shared-Code-and-Reuse.md
|   |-- 03-Frontend/
|   |   |-- 01-Public-and-Protected-Interfaces.md
|   |   |-- 02-Owner-Administration.md
|   |-- 04-Backend-and-Data/
|   |   |-- 01-Application-Logic-and-Authorization.md
|   |   |-- 02-Persistence-Migrations-and-Files.md
|   |-- 05-Integrations/
|   |   |-- 01-Mail-and-Translation-Implementation.md
|-- 07-Testing/
|   |-- 01-Verification/
|   |   |-- 01-Test-Plan-and-Results.md
|   |   |-- 02-Unit-Integration-and-System-Tests.md
|   |-- 02-Experience-and-Acceptance/
|   |   |-- 01-Design-QA.md
|   |   |-- 02-User-Acceptance.md
|   |-- 03-Security-and-Privacy/
|   |   |-- 01-Access-and-Data-Protection-Tests.md
|   |-- 04-Accessibility-Compatibility-and-Performance/
|   |   |-- 01-Quality-Attribute-Tests.md
|-- 08-Deployment/
|   |-- 01-Release-Management/
|   |   |-- 01-Release-and-Launch.md
|   |   |-- 02-Build-Test-and-Release-Automation.md
|   |-- 02-Environment-and-Configuration/
|   |   |-- 01-Hosting-Domain-and-Secrets.md
|   |-- 03-Data-and-Recovery/
|   |   |-- 01-Migrations-Backup-and-Rollback.md
|   |-- 04-Production-Verification-and-Guidance/
|   |   |-- 01-Smoke-Checks-and-Owner-Guide.md
|-- 09-Maintenance/
|   |-- 01-Operations/
|   |   |-- 01-Operations-and-Maintenance.md
|   |   |-- 02-Monitoring-Incidents-and-Recovery.md
|   |-- 02-Continuous-Improvement/
|   |   |-- 01-Post-Launch-Evaluation.md
|   |-- 03-Updates-and-Defect-Management/
|   |   |-- 01-Fixes-Dependencies-and-Releases.md
|   |   |-- 02-Technical-Debt-and-Refactoring.md
|   |-- 04-Owner-Documentation/
|   |   |-- 01-Owner-Guide-and-Troubleshooting.md
```
