# Meta Architecture

Meta Architecture is the set of high level decisions, which influence the system structure without being the strucutre themselves. Styles, Patterns or principles form the design.
The consistent application of the meta archtiecture ensure coneptional integrity

## Architecutre Patterns

Relevant architecture patterns are the following

### Layered Architecture

Hierarchical structure of a system. Layers a*re seperated by interfaces.

```mermaid
graph TD
    A[Presentation Layer] --> B[Application Layer]
    B --> C[Domain / Business Logic Layer]
    C --> D[Infrastructure / Data Access Layer]
    D --> E[(Database)]

    style A fill:#4A90D9,color:#fff
    style B fill:#5BA85A,color:#fff
    style C fill:#E8A838,color:#fff
    style D fill:#C0392B,color:#fff
```

Pro:

* Reusability and Replaciabilty 
* Standardiziation
* Maintenance

Contra:

* Efficiency 

### Pipes & Filters

```mermaid
graph LR
    I[Input] --> F1[Filter 1]
    F1 -->|Pipe| F2[Filter 2]
    F2 -->|Pipe| F3[Filter 3]
    F3 --> O[Output]

    style I fill:#7F8C8D,color:#fff
    style F1 fill:#2980B9,color:#fff
    style F2 fill:#2980B9,color:#fff
    style F3 fill:#2980B9,color:#fff
    style O fill:#7F8C8D,color:#fff
```

### Shared Repository

```mermaid
graph TD
    R[(Shared Repository)]
    C1[Component A] <--> R
    C2[Component B] <--> R
    C3[Component C] <--> R
    C4[Component D] <--> R

    style R fill:#8E44AD,color:#fff
    style C1 fill:#2980B9,color:#fff
    style C2 fill:#2980B9,color:#fff
    style C3 fill:#2980B9,color:#fff
    style C4 fill:#2980B9,color:#fff
```

### Microcore Architecture

```mermaid
graph TD
    Core[Microcore / Kernel]
    P1[Plugin 1] --> Core
    P2[Plugin 2] --> Core
    P3[Plugin 3] --> Core
    P4[Plugin 4] --> Core
    Core --> S[Core Services]

    style Core fill:#C0392B,color:#fff
    style P1 fill:#2980B9,color:#fff
    style P2 fill:#2980B9,color:#fff
    style P3 fill:#2980B9,color:#fff
    style P4 fill:#2980B9,color:#fff
    style S fill:#27AE60,color:#fff
```

### Model-View-Controller

```mermaid
graph LR
    U([User]) -->|interacts| V[View]
    V -->|user action| C[Controller]
    C -->|updates| M[Model]
    M -->|notifies| V

    style U fill:#7F8C8D,color:#fff
    style V fill:#2980B9,color:#fff
    style C fill:#E8A838,color:#fff
    style M fill:#27AE60,color:#fff
```

