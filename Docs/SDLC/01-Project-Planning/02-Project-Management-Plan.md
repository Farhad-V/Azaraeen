# Project Management Plan

Use these documents to plan delivery, review dependencies and coordinate changes.


## Work breakdown and dependencies

## Purpose

Break agreed deliverables into reviewable work packages: planning, requirements, analysis, technical/UX design, portfolio/admin/application implementation, verification and release.

## Topics and outputs

Link each package to the relevant source document, intended output and prerequisite decisions. Add detail as work becomes clear; do not invent durations, owners or commitments.

## Boundaries

This is an output/dependency breakdown, not a personal schedule, Gantt chart or fixed sprint plan.

Detailed artifacts and evidence are pending unless explicitly stated above. This outline does not establish a completed assessment or implementation.


## 5. Stakeholders and decision-making

| Stakeholder | Role and responsibilities |
|---|---|
| Samira | Portfolio owner and primary project contributor across the development lifecycle; decides product scope, content publication and visitor access. |
| Farhad | Collaborates with Samira on project delivery. |
| Employers, recruiters and other approved visitors | Use the professional portfolio and authorized content. |

The private application archive serves Samira. Proposed scope changes are presented for Samira's decision. Detailed work allocation between Samira and Farhad remains flexible.

## 12. Change and configuration management

Record proposed changes and effects on scope and dependencies for Samira's decision. Keep code and documentation in Git. Use the previously discussed GitHub Issues/Kanban approach with acceptance criteria: Ready, In Progress, Review & Testing, Done.

Use patch/minor/major release distinctions and a changelog as discussed. A detailed branching policy is not selected.

## 13. Communication

Review concrete decisions and unresolved issues in project discussions, in Persian with useful English terminology. Reuse established decisions and ask only about specific gaps.

No recurring meeting cadence, daily reporting obligation or personal work schedule is imposed.


## 6. SDLC approach

Use iterative delivery with requirements, analysis, design, implementation and verification in manageable increments. Documentation follows the product; security and privacy apply throughout.

The seven phases are the documentation structure chosen for Azaraeen, not a universal or mandatory SDLC standard. They are not mutually exclusive time blocks. Research and requirements analysis inform the early phases; UX/UI and technical design inform each other; evaluation and design/development collaboration continue through delivery. Each artifact has one primary location, with links from related phases. See the SDLC guide. UX/UI flows reference the original requirements and process analysis; implementation guidance is maintained in the handoff index.

### Phase deliverables and readiness criteria

This table defines expected outputs for each phase and where the primary artifacts are maintained. A linked outline is not evidence of completion. Assess readiness for the selected increment, record unresolved issues and revisit earlier work when needed; these criteria do not impose a calendar or automatic approval gate.

| Phase | Expected deliverables | Readiness criteria | Primary artifacts |
|---|---|---|---|
| 01 Project Planning | Purpose/objectives, agreed MVP scope and exclusions, responsibilities, resources, feasibility findings, risks and delivery dependencies. | The selected work has clear value and boundaries; known constraints and decisions needing investigation are visible. Hosting suitability is assessed before dependent technology choices. | Project plan; scope; feasibility; risks. |
| 02 Requirements Engineering | User/business needs, identified functional and quality requirements, scope priorities, acceptance criteria and traceability. | For the selected increment, required behavior and important exceptions are testable; relevant quality criteria and unresolved decisions are explicit; acceptance criteria link to requirements. | Functional requirements; quality requirements; acceptance and traceability. |
| 03 System Analysis | System context, use cases/process models, domain/data relationships, business rules, state transitions, data flows and exception scenarios. | Selected journeys explain actors, information, state changes and alternate outcomes consistently. Contradictions and blocking gaps are resolved or recorded for decision before dependent work proceeds. | Context; processes; state rules; data relationships. |
| 04 System Design | System/software architecture, justified technology choices, component/interface contracts, database/file design, security/privacy mechanisms, integrations and infrastructure/recovery design. | The selected behavior has an implementable technical design aligned with requirements and hosting evidence. Critical authorization, version preservation and failure/recovery paths are addressed; unresolved technical risks are explicit. | System architecture; software architecture; database; security; integrations. |
| 04 System Design — UI/UX | Information architecture, interaction flows, wireframes, responsive visual/component specifications, bilingual/accessibility guidance, prototypes and evaluation findings. | Selected owner/visitor tasks and relevant empty, loading, validation, error and success states are reviewable. Designs are sufficiently clear to implement; material usability issues and evaluation limitations are addressed or documented. | User flows; visual design; components; prototypes/evaluation. |
| 05 Agile Iterative Development — Implementation | Working frontend/backend/data changes and integrations, implementation decisions, reproducible local setup and relevant developer-check evidence. | Selected behavior runs in the development/test environment, implements the reviewed access/validation rules, and passes relevant developer checks. Code review findings and deviations from design/requirements are addressed or explicitly tracked. | Source code in the Application/Frontend and Application/Backend directories as the stack evolves; collaboration notes; local setup; data implementation. |
| Agile Iterative Development — Testing | Risk-based test plan/cases, execution results, defect/retest records, security and quality evidence, design QA and user acceptance outcomes. | Evidence identifies the tested version/environment and links to selected acceptance criteria. Blocking failures are resolved; residual defects, coverage limits and acceptance decisions are visible before release. | Test plan/results; security checks; quality checks; acceptance. |
| 06 Deployment and Release | Versioned release, environment/configuration instructions, migration and recovery procedures, production smoke-check results and initial owner guidance. | Target configuration and recovery steps are prepared; the deployed version passes critical production checks for access, private files, correct resumes and mail. Material release failures are resolved or explicitly block the release. | Release; environment; rollback/recovery; production checks. |
| 07 Maintenance and Evolution | Operational/incident records, recovery verification, verified fixes and dependency updates, technical-debt items, maintained owner guidance and improvement findings. | Each maintenance change has appropriate regression evidence and updated guidance before release. Operational findings have recorded outcomes/follow-up decisions. Maintenance is continuous, not a phase declared permanently finished. | Operations/recovery; fixes/updates; evaluation; owner guidance. |

