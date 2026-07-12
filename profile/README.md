# Go Distributed Lab

> Learning distributed systems by building production-ready systems from scratch in Go.

## Vision

This organization documents my journey of learning distributed systems through implementation rather than theory.

Every concept is built as a production-style Go project with benchmarks, documentation, Docker support, CI/CD, architecture diagrams, and documented engineering trade-offs.

---

## Roadmap

### Level 1 — Go Concurrency & Foundations

* [x] **[Worker Pool](https://github.com/go-distributed-lab/go-worker-pool)** — Concurrent job processing with retries, dead-letter queues, context cancellation, and graceful shutdown.
* [x] **[Rate Limiter](https://github.com/go-distributed-lab/go-rate-limiter)** — Four rate limiting algorithms behind a common interface with HTTP middleware and zero-allocation hot paths.
* [ ] Cache
* [ ] Circuit Breaker

### Level 2 — Backend Infrastructure

* [ ] Message Queue
* [ ] Load Balancer
* [ ] API Gateway

### Level 3 — Distributed Systems

* [ ] Service Discovery
* [ ] Distributed Lock
* [ ] Consistent Hashing
* [ ] Bloom Filter

### Level 4 — Consensus & Coordination

* [ ] Raft

---

## Completed Projects

| Project                                                                  | Concepts                                                                  | Status     |
| ------------------------------------------------------------------------ | ------------------------------------------------------------------------- | ---------- |
| [go-worker-pool](https://github.com/go-distributed-lab/go-worker-pool)   | Goroutines, Channels, WaitGroups, Retry, DLQ, Graceful Shutdown           | ✅ Complete |
| [go-rate-limiter](https://github.com/go-distributed-lab/go-rate-limiter) | Token Bucket, Leaky Bucket, Fixed Window, Sliding Window, HTTP Middleware | ✅ Complete |

---

## Repository Standards

Every repository in this organization aims to include:

* 🏗️ Architecture Diagrams
* 🐳 Docker Support
* 📊 Benchmarks & Performance Analysis
* ✅ Unit & Integration Tests
* 📚 Comprehensive Documentation
* 🔄 CI/CD Pipeline
* 🧪 Race Detection & Static Analysis
* 🎥 Demo / Usage Examples
* ⚖️ Design Decisions & Trade-offs

---

## Engineering Approach

Each project follows the same learning and engineering process:

1. Understand the problem and production use cases.
2. Study the underlying algorithm or system design concept.
3. Design the architecture and package boundaries.
4. Implement the core system from scratch in Go.
5. Test concurrency and correctness with Go's race detector.
6. Benchmark throughput, latency, memory, and allocations.
7. Analyze design trade-offs and performance characteristics.
8. Document the architecture and implementation decisions.

---

## Goal

Build a collection of production-quality Go implementations of the core building blocks behind modern backend and distributed systems.

The goal is not only to make each system work, but to understand **why it works, how it behaves under load, where it breaks, and the engineering trade-offs behind its design**.

