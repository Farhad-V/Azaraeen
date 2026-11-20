# Deployment Runbook

## Prepare

Record the current and candidate versions. Verify access to configuration without printing secrets. Check that a compatible backup exists for the database and private files.

## Deploy and verify

Apply approved migrations and deploy. Smoke-test public EN/DE, owner access, protected file denial for unauthorized sessions, valid and expired grants, correct application resume and approved email delivery. Use synthetic records for production checks where possible.

## Recover

If a critical access, history or delivery check fails, stop the rollout. Restore the previous compatible release or follow the tested database and file recovery order. Record findings, affected versions and recovery results.

## Related documents

- [Test strategy](../05-Agile-Iterative-Development/02-Test-Strategy.md)
- [Release notes](03-Release-Notes.md)
