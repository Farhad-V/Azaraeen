# Deployment Plan

Production deployment is pending. Confirm the fit of the existing azaraeen.de domain and hosting before release.

1. Identify the candidate version and confirm owner acceptance and test evidence.
2. Configure HTTPS, server-side secrets, private storage and tested mail settings.
3. Back up existing data and files, record a rollback point, and verify an isolated restore.
4. Run migrations and deploy through the runbook, then record smoke results and release notes.

## Related documents

- [Test strategy](../05-Agile-Iterative-Development/02-Test-Strategy.md)
- [Release notes](03-Release-Notes.md)
