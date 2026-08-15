# Go Distributed Lab

> Learning distributed systems by building production-ready systems from scratch in Go.

## Vision

This organization documents my journey of learning distributed systems through implementation rather than theory.

Every concept is built as a production-style Go project with benchmarks, comprehensive documentation, Docker support, CI/CD, architecture diagrams, and documented engineering trade-offs.

---

## Roadmap

### Level 1 — Go Concurrency & Foundations

- [x] **[Worker Pool](https://github.com/go-distributed-lab/go-worker-pool)** — Concurrent job processing with retries, dead-letter queues, context cancellation, and graceful shutdown.
- [x] **[Rate Limiter](https://github.com/go-distributed-lab/go-rate-limiter)** — Token Bucket, Leaky Bucket, Fixed Window, and Sliding Window implementations behind a common interface with HTTP middleware.
- [x] **[Cache](https://github.com/go-distributed-lab/go-cache)** — Generic in-memory cache implementing LRU, LFU, FIFO, TTL, and Sharded LRU with benchmarks and an optional HTTP API.

### Level 2 — Backend Infrastructure

- [x] **[Message Queue](https://github.com/go-distributed-lab/go-message-queue)** — In-memory broker supporting topics, retries, acknowledgements, dead-letter queues, metrics, backpressure, and HTTP APIs.
- [x] **[Load Balancer](https://github.com/go-distributed-lab/go-load-balancer)** — Layer-7 HTTP reverse proxy supporting Round Robin, Weighted Round Robin, Least Connections, Random, IP Hash, health checks, runtime backend management, and graceful shutdown.
- [ ] API Gateway
- [ ] Circuit Breaker

### Level 3 — Distributed Systems

- [ ] Service Discovery
- [ ] Distributed Lock
- [ ] Consistent Hashing
- [ ] Bloom Filter
- [ ] Distributed Cache

### Level 4 — Consensus & Coordination

- [ ] Raft

---

## Completed Projects

| Project | Concepts | Status |
|---------|----------|--------|
| [go-worker-pool](https://github.com/go-distributed-lab/go-worker-pool) | Goroutines, Channels, WaitGroups, Retry, Dead-Letter Queue, Graceful Shutdown | ✅ Complete |
| [go-rate-limiter](https://github.com/go-distributed-lab/go-rate-limiter) | Token Bucket, Leaky Bucket, Fixed Window, Sliding Window, HTTP Middleware, Atomic Metrics | ✅ Complete |
| [go-cache](https://github.com/go-distributed-lab/go-cache) | LRU, LFU, FIFO, TTL, Sharded Cache, Go Generics, Thread Safety, HTTP API | ✅ Complete |
| [go-message-queue](https://github.com/go-distributed-lab/go-message-queue) | Pub/Sub, Broker, Topics, Acknowledgements, Retry, Dead-Letter Queue, Backpressure, HTTP API | ✅ Complete |
| [go-load-balancer](https://github.com/go-distributed-lab/go-load-balancer) | Reverse Proxy, Round Robin, Weighted RR, Least Connections, Random, IP Hash, Health Checks, Runtime Backend Management | ✅ Complete |

---

## Repository Standards

Every repository in this organization aims to include:

- 🏗️ Architecture Diagrams
- 🐳 Docker Support
- 📊 Benchmarks & Performance Analysis
- ✅ Unit & Integration Tests
- 📚 Comprehensive Documentation
- 🔄 CI/CD Pipeline
- 🧪 Race Detection & Static Analysis
- 🎥 Demo / Usage Examples
- ⚖️ Design Decisions & Trade-offs

---

## Engineering Approach

Each project follows the same engineering process:

1. Understand the production problem and real-world use cases.
2. Study the underlying algorithms and system design concepts.
3. Design the architecture, APIs, and package boundaries.
4. Implement the system from scratch using Go's standard library whenever possible.
5. Validate correctness with comprehensive tests and Go's race detector.
6. Benchmark throughput, latency, memory usage, and allocations.
7. Analyze performance characteristics and engineering trade-offs.
8. Document the implementation with architecture diagrams and usage examples.

---

## Current Progress

```text
✅ Worker Pool
        │
        ▼
✅ Rate Limiter
        │
        ▼
✅ Cache
        │
        ▼
✅ Message Queue
        │
        ▼
✅ Load Balancer
        │
        ▼
⬜ API Gateway
        │
        ▼
⬜ Circuit Breaker
        │
        ▼
⬜ Service Discovery
        │
        ▼
⬜ Distributed Lock
        │
        ▼
⬜ Consistent Hashing
        │
        ▼
⬜ Distributed Cache
        │
        ▼
⬜ Raft
```

---

## Principles

Across every repository, I aim to:

- Build from first principles using Go's standard library whenever practical.
- Understand the algorithms before writing code.
- Measure performance with benchmarks instead of assumptions.
- Design reusable, interface-driven components.
- Document implementation details, trade-offs, and architectural decisions.
- Prioritize correctness, simplicity, and maintainability over unnecessary abstraction.

---

## Long-Term Goal

Build a collection of production-quality Go implementations of the core building blocks behind modern backend and distributed systems.

As the collection grows, these libraries will be composed together to build larger distributed systems, demonstrating how production infrastructure is engineered from reusable components while documenting the reasoning, trade-offs, and performance characteristics behind every design decision.
