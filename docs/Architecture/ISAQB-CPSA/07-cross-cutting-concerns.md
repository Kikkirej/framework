# Cross Cutting Concerns

Aspects which are not clearly connectable for one module. 

This can be for example...

* ... Configuration
* ... Security (Authn/Authz/Encryption)
* ... Protocol (Tracing/Logging/Audit)
* ... Persistence
* ... Monitoring
* ... UI (Navigation/Validation/Dataconversion)
* ... Transactions
* ... Error Handling
* ...

THe high level process is to identify areas (like the ones before), Make decision how it should be handled and the apply it to the different modules.

If cross-cutting concerns are not taken into account the danger is to have...

* ... fragmented solutions and redudancy
* ... error likeliness
* ... dirty/hard to read code
* ... bad maintenance

## AOP

Possible way to address cross cutting concerns 

Advice and Code are seperated. 

| Term      | Meaning                                                                 |
|-----------|-------------------------------------------------------------------------|
| Aspect    | A module encapsulating a cross-cutting concern (e.g. logging, security) |
| Advice    | The code that is executed when a joinpoint is reached                   |
| Joinpoint | A specific point in program execution (e.g. method call, exception)     |
| Pointcut  | A predicate that selects which joinpoints an advice applies to          |

This can be merged with an Aspect Weaver. 

There are also some frameworks for different programming languages

* Java
** AspectJ
* .NET
** PostSharp
** Aspect#
* C++
** AspectC++
* Spring
** Spring AOP
