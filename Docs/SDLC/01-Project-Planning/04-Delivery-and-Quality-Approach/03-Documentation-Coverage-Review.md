## Documentation coverage review

Comparison of the supplied lifecycle outline with the Azaraeen documentation. This review describes documentation coverage, not completed engineering work.

| Phase | Preserved or merged | Added to address gaps | Applicability boundaries |
|---|---|---|---|
| Planning | Purpose/objectives cover charter intent; scope/deliverables, roles, resources, risks and communication already have primary sources. | Feasibility assessment and work breakdown/dependencies. | No invented sponsor authority, ROI target, budget or personal schedule. Gantt charts, deadlines and sprint commitments remain outside the agreed planning scope. |
| Requirements | Business needs link to planning purpose; functional/NFR specifications, acceptance and traceability remain primary sources. | Business-needs/value view and epics/user stories; traceability now includes implementation references. | Use cases remain in System Analysis and are linked from requirements; no duplicate BRD/SRS version of the same behavior. |
| System Analysis | Processes, state transitions, roles, domain relationships and external interactions already covered. | Domain glossary, data flows and current-state/gap analysis. | BPMN/DFD/UML are optional notations chosen for clarity. Integrations are the actual mail/translation needs; payment, SMS and maps are not added. |
| System Design | System/software architecture, database/data architecture, interfaces, security, integrations and infrastructure already covered. | Component/runtime detail; strengthened architecture decision record guidance. | No assumed microservices, serverless, caching, load balancers, CDN or protocol. Technical choices depend on requirements and existing-host feasibility. |
| UX/UI Design | Discovery evidence belongs in Requirements; information architecture, flows, wireframes, visual design, components, prototypes and evaluation already covered. | No duplicate research category needed. | Personas and journey maps may be used when evidence supports them; fictional personas are not treated as research. Component/visual work can evolve into a design system without requiring a separate enterprise-scale system. |
| Implementation | Frontend, backend/data, integrations, coding conventions, migrations/file handling and handoff already covered. | Local setup/tooling and shared-code/reuse guidance. | Documentation stays here; source code, migrations, tests and runnable configuration belong in the application/tooling locations selected during implementation. Docker/SDKs are not presumed necessary. |
| Testing | Strategy/results, scenarios, design QA, UAT, security/privacy and quality checks already covered. | Explicit unit/integration/system-E2E boundaries and risk-based load-test guidance. | Test levels can share a category without duplicate folders. No penetration test, compliance certification or numeric target is claimed by an outline. |
| Deployment | Environment configuration, release, migrations, backup/rollback and production checks already covered. | Build/test/release automation decision topic. | CI/CD is evaluated for usefulness; IaC, containers and zero-downtime releases are conditional on actual infrastructure needs and support. |
| Maintenance | Monitoring/incidents/recovery, defects, dependency updates and feedback already covered. | Technical-debt/refactoring topic and maintained owner documentation. | No mandatory Grafana, on-call rotation, support staffing or personal work schedule. Backups need operational verification, not merely a design document. |

## Source-of-truth rules

- Project-wide scope and risk decisions: Planning; detailed behavior/quality expectations: Requirements.
- Required behavior models: Analysis; technical mechanisms: System Design; interface specifications: UX/UI.
- Handoff in Implementation indexes original design artifacts; it does not become an extra lifecycle phase.
- Prototype evaluations remain in UX/UI. Verification of implemented software and acceptance evidence remain in Testing.
- Backup design: System Design; release recovery procedures: Deployment; recurring operational evidence: Maintenance.
- Unknown costs, providers, technologies and quality targets remain explicit open decisions. A file or folder does not mean that the work is complete.
