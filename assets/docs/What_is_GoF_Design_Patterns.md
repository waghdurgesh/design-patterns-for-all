# GoF (Gang of Four) Design Patterns

## Introduction

**GoF (Gang of Four) Design Patterns** are a collection of **23 software design patterns** introduced in the book:

> **Design Patterns: Elements of Reusable Object-Oriented Software (1994)**

The book was written by:

- Erich Gamma
- Richard Helm
- Ralph Johnson
- John Vlissides

These four authors are collectively known as the **Gang of Four (GoF)**.

A **design pattern** is a **general, reusable solution** to a commonly occurring problem in software design. It is **not a ready-made implementation**, but rather a template or best practice that can be adapted to different situations.

---

# Categories of GoF Design Patterns

The 23 patterns are divided into three categories:

1. Creational Patterns
2. Structural Patterns
3. Behavioral Patterns

---

# 1. Creational Design Patterns

Creational patterns deal with **object creation mechanisms**, making object creation more flexible and reusable.

| Pattern | Purpose |
|----------|----------|
| Singleton | Ensures only one instance of a class exists. |
| Factory Method | Creates objects without specifying their concrete classes. |
| Abstract Factory | Creates families of related objects. |
| Builder | Constructs complex objects step by step. |
| Prototype | Creates new objects by cloning existing ones. |

## Example

```java
DatabaseConnection connection = DatabaseConnection.getInstance();
```

The above uses the **Singleton Pattern**, ensuring only one database connection instance exists.

---

# 2. Structural Design Patterns

Structural patterns define **how classes and objects are combined** to form larger structures.

| Pattern | Purpose |
|----------|----------|
| Adapter | Converts one interface into another compatible interface. |
| Bridge | Separates abstraction from implementation. |
| Composite | Treats individual objects and object groups uniformly. |
| Decorator | Adds new functionality dynamically without modifying the original object. |
| Facade | Provides a simplified interface to a complex subsystem. |
| Flyweight | Shares objects to reduce memory usage. |
| Proxy | Controls access to another object. |

## Example

A payment system may expose a single `PaymentService` that internally communicates with multiple payment gateways.

This is an example of the **Facade Pattern**.

---

# 3. Behavioral Design Patterns

Behavioral patterns define **how objects communicate and interact**.

| Pattern | Purpose |
|----------|----------|
| Chain of Responsibility | Passes requests through multiple handlers until processed. |
| Command | Encapsulates requests as objects. |
| Interpreter | Defines grammar and interprets language expressions. |
| Iterator | Traverses collections without exposing internal representation. |
| Mediator | Centralizes communication between objects. |
| Memento | Saves and restores an object's previous state. |
| Observer | Notifies dependent objects when state changes. |
| State | Changes behavior based on internal state. |
| Strategy | Encapsulates interchangeable algorithms. |
| Template Method | Defines the skeleton of an algorithm while allowing subclasses to customize steps. |
| Visitor | Adds new operations without modifying existing object structures. |

## Example

```java
sort(new QuickSortStrategy());
sort(new MergeSortStrategy());
```

Choosing different sorting algorithms at runtime is an example of the **Strategy Pattern**.

---

# Why Use GoF Design Patterns?

GoF patterns help developers:

- Reuse proven design solutions.
- Improve maintainability.
- Reduce code duplication.
- Minimize coupling between components.
- Increase flexibility and scalability.
- Make code easier to understand and test.
- Communicate architecture using a common vocabulary.

---

# Real-World Analogy

Think of design patterns as **architectural blueprints**.

- A **class** is like a house.
- A **design pattern** is like the blueprint used to build many similar houses.
- Different builders can implement the same blueprint differently while preserving the overall design.

---

# Most Commonly Used GoF Patterns in Industry

The following patterns are frequently used in real-world applications and technical interviews:

- Singleton
- Factory Method
- Builder
- Adapter
- Decorator
- Facade
- Observer
- Strategy
- Command
- Template Method

---

# Summary

GoF Design Patterns provide reusable solutions to common object-oriented design problems.

## Creational Patterns (5)

- Singleton
- Factory Method
- Abstract Factory
- Builder
- Prototype

## Structural Patterns (7)

- Adapter
- Bridge
- Composite
- Decorator
- Facade
- Flyweight
- Proxy

## Behavioral Patterns (11)

- Chain of Responsibility
- Command
- Interpreter
- Iterator
- Mediator
- Memento
- Observer
- State
- Strategy
- Template Method
- Visitor

Understanding these patterns helps in writing cleaner, more maintainable, and scalable software systems.