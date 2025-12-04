# 📬 Messaging Systems

---

## 1. Messaging Fundamentals

### High-Level Guidance
Messaging systems decouple producers and consumers to enable asynchronous communication and scalability.

### What to Know
- Message queues vs topics
- Synchronous vs asynchronous communication
- Pub/Sub vs Point-to-Point
- Benefits: decoupling, fault tolerance, load leveling

---

## 2. Kafka

### High-Level Guidance
Distributed streaming platform for high-throughput, fault-tolerant messaging.

### What to Know
- Topics, partitions, and offsets
- Producers and consumers
- Consumer groups for parallel processing
- Exactly-once vs at-least-once vs at-most-once delivery
- Kafka Streams for processing data in real-time

### Practical Usage
- Event-driven microservices
- Audit logs and analytics pipelines

---

## 3. RabbitMQ

### High-Level Guidance
Broker-based message queue system for reliable messaging.

### What to Know
- Queues, exchanges (direct, fanout, topic, headers)
- Routing keys and bindings
- Acknowledgements and durable queues
- Publisher confirms

### Practical Usage
- Task queues
- Asynchronous processing in Spring Boot
- RPC over messaging

---

## 4. ActiveMQ / JMS (Java Messaging Service)

### High-Level Guidance
Standard API for message-oriented middleware in Java.

### What to Know
- Point-to-point (queues) vs publish-subscribe (topics)
- Message selectors
- Durable vs non-durable subscriptions
- Transactions and acknowledgements

### Practical Usage
- Legacy enterprise integration
- Decoupling systems within Java ecosystem

---

## 5. Key Concepts

### Delivery Semantics
- **At-most-once**: message may be lost
- **At-least-once**: message may be duplicated
- **Exactly-once**: message processed once (hardest)

### Idempotency
- Critical for ensuring safe retries in distributed systems

### Dead Letter Queues (DLQ)
- Store messages that cannot be processed
- Useful for retries and debugging

---

## 6. Tradeoffs & Considerations

### Performance
- Kafka → high throughput, lower latency
- RabbitMQ → reliability, rich routing

### Ordering Guarantees
- Kafka → per-partition ordering
- RabbitMQ → per-queue ordering

### Scalability
- Kafka → distributed by design
- RabbitMQ → clustering and federation

---

## 7. Practical Tips for Spring Integration

- Use `spring-kafka` or `spring-rabbit` for simplified config
- Prefer asynchronous consumers for scalability
- Handle retries and DLQs
- Monitor offsets, consumer lag, and queue depth

---
