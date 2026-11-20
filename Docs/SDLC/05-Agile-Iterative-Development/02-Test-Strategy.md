# Test Strategy

Verification is planned. No application test execution has been recorded.

| Test | Focus | Scope |
|---|---|---|
| T-01 | Public and protected output | FR-01–FR-04 |
| T-02 | Grant lifecycle and session counts | FR-05–FR-09 |
| T-03 | Request, acknowledgement and approved delivery | FR-10, FR-11 |
| T-04 | Draft, submission, search and history | FR-12–FR-15 |
| T-05 | Correct resume, including older submitted versions | FR-16 |
| T-06 | Locale fallback and draft publication | FR-17–FR-19 |
| T-07 | Keyboard use, backup restoration and response measurements | Quality checks |

Use a controlled clock for expiry and synthetic file fixtures for access tests. Record version, environment, test data, expected result, actual result and evidence. Treat unauthorized private file reads and incorrect resume delivery as release blockers.

## Related documents

- [Acceptance criteria](../02-Requirements-Engineering/03-Requirements-Traceability-Matrix.md)
