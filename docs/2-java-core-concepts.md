# ☕ Java Core Concepts

---

## 1. Primitive vs Wrapper (Non-Primitive) Types

### High-Level Guidance
Understand the difference between raw memory-efficient values and object-based representations used in collections and generics.

### What to Know
- Primitives: `int`, `double`, `boolean`, `char`, etc.
- Wrappers: `Integer`, `Double`, `Boolean`, `Character`
- Primitives store values directly; wrappers store references
- Wrappers support `null`, primitives do not

### Practical Usage
- Collections require wrapper types
- Wrappers used in generics and streams

---

## 2. `final` Keyword

### High-Level Guidance
Controls mutability and inheritance.

### What to Know
- `final` variable → cannot be reassigned
- `final` method → cannot be overridden
- `final` class → cannot be extended

### Practical Usage
- Immutability for thread safety
- Preventing framework extension

---

## 3. Arrays, Lists, Maps, Sets

### High-Level Guidance
Core data storage and access mechanisms in Java.

### What to Know
- Arrays: fixed size, fast access
- List: ordered, allows duplicates
- Set: unique elements
- Map: key-value storage

### Big-O Awareness
- `ArrayList` search → O(n)
- `HashMap` lookup → O(1) average

---

## 4. Queue vs Stack

### High-Level Guidance
Understand data flow ordering.

### What to Know
- Stack: LIFO (method calls, undo)
- Queue: FIFO (task scheduling, messaging)

---

## 5. JVM & Memory Management

### High-Level Guidance
Java runs on a virtualized runtime with automatic memory cleanup.

### What to Know
- Heap vs Stack
- Young vs Old Generation
- Garbage Collection basics
- JVM vs JRE vs JDK

---

## 6. Exceptions

### High-Level Guidance
How Java enforces error handling at compile time and runtime.

### What to Know
- Checked vs Unchecked exceptions
- `try-catch-finally`
- `throw` vs `throws`
- Custom exceptions

---

## 7. Enums

### High-Level Guidance
Typesafe representation of fixed constant sets.

### What to Know
- Enum can have fields and methods
- Used in state machines and configs

---

## 8. Threads & Concurrency

### High-Level Guidance
Running multiple tasks at once safely.

### What to Know
- `Thread` vs `Runnable`
- Race conditions
- Synchronization
- Visibility vs atomicity

---

## 9. `Comparator` vs `Comparable`

### High-Level Guidance
Sorting strategies for objects.

### What to Know
- `Comparable` → natural ordering
- `Comparator` → external/custom ordering

---

## 10. Generics

### High-Level Guidance
Type safety at compile time.

### What to Know
- `<T>` generic types
- Upper & lower bounds (`extends`, `super`)
- Type erasure

---

## 11. Binary Tree

### High-Level Guidance
Fundamental hierarchical data structure.

### What to Know
- Root, parent, child, leaf
- Traversals (in-order, pre-order, post-order)
- BST vs general tree

---

## 12. Heap vs Stack Memory

### High-Level Guidance
How Java organizes memory.

### What to Know
- Stack: method calls, primitives, references
- Heap: objects, shared memory
- Stack is fast, heap is larger

---

## 13. Functional Interfaces & Lambda Utilities

### High-Level Guidance
Foundation of modern Java functional programming.

### What to Know
- `Predicate`, `Consumer`, `Supplier`, `Function`
- Method references (`::`)
- `Optional` for null safety

---

## 14. `static` Keyword

### High-Level Guidance
Class-level shared behavior and state.

### What to Know
- Static fields belong to the class
- Static methods cannot access instance state
- Static blocks for initialization

---

## 15. `Date` vs `LocalDate`

### High-Level Guidance
Old vs modern date/time API.

### What to Know
- `Date` is mutable and poorly designed
- `LocalDate`, `LocalTime`, `LocalDateTime` are immutable and thread-safe
- `ZonedDateTime` for time zones

---

## 16. Autoboxing

### High-Level Guidance
Automatic conversion between primitives and wrappers.

### What to Know
- `int` ↔ `Integer`
- Hidden performance cost
- Can cause `NullPointerException`

---

## 17. Data Structures & Algorithms

### High-Level Guidance
Performance foundation of all software.

### What to Know
- Arrays, Linked Lists, Trees, Hash Tables
- Sorting: quicksort, mergesort
- Searching: binary search

---

## 18. Atomics

### High-Level Guidance
Lock-free thread-safe operations.

### What to Know
- `AtomicInteger`, `AtomicBoolean`
- CAS (Compare-And-Swap)

---

## 19. Executors

### High-Level Guidance
High-level thread management.

### What to Know
- `FixedThreadPool`, `CachedThreadPool`
- `Future`, `Callable`
- Graceful shutdown

---

## 20. Streams API

### High-Level Guidance
Declarative data processing.

### What to Know
- Intermediate vs terminal operations
- `map`, `filter`, `reduce`, `collect`
- Parallel streams

---
