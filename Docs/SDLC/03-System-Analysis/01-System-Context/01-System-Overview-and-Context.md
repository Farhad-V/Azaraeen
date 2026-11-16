## System overview and context

## Purpose

Define the system boundary, actors and external dependencies for Azaraeen. This document describes the required system context; technical architecture is maintained in System Design.

## System boundary

Azaraeen provides public professional content, protected portfolio and resume access, owner content/publication controls, access administration and a private job-application archive. Saving an application record does not submit an application to an employer.

## Actors and external systems

- Samira operates the private administration and makes publication/access decisions.
- Public visitors view introductory content and may initiate an email access request.
- Approved visitors use application-specific or direct-request access.
- The visitor's email application composes and sends requests; the website cannot infer message receipt from a click.
- Mail services support receipt acknowledgement and approved credential delivery; the mechanism remains unresolved.
- Existing hosting provides the intended production environment, subject to compatibility assessment.
- A translation service is optional and undecided; translations require owner approval.

Job portals and employer systems are external. Application details and correspondence are manually archived in MVP. GitHub and LinkedIn are outbound profile links, not authenticated integrations.

## Related sources

- [Functional requirements](../../02-Requirements/02-Requirement-Specification/01-Functional-Requirements.md)
- [Stakeholders and users](../../02-Requirements/01-Discovery/02-Stakeholders-and-Users.md)
- [Processes and scenarios](../02-Behavior-and-Processes/01-Processes-and-User-Scenarios.md)

Detailed context diagrams remain to be developed.
