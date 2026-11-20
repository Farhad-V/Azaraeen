# Low-Level Design

Use these topics for data, interfaces and security details.


## Database design

Translate the conceptual entities and relationships from System Analysis into the selected database design. Cover companies, applications, optional contacts, document versions, credentials, visits and published bilingual content.

Define schema, keys, relationships, constraints, indexing, version preservation and data lifecycle boundaries. Describe data architecture: ownership, storage responsibilities, consistency and how archived submissions remain independent of later edits. Component/API contracts are maintained in API and Interfaces.

## Working material

Outline only. Database technology, schema and migrations have not yet been selected or produced here.


## File storage and versioning

## Work topics

Define private document storage, immutable application submission versions, resume-to-application association and authorized file delivery.

## Expected artifacts

Storage responsibilities, metadata, retention/deletion implications, failed-upload handling and links to security/database design. Do not assume a public file URL is private.

## Current material

Topic outline. Decisions, implementation and verification evidence will be added as the work is performed.


## API and interfaces

## Purpose and activities

Define component boundaries and contracts, including inputs, outputs, validation, authorization and error behavior. Specify HTTP APIs only where the architecture requires them; external APIs are not assumed.

## Expected outputs

Interface specifications supporting applications, access, content publication and resume delivery.

## Working material

Outline only. Detailed decisions and evidence remain to be added when this activity is performed.


## Integrations

## Purpose and activities

Design email request receipt, acknowledgement, owner approval and automatic credential delivery. Evaluate optional translation integration, privacy, provider cost and failure handling.

## Expected outputs

Integration contracts, event/data flows, retries and delivery outcomes. Provider choices remain open.

## Working material

Outline only. Detailed decisions and evidence remain to be added when this activity is performed.


## Security design

Specify owner and visitor authentication, session handling, authorization, private-file access checks, credential generation/storage/delivery and expiry/revocation enforcement. Keep the private application archive owner-only and preserve the agreed access model.

Record technical mechanisms, threat scenarios and their relationship to requirements. Email and translation flow design belongs in Integrations; operational diagnostics and secrets configuration belong in Infrastructure and Observability.

## Working material

Outline only. Detailed mechanisms and their verification remain to be developed; no completed security assessment is implied.


## Privacy and data protection

## Work topics

Identify personal information in owner documents, application contacts, access history and translation/mail exchanges.

## Expected artifacts

Data minimization, retention/deletion choices, provider data handling and privacy-notice inputs. Legal applicability remains to be assessed; no compliance claim is made.

## Current material

Topic outline. Decisions, implementation and verification evidence will be added as the work is performed.
