# Software Requirements Specification

The functional and non-functional requirements supply the baseline for Azaraeen.


## Functional requirements

Product behavior agreed in project discussions. Identifiers support cross-references; they do not indicate implementation or acceptance status.

- **FR-01** Public introduction: configurable header, hero, profile image, short summary, GitHub/LinkedIn links, selected skills, languages, work and education summaries.
- **FR-02** Owner-controlled public/private visibility, including profile image and separate certificate title, description and file visibility. Private titles can be completely absent publicly.
- **FR-03** One visitor authentication unlocks all published protected content. No per-section passwords or per-recipient content permissions, except application-specific resume selection.
- **FR-04** Protected case studies and certificates/education documents; original private files require protection too. Only resumes have a download action; other content is presented within the site. This cannot prevent screenshots or all saving.
- **FR-05** An application-specific link and password can be created immediately after entering company and job title, while the record is still a draft, without uploads or submission dates.
- **FR-06** Application access is associated with company and position, not verified individual identity. Optional contact details do not define the record.
- **FR-07** Owner-selected expiry starting at creation, or no expiry; revocation and renewal. Expiry blocks further protected access, including existing sessions. Clear expiry message offers email-based access requests.
- **FR-08** Renewal preserves link, password and history; credential replacement is a separate explicit action.
- **FR-09** Visits show opened/not opened and session-based counts. Refresh/navigation does not add visits; no page/download tracking. Counts identify use of credentials, not the individual or proof of reading.
- **FR-10** Request Access opens the visitor's email composer with recipient and subject prepared. Always offer a visible address and copy option. Visitor writes their reason and sends the email.
- **FR-11** Acknowledgement after email receipt; owner approval precedes automatic delivery of access link/password. Mail receipt and approval integration require technical analysis; a composer link alone cannot implement these steps.
- **FR-12** Private application archive included in MVP: one record per position/application, company, optional contacts, job advertisement PDF, exact submitted resume/cover letter/other files, dated responses, interviews and history.
- **FR-13** Manual archive entry; no inbox synchronization in MVP. Attachments are optional. Company/job title required for draft; submission date required when marking submitted. Saving records does not submit applications.
- **FR-14** States: draft, submitted/awaiting response, interviewing, offer, rejected, withdrawn. Silence is not automatic rejection. Optional follow-up stays inside its record; no separate upcoming-task dashboard.
- **FR-15** Search by company, job title and contact. Creating a record for a company with history displays nonblocking information and a link to prior records, without confirmation or dismissal requirements.
- **FR-16** Authenticated application visitors view/download the resume version actually sent for that application. Archived versions remain unchanged by later edits. Direct access requesters receive the owner-designated main resume.
- **FR-17** English default, English/German interface and content. Images may remain English. Automatic translation is a draft with manual editing and owner approval before publication; exact semantic accuracy is not guaranteed.
- **FR-18** Side-by-side English/German preview. Missing/unapproved German content falls back to English without hiding the section. Publishing changed English invalidates the related German approval until reviewed.
- **FR-19** Content edits remain drafts until owner publication; previous published content remains visible until replacement is published.

## Related documents

- Nonfunctional requirements
- Constraints, assumptions and risks
- Scope and prioritization
- Acceptance and traceability


## Nonfunctional requirements

## Agreed quality expectations

- Protect original private files as well as pages; restrict the application archive to the owner.
- Preserve submitted documents and application/access history independently of later edits.
- Keep visitor entry simple and support reviewed bilingual publication.
- Define admin authentication, accessibility and performance acceptance criteria during requirements development; no numerical targets are assumed.

## Quality criteria requiring definition

Security verification, accessibility targets, performance limits, backup/recovery objectives and operational reliability criteria remain to be specified. No numerical targets or completed compliance assessments are implied.

Behavioral access/publication rules remain in Functional Requirements. Technical mechanisms belong in System Design, and verification evidence belongs in Testing.


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

These are unresolved items, not implemented solutions. The project-wide risk overview remains in Project Planning; this document records their implications for requirements.


## Prioritization and scope

## Agreed MVP

The functional baseline FR-01 through FR-19 is included in the agreed MVP: public introduction, configurable protected content, early application access creation, expiry/renewal, basic visits, email access requests, the private searchable application archive, resume version selection and bilingual publication.

No finer ordering, scoring or sprint allocation has been agreed. Requirement numbers are identifiers, not priorities. Dependencies should inform the order of implementation without introducing personal scheduling commitments.

## Deferred or excluded from MVP

- Multiple templates and advanced page builders.
- Page/download tracking and detailed visitor analytics.
- Automatic import of application correspondence from an inbox.
- A separate upcoming-task dashboard.

## Scope decisions

Project Planning is the primary source for project scope. This document applies that scope to the functional baseline. Proposed additions require Samira's decision and corresponding updates to affected requirements and acceptance criteria.
