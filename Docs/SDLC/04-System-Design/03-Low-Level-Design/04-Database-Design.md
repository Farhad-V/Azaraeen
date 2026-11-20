# Database Design

Proposed entities: Company, Contact, Application, ApplicationEvent, ArtifactVersion, ContentRevision, TranslationRevision, AccessGrant, VisitorSession and AccessRequest. Application requires company and job title. Submitted status requires a submission date. Link submitted artifacts by immutable version ID and enforce references at persistence boundaries.
