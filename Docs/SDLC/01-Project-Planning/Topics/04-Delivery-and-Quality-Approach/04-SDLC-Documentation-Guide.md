## SDLC documentation guide

These seven folders are the working organization chosen for Azaraeen. They are not a prescribed universal lifecycle, independent projects or a required one-pass sequence. Folder numbers support navigation. Research, security, accessibility, quality assurance and collaboration span multiple phases.

| Phase | Primary documentation |
|---|---|
| [01 Project Planning](../01-Project-Definition/01-Project-Plan.md) | Purpose, scope, delivery approach, responsibilities, resources and risks. |
| [02 Requirements Engineering](../../../02-Requirements-Engineering/Topics/02-Requirement-Specification/01-Functional-Requirements.md) | User needs, required capabilities, quality expectations and acceptance criteria; supported by discovery evidence. |
| [03 System Analysis](../../../03-System-Analysis/Topics/01-System-Context/01-System-Overview-and-Context.md) | Detailed models of processes, domain information, rules and state transitions. Requirements analysis overlaps this work; models support rather than replace the requirement statements. |
| [04 System Design](../../../04-System-Design/01-High-Level-Design/01-Architecture/03-Architecture-Decisions.md) | Technical architecture, database, interfaces, security mechanisms and integrations. |
| [04 System Design — UI/UX](../../../04-System-Design/02-UI-UX-Design/) | Information architecture, interactions, screens, prototypes, evaluation and design specifications for implementation. |
| [Agile Iterative Development — Implementation](../../../05-Agile-Iterative-Development/Topics/02-Implementation/01-Design-and-Development-Collaboration/02-Development-Collaboration.md) | Construction guidance, implementation decisions and collaboration resolving design/engineering issues. |
| [Agile Iterative Development — Testing](../../../05-Agile-Iterative-Development/Topics/03-Testing/) | Verification plans/results, implementation design review and acceptance evidence. Test planning begins before coding is complete. |
| [06 Deployment and Release](../../../06-Deployment-Release/Topics/01-Release-Management/01-Release-and-Launch.md) | Release configuration, production checks, recovery and owner guidance. |
| [07 Maintenance and Evolution](../../../07-Maintenance-Evolution/Topics/01-Operations/01-Operations-and-Maintenance.md) | Operations, defect correction, updates and post-release evaluation. |

## Document ownership and overlap

- Each artifact has one primary source; other phases link to it.
- Original design specifications are maintained under System Design in UI/UX. Implementation holds a handoff index linking to those sources and records construction decisions; handoff is an ongoing collaboration activity, not an additional phase.
- System Analysis describes required processes and information. UX user flows design how people navigate and interact with those processes.
- Prototype usability evaluation belongs with UX/UI; comparison of working software against designs and acceptance criteria belongs with Testing. Usability testing of working software may inform both through links.
- Security requirements belong in Requirements, mechanisms in System Design, evidence in Testing and operational procedures in Deployment/Maintenance.
- The previously discussed 15-step design process is a reference for activities, not a second folder hierarchy or mandatory numbered process.

## Document maturity

Project Planning and the Requirements baseline contain decisions from project discussions and open items. The remaining activity outlines describe intended work. A file's existence does not mean the activity has been performed. Detailed acceptance criteria, technical designs, Figma screens and test evidence remain to be developed.

## Reference

[IEEE Computer Society — SWEBOK](https://www.computer.org/education/bodies-of-knowledge/software-engineering) provides software-engineering knowledge areas. The folder ownership above is the project's own documentation convention.







## Topic organization

Each phase has entry documents. Supporting topics are grouped under Topics or under the relevant design branch. Cross-phase references link to the original topic documents.




## Full structure

[Categories and topic documents](02-Documentation-Structure.md)


## Coverage review

[Comparison and integration of the supplied lifecycle outline](03-Documentation-Coverage-Review.md)
