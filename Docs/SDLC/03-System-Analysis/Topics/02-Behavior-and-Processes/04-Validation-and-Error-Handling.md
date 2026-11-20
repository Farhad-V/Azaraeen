## Validation and error handling

## Purpose

Analyze validation rules and observable error outcomes. Link each scenario to its requirement and relevant state model. Technical enforcement belongs in System Design/Implementation; message presentation belongs in UX/UI; verification evidence belongs in Testing.

## Established rules

- Company and position are required to save an application draft.
- A submission date is required when marking an application submitted; attachments remain optional.
- Credentials can be created before submission and before documents are uploaded.
- Expired or revoked access must not allow further protected requests, including through an existing session.
- Expired access explains that validity has ended and offers the email request route.
- Missing/unapproved German content falls back to English; unpublished edits do not replace the current published version.
- Renewal preserves the existing link, password and history; credential replacement is a separate action.

## Scenarios requiring further decisions

| Scenario | Analysis needed |
|---|---|
| Invalid credentials | Define user feedback and retry behavior without exposing private content. |
| Resume not uploaded for an application | Define the visitor result; do not silently substitute an unrelated resume. |
| Invalid expiry value | Define accepted values, timezone presentation and validation feedback. |
| Unsupported, oversized or failed file upload | Establish permitted file types/limits and recovery behavior; the advertisement archive is PDF. |
| Mail acknowledgement/delivery fails | Define owner visibility, retry behavior and outcomes without implying access was delivered. |
| Translation fails or English changes | Preserve publication/approval rules and English fallback; define owner feedback. |
| Invalid or inconsistent application/event dates | Establish permitted corrections and chronological rules without assuming every unusual date is invalid. |

These open scenarios are not newly approved feature requirements. Resolve them against the [requirements baseline](../../../02-Requirements-Engineering/Topics/02-Requirement-Specification/01-Functional-Requirements.md) and record accepted rules in [Business Rules and State Transitions](03-Business-Rules-and-State-Transitions.md).
