# 🌱 Spring & Spring Boot – Speaking & Practical Mastery

---

## 1. Inversion of Control (IoC)

### High-Level Guidance
IoC shifts control of object creation and lifecycle from the developer to the Spring container.

### What to Know
- Objects are managed by the Spring container
- Promotes loose coupling
- Enables dependency injection

### Practical Usage
- All `@Component`, `@Service`, `@Repository` beans are IoC-managed

---

## 2. Dependency Injection (DI)

### High-Level Guidance
Dependencies are provided externally instead of created internally.

### What to Know
- Constructor injection (preferred)
- Field injection (discouraged)
- Setter injection

### Practical Usage
- Required for testability and clean architecture

---

## 3. Beans & Scopes

### High-Level Guidance
Beans are objects managed by the Spring container.

### What to Know
- Singleton (default)
- Prototype
- Request
- Session

### Practical Usage
- Services are usually Singleton
- Controllers are typically Singleton

---

## 4. Spring Annotations

### High-Level Guidance
Annotations drive behavior through configuration.

### What to Know
- Stereotypes: `@Component`, `@Service`, `@Repository`, `@Controller`, `@RestController`
- Web: `@GetMapping`, `@PostMapping`
- Injection: `@Autowired`
- Config: `@Configuration`, `@Bean`

---

## 5. Profiles

### High-Level Guidance
Environment-specific configuration management.

### What to Know
- `@Profile`
- `spring.profiles.active`
- `application-dev.yml`, `application-prod.yml`

---

## 6. REST APIs with Spring

### High-Level Guidance
Building HTTP APIs using Spring MVC.

### What to Know
- `@RestController`
- `ResponseEntity`
- DTOs vs Entities
- Validation with `@Valid`

---

## 7. Spring Boot vs Spring Framework

### High-Level Guidance
Spring Boot simplifies Spring Framework setup and configuration.

### What to Know
- Auto-configuration
- Embedded servers
- Starters
- Opinionated defaults

---

## 8. Eager vs Lazy Loading

### High-Level Guidance
Controls when beans or ORM relationships are initialized.

### What to Know
- Eager: loaded at startup
- Lazy: loaded on first use
- Lazy initialization improves startup time

---

## 9. Lombok – Pros vs Cons

### High-Level Guidance
Reduces boilerplate by generating code at compile time.

### Pros
- `@Getter`, `@Setter`, `@Builder`, `@Data`
- Improves readability

### Cons
- Hidden logic
- Debugging difficulty
- IDE/plugin dependency

---

## 10. Error Handling

### High-Level Guidance
Centralized exception management across REST APIs.

### What to Know
- `@ControllerAdvice`
- `@ExceptionHandler`
- Custom error response models

---

## 11. Hibernate

### High-Level Guidance
Object-Relational Mapping (ORM) provider.

### What to Know
- Entities
- Session vs EntityManager
- First-level cache
- Lazy loading
- N+1 query problem

---

## 12. Spring Data JPA

### High-Level Guidance
Abstraction layer over JPA and Hibernate.

### What to Know
- `JpaRepository`
- Derived queries
- Pagination & sorting
- Custom JPQL & native queries

---

## 13. `@Transactional`

### High-Level Guidance
Manages database transactions declaratively.

### What to Know
- Propagation types
- Rollback behavior
- Read-only transactions

---

## 14. Logging

### High-Level Guidance
Tracking application behavior, errors, and performance.

### What to Know
- SLF4J + Logback
- Log levels (`INFO`, `DEBUG`, `ERROR`)
- Structured logging
- Log correlation IDs

---
