# Architecture Definition Document (ADD)
<!-- https://digital-portfolio.opengroup.org/togaf-standard-architecture-content/latest/01-doc/chap04.html -->
## Role/Purpose
Deliverable that describes the core architectural artifacts created during a project. 

This document is based on the [TOGAF® standard](https://publications.opengroup.org/standards/togaf/c220). 

## Dependencies

* [Architecture Requirements Specification (ARS)](./arch-requirements-specification.md)

## Contents

| Content | Description | Required |
|---------|-------------|----------|
| Scope | Define the scope of the architecture work, including systems, domains, and boundaries | Yes |
| Goals, objectives and constraints | Summarize the goals, objectives, and constraints that guided the architecture development | Yes |
| Stakeholders* | Identify the key stakeholders involved in the architecture development and their roles | Yes |
| Context* | Describe the context in which the architecture was developed, including business drivers, market conditions, and regulatory requirements | No |
| Architecture Principles | Reference the architecture principles that were applied during the architecture development. This can also be a reference to the general principles | No |
| Baseline Architecture | Describe the baseline architecture, including current state diagrams, models, and documentation | Recommended |
| Architecture models | Business, Data, Application, and Technology Architecture models that represent the target architecture | Yes |
| Building Block View* | Describe the building blocks that make up the architecture, including their relationships and interactions | Recommended |
| Rationale and justification for architectural approach | Explain the rationale and justification for the chosen architectural approach, including trade-offs and alternatives considered. This is important for a good acceptance. This is especially important for higher purposes (Strategy, Portfolio) | Recommended |
| Architecture Decisions* | Decisions made during the architecture development, including the reasoning behind them and their impact on the architecture | No |
| Mapping to Architecture Repoisotory | Reference the relevant architecture artifacts stored in the Architecture Repository | No |
| Gap Analysis | Identify the gaps between the baseline and target architectures, including any risks or issues that need to be addressed | Recommended |
| Impact assessment | Assess the impact of the target architecture on existing systems, processes, and stakeholders | No |
| Transition Architecture | Describe the transition architecture that outlines the steps required to move from the baseline to the target architecture | No |
| Glossary* | Define key terms and concepts used in the architecture document | No |

All parts are from the TOGAF® standard. Parts with * are from arc42 template.

## Document States

| State | Description |
|-------|-------------|
| Draft | Document is worked on and not yet approved |
| Review | Optional State to make it transparent that the document is in review |
| Approved | Document is approved and valid. Important is that the approval comes from the stakeholders |
| Obsolete | Document is obsolete and not valid anymore. This might be because the project was cancelled or a new version is available. |

## Document Templates

An example template is part of [TOGAF® Standard, 10th Edition Template Deliverables](https://publications.opengroup.org/i094). This might be a good starting point. 

Besides that I am also a fan of the [Arc42 Template](https://arc42.org/) which is more lightweight and easier to use. 