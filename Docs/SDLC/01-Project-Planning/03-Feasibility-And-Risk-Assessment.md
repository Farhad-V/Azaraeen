# Feasibility And Risk Assessment

azaraeen.de and the existing Hetzner Level 1 hosting are the preferred baseline. Verify runtime, database, HTTPS, private files, scheduled work and recovery on the actual plan before selecting a stack.

| Risk | Verification or mitigation |
|---|---|
| Private files exposed by the web root | Prove only authorized application requests can retrieve them |
| Mail receipt or delivery cannot be automated reliably | Test controlled receipt, approval, retries and duplicate handling |
| Confidential text sent to translation provider | Review data handling and cost before selecting a provider |
| Incorrect historical resume | Verify immutable version references and restore behavior |
| Unclear resume action before upload | Get owner decision on the visible unavailable state |
