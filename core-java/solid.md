# SOLID Principles

The SOLID principles are a set of five design principles that aim to make software systems more scalable, flexible, and maintainable. The five principles are:

## Single Responsibility Principle (SRP)
A class should have only one reason to change, meaning it should have only one responsibility or job to do. If a class has multiple responsibilities, changes to one responsibility may cause unexpected issues in other responsibilities.

## Open-Closed Principle (OCP)
A class should be open for extension but closed for modification. This means that you should be able to add new functionality to a class without changing its existing code.

## Liskov Substitution Principle (LSP)
Subtypes should be able to substitute their base types without affecting the correctness of the program. In other words, if you have a function that takes an object of a certain class as a parameter, you should be able to substitute that object with an object of any of its subclasses without changing the behavior of the function.

## Interface Segregation Principle (ISP)
Clients should not be forced to depend on interfaces they do not use. This means that you should design your interfaces to be cohesive and only expose the methods that are needed by the clients that use them.

## Dependency Inversion Principle (DIP)
High-level modules should not depend on low-level modules. Both should depend on abstractions. Abstractions should not depend on details. Details should depend on abstractions.
