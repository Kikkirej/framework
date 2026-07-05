# Overview

Over the years I had again and again the experience, which I expect many engineers share, that software products are supportin business processes.

There are different ways to implement the business processes, which I saw over the years.

* Hardcoded (classic, but truth is completely in source code)
* Workflow Engine (BPMN or other based orchestration engine)
* Domain Specific Language (DSL) (custom definition of flow logic)
* Workflow to code
    * Okay... I never saw that live yet, but I love the concept :D

All have pros and cons depending on different use cases and also based on the experience of the dev team.

From my point of view the fitting for different use cases:

| Use Case | Proposed Solution | Rationale |
|---|---|---|
| Small business workflows (e.g. approval or follow-up reminder flows) | Hardcoded logic | The overhead of a workflow engine adds too much complexity — both in development and runtime. Can be reconsidered if a workflow engine is already present in the stack. |
| Hardcoded flow in an application (distributed or centralized) | Workflow Engine or Workflow-to-Code (e.g. Kogito) | Keeps the business flow consistent with the code and separates process definition from implementation, reducing error probability. Also enables scaling and distribution in a cloud-native environment. |
| Deployment-specific workflows | Workflow Engine | A DSL could work technically, but adds unnecessary complexity and requires users to learn a new language. A workflow engine is the clear recommendation here. Be aware that this level of configurability is hard to quality-test. |
| Long-running business transactions / sagas (e.g. order fulfillment, onboarding) | Workflow Engine | Provides durable state, built-in retry logic, and compensation (saga rollback) out of the box. Hardcoding this leads to fragile state machines that are difficult to debug and recover after failures. |
| Human-in-the-loop processes (e.g. manual approvals, role-based task assignment) | Workflow Engine | BPMN-based engines have first-class support for user tasks, deadlines, and escalations. Implementing this hardcoded is error-prone and hard to change as process rules evolve. |

For choosing a concrete workflow engine, see the [technology comparison](technology-comparison.md) of Camunda 7/8, jBPM 7/10, Kogito, Operaton, CIB seven, Flowable and Activiti.
