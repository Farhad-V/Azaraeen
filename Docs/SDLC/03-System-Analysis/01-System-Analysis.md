# System Analysis

## Actors and boundaries

Samira owns content, grants and application records. Public visitors see published public content. Credential holders see published protected content and their entitled resume. Mail and translation providers support distinct workflows. The application archive remains owner-only.

## Main workflows

- **Publication:** edit a draft, preview English and German, approve translation and publish. A changed English source invalidates downstream German approval.
- **Application:** create a draft from company and title, attach optional artifacts, record submission date when submitted, and append dated responses or interviews.
- **Grant:** issue while draft, verify and count access by session, renew or revoke, and block expired access even for an existing session.
- **Request:** visitor sends mail, system acknowledges receipt, Samira approves, system delivers credentials.

## Data and invariants

One company can have several applications. Each application keeps dated history and immutable submitted artifact references. A grant belongs to an application or a direct-access request. Public content depends on publication and audience visibility; locale fallback operates per content item.

Draft can progress to submitted/awaiting response and later interviewing, offer, rejected or withdrawn as appropriate. Silence leaves status unchanged. Rules for reopening records and the unavailable resume state require owner review.
