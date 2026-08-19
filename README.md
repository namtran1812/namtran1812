# Hey, I'm Nam 👋

I'm a **CS + Economics student at the University of Florida** who likes building things close to the systems layer — especially **trading infrastructure, databases, compilers, distributed systems, and performance tooling**.

I spend a lot of time figuring out what happens underneath abstractions: why something is slow, what happens when it crashes, and what assumptions actually make concurrent systems correct.

---

## 🌱 Open Source

Recently, I've been contributing to production systems and learning how large codebases approach performance, correctness, and hardware.

**[NVIDIA NCCL](https://github.com/namtran1812/nccl)** · `C++` `CUDA` `GPU Systems`
Worked on Blackwell collective performance and P2P diagnostics, including a ReduceScatter optimization that cut **4 MiB BF16 latency ~54% on 2×B200**.

**[AWS s2n-bignum](https://github.com/namtran1812/s2n-bignum)** · `OCaml` `HOL Light` `x86-64`
Extended formally verified x86 semantics for timing-sensitive bit-scan instructions and added constant-time policy checks around Intel DOIT behavior. **PR #444 · Issue #361**

**[Microsoft STL](https://github.com/namtran1812/STL)** · `C++` `Standard Library` `ABI`
Optimized five `std::exception_ptr` operations by removing unnecessary CRT call boundaries while preserving ABI and ownership semantics.

**[Meta Folly](https://github.com/namtran1812/folly)** · `C++` `Concurrency` `Atomics`
Audited `MeteredExecutor` synchronization and removed an unnecessary sequentially consistent atomic operation.

**[Hudson River Trading · slang-server](https://github.com/namtran1812/slang-server)** · `C++` `SystemVerilog` `LSP`
Added context-aware parameter/port autocomplete and fixed call-hierarchy navigation. **212/212 tests passing.**

**[Jane Street · magic-trace](https://github.com/namtran1812/magic-trace)** · `OCaml` `Linux perf` `Intel PT`
Added hardware-triggered Intel PT range tracing and fixed multi-thread trigger and timestamp correctness issues.

---

## ⚡ Trading & Financial Systems

### [MiniMatch](https://github.com/namtran1812/minimatch)

`C++20` `Boost.Asio` `SQLite` `Prometheus` `Grafana`

A small exchange stack I built to understand the full path from receiving an order to executing it: **matching, smart routing, OMS/EMS, execution algorithms, replay, and observability**.

**1M+ orders · ~35% lower p99 matching latency**

### [Mercator](https://github.com/namtran1812/mercator)

`C++23` `Python` `Kafka` `ClickHouse` `PostgreSQL` `Redis`

A fixed-income pricing platform for **9,500+ instruments**, with dependency-aware repricing and deterministic market replay. A big part of the project was making distributed state behave correctly through crashes, retries, and redelivery.

---

## ⚙️ Systems

### [ChronosDB](https://github.com/namtran1812/chronosdb)

`Rust` `MVCC` `WAL` `Storage Engines`

A transactional database I built from scratch to understand what MVCC, pages, buffer management, checkpoints, and recovery look like beyond textbook diagrams.

**~92% lower recovery latency · ~13× speedup**

### [Helix](https://github.com/namtran1812/helix)

`Rust` `SSA` `CFG` `SCCP`

An optimizing compiler with SSA construction, dominance analysis, sparse conditional constant propagation, branch folding, and dead-code elimination.

**1,288/1,288 differential tests · 76.1% fewer IR instructions**

### [Aegis Fabric](https://github.com/namtran1812/aegis-fabric)

`Rust` `eBPF` `Linux` `cgroup v2`

A Linux runtime for tracing scheduler behavior inside isolated workloads and measuring wake-to-run latency across processes and threads.

**p50–p99.9 telemetry · ~0.5% runtime overhead**

### [Infrastructure Control Plane](https://github.com/namtran1812/terraform-provider-viettelidc)

`Go` `gRPC` `PostgreSQL` `Redis` `Prometheus`

A bounded-concurrency monitoring and reconciliation system with mTLS, RBAC, auditing, retries, circuit breakers, and provider inventory synchronization.

**Tested across 10,000 simulated servers**

---

## ☁️ Distributed & Data Systems

### [TraceCell](https://github.com/namtran1812/tracecell)

`TypeScript` `AWS Lambda` `EventBridge` `SQS` `DynamoDB` `S3`

An observability system for robotic fleets that reconstructs what happened even when telemetry arrives **late, twice, concurrently, or out of order**.

**10K-event AWS deployment · 23% lower p95 investigation latency**

### [DriftGraph](https://github.com/namtran1812/driftgraph)

`Python` `Polars` `Parquet` `PyTorch`

A temporal reconstruction engine built around a deceptively simple question: *what exactly did the dataset look like at this point in time?*

Handles late events, checkpoints, stale-state invalidation, and crash recovery while preserving point-in-time correctness.

**~7.06M events/sec · 7.45× throughput improvement**

---

## 🔐 Security

### [SentryMesh](https://github.com/namtran1812/sentrymesh)

`Go` `PostgreSQL` `OpenTelemetry` `Prometheus`

An AI security gateway for prompt injection, PII leakage, RAG provenance, and approval-gated agent actions, with durable asynchronous auditing.

**~2.1K req/s · 100% audit persistence in validated fault-injection runs**

---

## 🔬 Research & Applied Data

### [LaborLens](https://github.com/namtran1812/laborlens)

`Python` `ClickHouse` `FastAPI` `FRED/ALFRED` `BLS QCEW`

A labor-market research engine built around another time problem: making sure an analysis only knows what was **actually known at that point in history**.

It reconstructs historical data vintages, detects labor-market regimes, and grounds generated analysis against the underlying economic data.

---

### What I like working on

`C++` · `Rust` · `Linux` · `Distributed Systems` · `Databases` · `Compilers` · `GPU Systems` · `Trading Infrastructure`

<sub>I like systems where correctness, latency, and failure behavior can be measured rather than assumed.</sub>

