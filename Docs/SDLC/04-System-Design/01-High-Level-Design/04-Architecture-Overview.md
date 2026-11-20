# Architecture Overview

Proposed topology: browser → application → relational persistence and private file storage. Keep publication, visitor access, archive and integrations as distinct application modules. Resolve protected content and file access on the server. Delivery retries and operator status belong at the integration boundary.
