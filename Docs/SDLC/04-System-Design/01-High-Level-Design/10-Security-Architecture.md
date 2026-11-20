# Security Architecture

Keep owner authentication separate from visitor grants. Recheck grant validity and relevant file entitlement at the server boundary, including requests from previously authenticated sessions. Protect admin actions and private resources, and exclude credentials and private contact details from logs.
