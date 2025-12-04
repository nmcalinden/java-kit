# ⚙️ DevOps & CI/CD for Java

---

## 1. Build Tools

### High-Level Guidance
Automate building, dependency management, and packaging of Java projects.

### What to Know
- **Maven**
  - `pom.xml` dependency management
  - Plugins: `maven-compiler-plugin`, `maven-surefire-plugin`
  - Lifecycle phases: `clean`, `compile`, `test`, `package`, `install`
- **Gradle**
  - Build scripts (Groovy/Kotlin DSL)
  - Dependency caching
  - Incremental builds
- Choosing Maven vs Gradle depending on team/project preference

---

## 2. Version Control & Branching

### High-Level Guidance
Maintain code history and support collaborative development.

### What to Know
- Git basics: `clone`, `branch`, `merge`, `rebase`
- Branching strategies:
  - Git Flow
  - GitHub Flow
  - Trunk-based development
- Pull requests and code review practices

---

## 3. Continuous Integration (CI)

### High-Level Guidance
Automatically build and test code changes to detect issues early.

### What to Know
- CI tools: GitHub Actions, Jenkins, GitLab CI, CircleCI
- Steps:
  1. Checkout code
  2. Build project
  3. Run unit tests
  4. Static analysis and code quality checks
- Fail fast strategy for broken builds
- Test reporting and artifact storage

---

## 4. Continuous Delivery / Continuous Deployment (CD)

### High-Level Guidance
Automate deployment of verified builds to staging/production.

### What to Know
- Pipeline stages: build → test → deploy
- Blue-green deployments
- Canary releases
- Rollbacks and versioned releases
- Environment configuration management

---

## 5. Containerization

### High-Level Guidance
Package Java applications with dependencies for consistent deployments.

### What to Know
- **Docker**
  - Dockerfile for Java apps
  - Multi-stage builds for smaller images
  - Docker Compose for local orchestration
- Benefits:
  - Consistent dev/staging/prod environments
  - Isolation and reproducibility

---

## 6. Orchestration & Kubernetes (Optional Advanced)

### High-Level Guidance
Run and manage containers at scale.

### What to Know
- Pods, Deployments, Services
- ConfigMaps and Secrets
- Horizontal Pod Autoscaling
- Rolling updates

---

## 7. Logging & Monitoring

### High-Level Guidance
Observe application health and diagnose production issues.

### What to Know
- Centralized logging: ELK stack (Elasticsearch, Logstash, Kibana)
- Metrics collection: Prometheus
- Visualization: Grafana
- Health endpoints: Spring Boot Actuator
- Alerting: thresholds for CPU, memory, error rates

---

## 8. Configuration Management & Secrets

### High-Level Guidance
Manage environment-specific configuration securely.

### What to Know
- Externalized config: `application.properties`, `application.yml`
- Profiles for dev, test, prod
- Secrets management: HashiCorp Vault, AWS Secrets Manager
- Avoid hardcoding passwords/API keys

---

## 9. CI/CD Best Practices for Java Projects

### High-Level Guidance
Ensure reliability, reproducibility, and maintainability of deployments.

### What to Know
- Keep builds **fast** and **deterministic**
- Run **unit, integration, and API tests** in pipeline
- Use **artifact repositories** (Nexus, Artifactory)
- Automate rollback on failures
- Monitor deployment metrics for continuous improvement

---
