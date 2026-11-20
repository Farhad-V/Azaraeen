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

- [Nonfunctional requirements](02-Non-Functional-Requirements.md)
- [Constraints, assumptions and risks](../03-Scope-and-Constraints/01-Constraints-Assumptions-Risks.md)
- [Scope and prioritization](../03-Scope-and-Constraints/02-Prioritization-and-Scope.md)
- [Acceptance and traceability](../04-Acceptance-and-Traceability/01-Acceptance-Criteria-and-Traceability.md)
