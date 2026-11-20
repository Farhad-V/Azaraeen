# API Specification

| Operation | Actor | Contract |
|---|---|---|
| Read published portfolio | Visitor | Locale input and audience-filtered output |
| Authenticate grant | Credential holder | Credential to scoped session or recoverable denial |
| Read protected artifact | Authorized visitor | Entitlement and valid grant required at read time |
| Save application | Owner | Draft requires company and title, submission adds date |
| Approve request / publish revision | Owner | Validate current state and return actionable status |

Transport and concrete paths remain open.
