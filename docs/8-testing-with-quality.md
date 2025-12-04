# 🧪 Testing & Quality

---

## 1. Unit Testing

### High-Level Guidance
Verify individual components in isolation to catch bugs early and ensure code correctness.

### What to Know
- **JUnit 5**: test lifecycle, annotations (`@Test`, `@BeforeEach`, `@AfterEach`)
- **Assertions**: `assertEquals`, `assertTrue`, `assertThrows`
- **Mockito**: mocking dependencies, stubbing behavior
- **Parameterized tests**: running same test with multiple inputs

### Practical Usage
- Test services, utility methods, domain logic
- Keep tests **fast, isolated, deterministic**

---

## 2. Integration Testing

### High-Level Guidance
Test multiple components together to ensure they interact correctly.

### What to Know
- Spring Boot integration tests (`@SpringBootTest`)
- Test slices (`@WebMvcTest`, `@DataJpaTest`)
- TestContainers for databases and messaging systems
- Mocking vs real dependencies tradeoffs

### Practical Usage
- Validate repository + service + controller flows
- Catch configuration or wiring issues

---

## 3. API / End-to-End Testing

### High-Level Guidance
Verify API behavior from the consumer’s perspective.

### What to Know
- Tools: RestAssured, Postman, Cypress
- Validating HTTP response codes, headers, body
- Testing edge cases and error scenarios
- Test automation for CI/CD pipelines

### Practical Usage
- Regression testing of public APIs
- Contract testing between microservices

---

## 4. Contract Testing

### High-Level Guidance
Ensure services adhere to agreed-upon API contracts.

### What to Know
- **Pact** or Spring Cloud Contract
- Consumer-driven contracts
- Prevent breaking changes across microservices

---

## 5. Code Quality & Static Analysis

### High-Level Guidance
Maintain clean, reliable, and maintainable code.

### What to Know
- **Static analysis**: SonarQube, SpotBugs
- **Linting / formatting**: Checkstyle, PMD
- **Code coverage**: JaCoCo, Cobertura
- Best practices: naming, single responsibility, readability

### Practical Usage
- Integrate into CI/CD to prevent regressions
- Detect code smells and potential bugs

---

## 6. Test Strategies & Best Practices

### High-Level Guidance
Adopt consistent testing approaches to ensure reliability.

### What to Know
- **Arrange-Act-Assert** pattern
- **AAA for unit tests**: setup, execute, verify
- Test boundaries and edge cases
- Isolate external systems where possible
- Maintain **fast, repeatable, deterministic tests**

---

## 7. Continuous Testing in CI/CD

### High-Level Guidance
Automate tests to enforce quality in each code change.

### What to Know
- Integrate unit, integration, and API tests into pipelines
- Run tests in parallel where possible
- Fail fast for breaking changes
- Reporting and visibility

---

## 8. Mocking & Fakes

### High-Level Guidance
Simulate dependencies to isolate testable logic.

### What to Know
- **Mockito / Mockk**
- Stubbing and verification
- Differences between mocks, stubs, fakes, spies

### Practical Usage
- Avoid hitting external databases, APIs, or queues during unit tests
- Simulate edge cases and exceptions

---

## 9. Test Coverage vs Test Effectiveness

### High-Level Guidance
High coverage doesn’t always mean high-quality tests.

### What to Know
- Coverage metrics: line, branch, and path coverage
- Focus on meaningful tests (business logic, error handling)
- Avoid brittle tests tied to implementation details

---
