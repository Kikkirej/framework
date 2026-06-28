# Context and Influences

## Overview: System context

the system context shows components in the direct environment. Like interfaces or actors. 

It describes everything outside of the own system. System boundary definition is the primary goal. 

This is often done as a UML use case diagram.

## Quality, Risks and Contraints

Collecting those helps with decision making and makes sure no uncertainities come up.

Constraints can be technical or organisational.

**Technical constraints** (examples):
* Programming language or runtime must be used (e.g. Java, Python)
* Target operating system or platform (e.g. Linux, Windows, embedded)
* Specific database system required (e.g. Oracle, PostgreSQL)
* Hardware limitations (CPU, memory, storage)
* Network restrictions (firewall rules, bandwidth, offline capability)
* Existing frameworks or libraries that must be integrated
* Security standards that must be met (e.g. TLS 1.3, FIPS 140-2)
* Performance requirements (response time, throughput)

**Organisational constraints** (examples):
* Budget and cost limits
* Deadlines and release dates
* Team size and skill set
* Required use of internal tools or processes (e.g. CI/CD pipeline, ticketing system)
* Compliance with laws or regulations (e.g. GDPR, HIPAA)
* Vendor contracts or license agreements
* Coding or documentation standards mandated by the organisation
* Outsourcing rules or geographic restrictions on data processing



## Scenarios

A scenario is a short example for the use of the system.

Scenarios are good for 

* idenitification of architecture risks
* Risk driven work
* Evaluation of the architecture
* Tests (including acceptance tests)

They typically have 3 aspects

1. Source
2. Artifact (what really happens)
3. Measurment

Example: A remote user (source) sends at high load a request  over the network (Artifact) and gets a reply in 5 seconds(measurement).

## Architecture goals

Architecture goals are short, clear summaries for specific factors.

These are explicit and longterm. 

## Questions to understand a system

* what can the system do?
* How far are our rights to decide?
* WHo should use the system?
* With which other systems does it need to interact?
* How big will the system be approximately?


## Quality Measure of software

Quality factors are defined by **ISO 25010**. Often they are pushing against each other.

* Maintainability <--> Performance
* Usability <--> Security
* Portability <--> Performance
* Cost <--> Availability/Stability

