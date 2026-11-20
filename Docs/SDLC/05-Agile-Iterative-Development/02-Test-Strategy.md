# Test Strategy

Plan verification against the acceptance criteria for each increment and record results with the tested version and environment.


## Test plan and results

## Purpose and activities

Plan risk-based verification of functional and quality requirements, including protected files, expiry/renewal, archived resumes, visits, email and bilingual publication.

## Expected outputs

Traceable scenarios, execution results, defects and retest evidence. Test planning can start before implementation is complete.

## Working material

Outline only. Detailed decisions and evidence remain to be added when this activity is performed.


## Unit, integration and system tests

## Work topics

Select risk-appropriate isolated, component-interaction and full-system scenarios.

## Expected artifacts

Cases and evidence for access validity, private files, archive integrity, correct resume versions, publication and mail behavior. Avoid duplicating cases already indexed in the test plan.

## Current material

Topic outline. Decisions, implementation and verification evidence will be added as the work is performed.


## Test levels

- Unit: isolated business rules and calculations.
- Integration: collaborating database, file, authorization and provider components.
- System/end-to-end: realistic owner and visitor journeys through the delivered application.

Link each scenario to its requirement and acceptance criterion. Keep actual test code with the application/test suite, not inside documentation folders. Record execution environment, result, defects and retest evidence when run.


## Design QA

## Purpose and activities

Compare implemented interfaces and interactions against reviewed design sources, including responsive layouts, keyboard use, bilingual presentation and feedback states.

## Expected outputs

Design discrepancies, linked fixes and verification outcomes. Original design specifications remain in their source documents.

## Working material

Outline only. Detailed decisions and evidence remain to be added when this activity is performed.


## User acceptance

## Purpose and activities

Verify owner and visitor journeys against agreed acceptance criteria. Record the evaluator, scope and limits of evaluation; owner acceptance alone does not prove usability for all recruiters.

## Expected outputs

Acceptance outcomes, unresolved issues and links to requirements and evidence.

## Working material

Outline only. Detailed decisions and evidence remain to be added when this activity is performed.


## Access and data protection tests

## Work topics

Verify unauthorized private-page/file access is denied, expiry affects active sessions, revocation works and the archive stays owner-only.

## Expected artifacts

Security regression evidence, defects and fixes; check logs and external integrations for unintended sensitive-data exposure.

## Current material

Topic outline. Decisions, implementation and verification evidence will be added as the work is performed.


## Quality attribute tests

## Work topics

Check agreed accessibility, browser/device compatibility, bilingual rendering and performance expectations.

## Expected artifacts

Environment coverage, measurements against approved targets and unresolved issues. Targets are pending; no arbitrary numeric thresholds are imposed.

## Current material

Topic outline. Decisions, implementation and verification evidence will be added as the work is performed.


## Performance and load

Select representative content sizes and concurrency based on expected use and hosting limits. Record actual measurements, capacity concerns and agreed thresholds. Stress testing or large synthetic loads are not mandatory without a concrete risk and an appropriate test environment.
