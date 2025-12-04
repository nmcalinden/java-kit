# 🌐 Distributed Systems

---

## 1. Introduction to Distributed Systems

### High-Level Guidance
Systems where components run on multiple networked machines but act as a single system.

### What to Know
- Benefits: scalability, fault tolerance, availability
- Challenges: network latency, partial failures, consistency
- Key properties: CAP theorem, distributed consensus

---

## 2. CAP Theorem

### High-Level Guidance
Trade-offs between **Consistency, Availability, and Partition Tolerance**.

### What to Know
- **Consistency (C)**: all nodes see the same data
- **Availability (A)**: every request gets a response
- **Partition Tolerance (P)**: system works despite network failures
- Only two of three can be guaranteed simultaneously

### Practical Usage
- Choose CP for financial systems (strong consistency)
- Choose AP for high-scale web apps (eventual consistency)

---

## 3. Consistency Models

### High-Level Guidance
Define how data is replicated across nodes.

### What to Know
- Strong consistency
- Eventual consistency
- Causal consistency
- Read-your-writes guarantee

---

## 4. Consensus & Coordination

### High-Level Guidance
Mechanisms to ensure agreement in distributed systems.

### What to Know
- Paxos, Raft algorithms
- Leader election
- Quorums
- Zookeeper / etcd

---

## 5. Fault Tolerance & Reliability

### High-Level Guidance
Handling failures gracefully in distributed systems.

### What to Know
- Replication strategies (master-slave, multi-master)
- Heartbeats & failure detection
- Retry strategies & exponential backoff
- Circuit breaker patterns

---

## 6. Scalability

### High-Level Guidance
Ability to handle growing workload efficiently.

### What to Know
- **Vertical scaling**: bigger machines
- **Horizontal scaling**: adding nodes
- Sharding / Partitioning
- Load balancing (Round-robin, Least Connections, Sticky sessions)

---

## 7. Distributed Transactions

### High-Level Guidance
Managing data consistency across multiple nodes.

### What to Know
- ACID vs BASE
- Two-Phase Commit (2PC)
- Sagas for eventual consistency
- Idempotency and compensation actions

---

## 8. Messaging & Event-Driven Architectures

### High-Level Guidance
Decoupling services via asynchronous communication.

### What to Know
- Event sourcing
- CQRS (Command Query Responsibility Segregation)
- Kafka, RabbitMQ, JMS
- Pub/Sub vs Event streaming

---

## 9. Caching & Data Replication

### High-Level Guidance
Improve performance and availability in distributed systems.

### What to Know
- Distributed caches: Redis Cluster, Memcached
- Cache consistency challenges
- Data replication strategies

---

## 10. Monitoring, Observability & Debugging

### High-Level Guidance
Detecting, tracing, and diagnosing issues in complex systems.

### What to Know
- Metrics, logs, traces
- Prometheus, Grafana
- Distributed tracing (Jaeger, Zipkin)
- Health checks & alerting

---

## 11. Practical Design Patterns

### High-Level Guidance
Reusable solutions for common distributed system problems.

### What to Know
- Circuit Breaker
- Bulkhead
- Retry & Backoff
- Leader Election
- Saga Pattern

---
