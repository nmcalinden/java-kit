# 📘 Java -- Design & Architecture Guide

> Goal: Build strong theoretical + practical speaking ability for Java
> backend, system design, and interviews.

------------------------------------------------------------------------

## 1. Object-Oriented Programming (OOP)

### Core Pillars

#### Encapsulation

-   Bundling data + behavior together
-   Hiding internal state using `private` fields + public methods
-   Prevents invalid state and improves maintainability

#### Abstraction

-   Exposing what a class does, not how
-   Achieved using interfaces and abstract classes

#### Inheritance

-   Child class extends parent class
-   Promotes code reuse
-   Risks tight coupling

#### Polymorphism

-   Same method call → different behavior at runtime
-   Achieved via inheritance and interfaces

------------------------------------------------------------------------

## 2. Interfaces vs Abstract Classes

| Feature               | Interface | Abstract Class |
|-----------------------|-----------|----------------|
| Multiple inheritance | ✅ Yes    | ❌ No          |
| State/fields         | ❌ No     | ✅ Yes         |
| Default methods      | ✅ Yes    | ✅ Yes         |


------------------------------------------------------------------------

## 3. Access Modifiers

| Modifier   | Visibility                          |
|------------|--------------------------------------|
| public     | Everywhere                           |
| protected  | Same package + subclasses            |
| default    | Same package                         |
| private    | Same class only                      |


------------------------------------------------------------------------

## 4. Constructors

-   Initialize objects
-   Support overloading
-   Enable immutability and dependency injection

------------------------------------------------------------------------

## 5. Overloading vs Overriding

### Overloading (Compile-Time)

-   Same method name, different parameters

### Overriding (Runtime)

-   Same method signature, child overrides parent

------------------------------------------------------------------------

## 6. Parent vs Child Classes

-   Inheritance, overriding, specialization

------------------------------------------------------------------------

## 7. High Cohesion & Low Coupling

-   High cohesion: one focused job
-   Low coupling: minimal dependencies

------------------------------------------------------------------------

## 8. SOLID Principles

-   S: Single Responsibility
-   O: Open/Closed
-   L: Liskov Substitution
-   I: Interface Segregation
-   D: Dependency Inversion

------------------------------------------------------------------------

## 9. Object Relationships

-   Association
-   Aggregation
-   Composition

------------------------------------------------------------------------

## 10. Design Patterns

### Creational

-   Singleton, Factory, Abstract Factory, Builder, Prototype

### Structural

-   Adapter, Decorator, Facade

### Behavioral

-   Observer, Iterator, State

------------------------------------------------------------------------

## 11. Caching

-   Benefits: performance, scalability
-   Risks: stale data, memory usage

------------------------------------------------------------------------

## 12. Communication Models

-   Sync vs Async
-   Request/Response, Pub/Sub

------------------------------------------------------------------------

## 13. Microservice Communication

-   REST, Events, Messaging

------------------------------------------------------------------------

## 14. Communication Protocols

-   HTTP, TCP, gRPC, WebSockets, AMQP

------------------------------------------------------------------------

## 15. Architecture Styles

-   DDD
-   Clean Architecture
-   Onion Architecture

------------------------------------------------------------------------

## 16. Big O Notation

-   O(1)
-   O(log n)
-   O(n) 
-   O(n²)

------------------------------------------------------------------------