The detailed phase descriptions below explain the work; the table above is the central deliverable/readiness reference. Actual decisions, designs, code and evidence remain in their primary locations and are linked rather than copied here.

### 6.1. Project Planning — purpose, boundaries and approach

Planning establishes the basis for product decisions: the problem, audience, expected value, scope, resources and dependencies. It also identifies what is unknown and what must be investigated later. For Azaraeen, this includes agreeing that the first release contains both the portfolio and the private application archive, and assessing the existing hosting before selecting technology. Personal scheduling remains outside the agreed planning scope.

### 6.2. Requirements — required capabilities and rules

Functional requirements describe capabilities such as creating an application draft, generating access credentials and uploading an advertisement PDF. Nonfunctional requirements describe qualities such as protected file access, accessibility, performance and reliability; concrete targets still need to be established where relevant.

Each selected requirement should identify the actor, trigger, expected result, applicable rules and acceptance criteria. For example: after entering company and position, Samira can generate and copy access credentials without uploading files or marking the application submitted. Another rule is that an expired credential must not permit further protected requests. These statements define observable behavior that can later be verified.

### 6.3. System Analysis — behavior, processes and information

Analysis connects the individual requirements into a coherent system. Examine what starts each process, which states it passes through, what information is needed, which exceptions can occur and how the process affects other parts of the product. Models can include use cases, activity diagrams, state diagrams and conceptual data relationships.

For example, analyze an access lifecycle from creation through use, expiry, renewal and revocation. Analyze the relationship between a company, its job applications, submitted documents, credentials and visits. Check what happens when access exists before its application-specific resume is uploaded. For email requests, distinguish opening the email composer from receiving the message, acknowledging receipt, owner approval and credential delivery. The output explains required behavior and dependencies; detailed technology choices follow in System Design.

### 6.4. System Design — technical structure and mechanisms

Translate the analyzed behavior into implementable technical decisions. Define component responsibilities, database structures, internal and external interfaces, file delivery, session and credential handling, email integration and deployment configuration. Evaluate relevant alternatives against the existing hosting and the agreed requirements.

For example, specify how every protected file request checks access validity, how archived resume versions remain associated with the correct application, and how approval initiates reliable email delivery. Record important decisions and tradeoffs. The implementation stack is selected through this work rather than assumed by this plan.

### 6.5. UX/UI Design — user experience and interface

Use the reviewed requirements and analysis to shape how visitors and the owner understand and operate the product. Design information architecture, navigation, task flows, field order, feedback and accessible interactions. Progress from wireframes to interactive prototypes and visual design in Figma, refining them through review and usability feedback.

For example, show how a visitor moves from the public introduction to password entry and protected work without repeated prompts. Design the expired-access message and request-access action. In the owner panel, make credential creation available early in an application draft and keep the previous-company notification informative and nonblocking. Include bilingual content, different screen sizes and relevant interface states.

### 6.6. Implementation — building working behavior

