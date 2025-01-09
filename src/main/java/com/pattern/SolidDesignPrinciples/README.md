# SOLID Design Principles
- **S**ingle Responsibility Principle
- **O**pen Closed Principle
- **L**iskov Substitution Principle
- **I**nterface Segregation Principle
- **D**ependency Inversion Principle

## Single Responsibility Principle
> There should never be more than one reason for a class to change.

Single Responsibility means that the class provides a very _focusd, single functionality_. Or it _addresses a specific concern_.

## Open Closed Principle
> Software entities (Classes, Modules, Methods, etc.) should be open for extension, but closed for modification.

Open for extension means it should be able to extend existing behavior.
Closed for modification means existing code remains unchanged.

This principle tells that to avoid or to completely avoid modifying existing base classes and use inheritance and overriding in order to achieve extension of existing behavior. 

## Liskov Substitution Principle
> We should be able to substitute base class objects with child class objects. This should not alter behavior/characteristics of program.

## Interface Segregation Principle
> Clients should not be forced to depend upon interfaces that they do not use.

In particular, we are talking about methods. Clients should not have to depend on methods that are defined in interfaces that they don't use.

_Interface Pollution_: Large Interfaces, Unrelated Methods

_Signs of Interface Pollution_:
  - Classes have empty method implementations.
  - Method implementations throw UnsupportedOperationException (or similar).
  - Method implementations return null or default/dummy values.

## Dependency Inversion Principle
> - High level modules should not depend upon low level modules. Both should depend upon abstractions.
> - Abstractions should not depend upon details. Details should depend upon abstractions.