# System Analysis

Review the system context, user scenarios, business rules and domain data.


## System overview and context

## Purpose

Define the system boundary, actors and external dependencies for Azaraeen. This document describes the required system context; technical architecture is maintained in System Design.

## System boundary

Azaraeen provides public professional content, protected portfolio and resume access, owner content/publication controls, access administration and a private job-application archive. Saving an application record does not submit an application to an employer.

## Actors and external systems

- Samira operates the private administration and makes publication/access decisions.
- Public visitors view introductory content and may initiate an email access request.
- Approved visitors use application-specific or direct-request access.
- The visitor's email application composes and sends requests; the website cannot infer message receipt from a click.
- Mail services support receipt acknowledgement and approved credential delivery; the mechanism remains unresolved.
- Existing hosting provides the intended production environment, subject to compatibility assessment.
- A translation service is optional and undecided; translations require owner approval.

Job portals and employer systems are external. Application details and correspondence are manually archived in MVP. GitHub and LinkedIn are outbound profile links, not authenticated integrations.

## Related sources

- Functional requirements
- Stakeholders and users
- Processes and scenarios

Detailed context diagrams remain to be developed.


## Current state and gaps

## Purpose

Compare evidence of the current project against the intended MVP.

## Topics and outputs

Record that domain/hosting and documentation exist; do not infer implemented portfolio features from document outlines or the reference application. Identify gaps in host compatibility, mail handling, resume availability and unverified workflows. Link evidence and resulting work items.

## Boundaries

Update using actual repository/runtime evidence. This is not a claim that the referenced third-party application is the product baseline.

Detailed artifacts and evidence are pending unless explicitly stated above. This outline does not establish a completed assessment or implementation.


## Processes and user scenarios

## Purpose and activities

Analyze public discovery, password entry, access requests, approval and delivery, application archiving and publication. Examine alternate and exceptional paths.

## Expected outputs

Process models and scenarios, including access before an application-specific resume has been uploaded.

## Working material

Outline only. The sections above describe intended work; completed artifacts, decisions and verification evidence have not yet been added.


## Use cases and roles

## Purpose

Identify actor goals, preconditions, normal paths and exceptions. User categories describe interaction contexts; they do not introduce additional permission tiers.

| Actor | Use cases |
|---|---|
| Public visitor | View published public content; compose an access request by email. |
| Approved visitor | Enter valid credentials once; view protected published content; download the assigned resume; request renewed access after expiry. |
| Samira | Manage and publish content; review translations; create/revoke/renew access; approve direct requests; manage and search application records and their history. |

All approved visitor access opens the published protected content, with application-specific resume selection. Private application records remain owner-only. Optional contact details do not prove who used credentials. Farhad's collaboration on project delivery does not by itself define a production account or permission role.

## Detailed use-case template

For each selected use case, record: actor, goal, trigger, preconditions, main flow, alternate/error flows, resulting state and linked requirement identifiers. Derive behavior from Functional Requirements; link process diagrams from Processes and User Scenarios.

Detailed use-case specifications remain to be written.


## Business rules and state transitions

## Purpose and activities

Model access creation, expiry, renewal and revocation; application states; content drafts, publication and translation approval.

## Expected outputs

State transitions, prerequisites, exceptions and consistency rules linked to requirements.

## Working material

Outline only. The sections above describe intended work; completed artifacts, decisions and verification evidence have not yet been added.


## Data and relationships

## Purpose and activities

Analyze companies, job applications, optional contacts, submitted versions, files, access credentials, visits and bilingual content.

## Expected outputs

Conceptual entities, relationships, ownership and historical preservation rules; database implementation belongs in System Design.

## Working material

Outline only. The sections above describe intended work; completed artifacts, decisions and verification evidence have not yet been added.


## Data flows

## Purpose

Model how profile content, application documents, access credentials, email requests and visit records enter, move through and leave the system.

## Topics and outputs

Use a context/data-flow view where it clarifies processing, stores, external actors and sensitive information boundaries. Include private file delivery and provider exchanges.

## Boundaries

Data-flow models explain information movement; process/activity models explain behavior. Avoid duplicate diagrams with no distinct purpose; notation can be lightweight.

Detailed artifacts and evidence are pending unless explicitly stated above. This outline does not establish a completed assessment or implementation.


## Reports, notifications and integrations

## Agreed reporting and feedback

- Show opened/not opened and session-based visit counts for each access; no page/download tracking or verified-person attribution.
- Search application history by company, job title and optional contact.
- When creating an application for a company with history, show nonblocking information linking to prior records. This is not a warning or confirmation gate.
- Show a clear expired-access message and a route to request renewed access.
- Optional follow-up information stays within its application record; there is no separate upcoming-task dashboard.

## Email flow

1. Request Access opens the visitor's composer with recipient and subject prepared; show the email address and copy option as a fallback.
2. The visitor writes their reason and sends the email.
3. Actual receipt triggers acknowledgement that the request will be reviewed; acknowledgement is not access approval.
4. Owner approval precedes automatic delivery of the link and password.

Receipt detection, request-to-approval correlation, duplicate acknowledgement handling and delivery failure behavior remain to be analyzed. A composer link alone cannot implement receipt or delivery automation. Manual archiving of job correspondence does not remove the separate access-email automation requirement.

## Integration boundaries

Describe information exchanged, triggering events, expected outcomes and failure cases here. Provider/API/protocol choices belong in Integrations. Translation provider, cost and handling of confidential text remain open. No automatic job-portal submission or inbox import is included in MVP.

- System context
- Open requirements decisions
