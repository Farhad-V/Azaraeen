# Requirements Traceability Matrix

The criteria below are proposed verification targets for the agreed functional baseline. Execution evidence is pending.

| Requirement | Acceptance criterion | Evidence |
|---|---|---|
| FR-01 | The public page shows only the configured introduction sections. | Not run |
| FR-02 | A hidden certificate title, description or file is absent from public responses independently of the other fields. | Not run |
| FR-03 | One valid visitor session unlocks all published protected sections without a second password prompt. | Not run |
| FR-04 | Unauthorized users cannot fetch original private files; only resumes offer a download action. | Not run |
| FR-05 | An owner can issue a link and password for a draft containing only company and job title. | Not run |
| FR-06 | Access records identify the application and company/position without requiring a visitor identity. | Not run |
| FR-07 | Finite grants stop working at expiry, including existing sessions; no-expiry grants work until revoked. | Not run |
| FR-08 | Renewal keeps the link, password and history; explicit replacement changes credentials. | Not run |
| FR-09 | Refresh and navigation leave the count unchanged; a new eligible session increments it once. | Not run |
| FR-10 | The access request opens a prepared composer and presents a copyable address. | Not run |
| FR-11 | A received request is acknowledged and access credentials are sent only after owner approval. | Not run |
| FR-12 | The owner can retrieve application metadata, exact submitted files and dated history in the private archive. | Not run |
| FR-13 | Draft requires company/title; submission requires date; optional files may be absent; saving sends nothing. | Not run |
| FR-14 | The owner can record the defined lifecycle states and follow-up. Silence does not change status. | Not run |
| FR-15 | Company, title and contact searches find matching records; company history guidance does not block saving. | Not run |
| FR-16 | Application access returns the archived submitted resume; direct access returns the designated main resume. | Not run |
| FR-17 | English is default. German translation remains a draft until the owner edits or approves it for publication. | Not run |
| FR-18 | EN/DE preview is available. Missing or invalidated German falls back to English per content item. | Not run |
| FR-19 | Unpublished edits are invisible to visitors; publishing replaces the previous visible revision. | Not run |

Record the test ID, tested version, environment and result in the test strategy when evidence is available.

## Related documents

- [Software requirements](01-Software-Requirements-Specification.md)
- [Test strategy](../05-Agile-Iterative-Development/02-Test-Strategy.md)