Develop the frontend, backend, database changes and integrations according to the reviewed designs. Implement validation, authorization, publication rules and error handling together with the feature. Review changes and run relevant developer checks as increments are built.

For example, implement the application draft form, credential generation and copy actions, archived file association and expiry enforcement. Keep related requirements and documentation aligned with approved changes discovered during development.

### 6.7. Testing — evidence that the product meets its requirements

Select tests according to behavior and risk: unit tests for isolated logic, integration tests for collaborating components, end-to-end tests for key journeys and owner acceptance checks for intended use. Include security/access checks, bilingual behavior, accessibility and performance checks against agreed criteria. Test design can begin with requirements and does not wait until implementation ends.

For example, verify that credentials can be generated before applying, refresh does not inflate visit counts, renewal preserves history, private files cannot be fetched without valid access and each application receives its archived resume. Verify that untranslated German sections use English and unapproved edits remain unpublished. Record defects, fix them and retest affected behavior.

### 6.8. Deployment — releasing and verifying operation

Prepare environment-specific configuration, domain/HTTPS setup, database changes, private storage permissions, mail configuration and secrets handling. Define backup and rollback/restoration steps before releasing. Verify the application in its production environment rather than relying only on local results.

For example, check the public page, protected-file denial, visitor login, correct resume delivery and mail delivery on the selected hosting. Provide owner instructions for routine administration and recovery. Deployment is complete when the release operates as intended and material release issues have been resolved or explicitly recorded.

### 6.9. Maintenance — sustaining and improving the product

After release, review operational errors and owner feedback, correct defects, update dependencies and maintain recoverable data. Revisit requirements when needs change and route proposed additions through scope review. Maintenance may produce a small patch or feed a later feature iteration.

For example, investigate failed access emails, verify recovery from backups, address a file-access defect or improve a confusing interaction. Record and verify changes before release. No support schedule or response-time commitment is established here.

These checkpoints describe expected outputs rather than completed work or mandatory approval gates. Requirements, analysis and design can be revisited as evidence changes.

## 7. Delivery sequence and dependencies

For the current project, establish the planning, requirements and analysis baseline before detailed Figma work. Technical and UX/UI design then inform each other; architecture does not have to be frozen before interaction design. Technology selection depends on hosting assessment. Email automation depends on a defined receipt, approval and delivery mechanism. Correct application-specific resume delivery depends on its archived version being available.

Personal daily tasks, time allocation, start/end dates, deadlines, sprint lengths and calendar milestones are outside this planning session. No schedule or time commitment is assigned.

## 11. Quality and verification

Acceptance criteria will cover visitor/owner journeys, private-file protection, expiry/renewal, session-based counts, archive integrity, correct resume selection and bilingual publication/fallback.

Use code review and tests appropriate to the implementation, including integration and end-to-end checks for important behavior. Performance/accessibility targets and test tooling remain to be defined.

Definition of Done: the selected behavior is usable, relevant checks pass and related documentation is current. This is a quality approach, not evidence that features have passed.

## 14. Deployment, guidance and support

Assess deployment on the existing hosting during system design. Define release verification, backup/restoration and rollback before production release. Prepare owner guidance for publication, access administration and application archiving.

Maintenance includes defect correction and necessary updates. No support staffing, response-time commitment or SLA has been agreed.


## 8. Cost considerations

The domain and hosting are already paid resources and form the baseline. No budget, person-hour estimate or contingency amount is specified. Additional services require an identified need and a separate decision; no purchase is implied.

Automatic translation may incur costs. Manual approval does not make translation free; provider and pricing remain undecided. Manual translation remains available.

## 9. Resources and environments

- Existing domain: azaraeen.de.
- Existing hosting: Hetzner Level 1. The supplied panel shows 10 GB storage and capacity for one database; runtime and automation suitability remain unverified.
- Local workspace: C:\xampp\htdocs\PROJECT\Azaraeen, with Frontend, Backend and Docs directories.
- Git/GitHub for source and documentation, Markdown for documents, and Figma for later design work.
- The reviewed multi-resume application and Kay Kazemi website provide ideas; no stack selection or permission to reuse third-party code is inferred.

Production architecture, test environment, translation provider and mail integration remain undecided.


## Milestones

Milestones are reviewable outcomes, without personal schedules or calendar commitments. Their definitions are the phase deliverables/readiness criteria in the lifecycle plan.

Use that source to evaluate planning, requirements, analysis, technical/UX design, implementation, verification and release readiness for selected increments. Documentation outlines alone do not establish milestone completion. Maintenance remains ongoing rather than a final completed milestone.

No dated milestone plan or completed milestone register has been agreed.
