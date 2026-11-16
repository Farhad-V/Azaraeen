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

Describe information exchanged, triggering events, expected outcomes and failure cases here. Provider/API/protocol choices belong in [Integrations](../../04-System-Design/04-Interfaces-and-Integrations/02-Email-and-Translation-Integrations.md). Translation provider, cost and handling of confidential text remain open. No automatic job-portal submission or inbox import is included in MVP.

- [System context](../01-System-Context/01-System-Overview-and-Context.md)
- [Open requirements decisions](../../02-Requirements/03-Scope-and-Constraints/01-Constraints-Assumptions-Risks.md)
