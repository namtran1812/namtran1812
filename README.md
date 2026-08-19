<div align="center">

# hey, i'm nam 👋

**cs + economics @ university of florida**

i like building things close to the systems layer — especially **trading infrastructure, databases, compilers, distributed systems, and performance tooling**.

most of my projects start with some version of the same question:
*what's actually happening underneath the abstraction?*

<a href="https://www.linkedin.com/in/nam2k5/">linkedin</a> · <a href="mailto:trannam18122005@gmail.com">email</a> · <a href="https://nemtranhoang.vercel.app/">website</a> · <a href="https://github.com/namtran1812">github</a>

</div>

<br>

## open source ᯓ★

> contributing to production systems + learning how large codebases think about performance, correctness, and hardware.

**[nvidia · nccl](https://github.com/namtran1812/nccl)**
`c++` · `cuda` · `gpu systems`

worked on blackwell collective performance + p2p diagnostics, including a geometry-aware reducescatter optimization that cut **4 mib bfloat16 latency ~54% on 2×b200**.

**[aws · s2n-bignum](https://github.com/namtran1812/s2n-bignum)**
`ocaml` · `hol light` · `x86-64` · `cryptography`

extended formally verified x86 semantics for timing-sensitive bit-scan instructions + added constant-time policy checks around intel doit behavior. **pr #444 · issue #361**

**[microsoft · stl](https://github.com/namtran1812/STL)**
`c++` · `standard library` · `abi`

optimized five `std::exception_ptr` operations by removing unnecessary crt call boundaries while preserving abi + ownership semantics.

**[meta · folly](https://github.com/namtran1812/folly)**
`c++` · `concurrency` · `atomics`

audited `meteredexecutor` synchronization + removed an unnecessary sequentially consistent atomic operation.

**[hudson river trading · slang-server](https://github.com/namtran1812/slang-server)**
`c++` · `systemverilog` · `lsp`

added context-aware parameter/port autocomplete + fixed call-hierarchy navigation. **212/212 tests passing.**

**[jane street · magic-trace](https://github.com/namtran1812/magic-trace)**
`ocaml` · `linux perf` · `intel pt`

added hardware-triggered intel pt range tracing + fixed multi-thread trigger and timestamp correctness issues.

<br>

## trading + financial systems 〽

### [minimatch](https://github.com/namtran1812/minimatch)

`c++20` · `boost.asio` · `sqlite` · `prometheus` · `grafana`

a small exchange stack i built to understand the full path from receiving an order to executing it — matching, smart routing, oms/ems, execution algorithms, deterministic replay, and observability.

`1m+ orders` · `~35% lower p99 matching latency`

### [mercator](https://github.com/namtran1812/mercator)

`c++23` · `python` · `kafka` · `clickhouse` · `postgresql` · `redis`

a fixed-income pricing platform for **9,500+ instruments** with dependency-aware repricing and deterministic market replay. a lot of the work went into making distributed market state behave correctly through crashes, retries, and redelivery.

`500 crash/restart tests` · `100 concurrent writers`

<br>

## systems + infrastructure ⚙

### [chronosdb](https://github.com/namtran1812/chronosdb)

`rust` · `mvcc` · `wal` · `storage engines`

a transactional database built from scratch to understand what pages, buffer management, mvcc, checkpoints, and recovery look like beyond textbook diagrams.

`~92% lower recovery latency` · `~13× speedup`

### [helix](https://github.com/namtran1812/helix)

`rust` · `ssa` · `cfg` · `sccp`

an optimizing compiler with ssa construction, dominance analysis, sparse conditional constant propagation, branch folding, unreachable-block pruning, and dead-code elimination.

`1,288/1,288 differential tests` · `76.1% fewer ir instructions`

### [aegis fabric](https://github.com/namtran1812/aegis-fabric)

`rust` · `ebpf` · `linux` · `cgroup v2`

a linux runtime for tracing scheduler behavior inside isolated workloads + measuring wake-to-run latency across processes and threads.

`p50–p99.9 telemetry` · `~0.5% runtime overhead`

### [infrastructure control plane](https://github.com/namtran1812/terraform-provider-viettelidc)

`go` · `grpc` · `postgresql` · `redis` · `prometheus`

a bounded-concurrency monitoring + reconciliation system with mtls, rbac, auditing, retries, circuit breakers, and provider inventory synchronization.

`10,000 simulated servers`

<br>

## distributed + data systems ⑂

### [tracecell](https://github.com/namtran1812/tracecell)

`typescript` · `aws lambda` · `eventbridge` · `sqs` · `dynamodb` · `s3`

an observability system for robotic fleets that reconstructs what happened even when telemetry arrives **late, twice, concurrently, or out of order**.

`10k-event aws deployment` · `32% lower p50` · `23% lower p95 investigation latency`

### [driftgraph](https://github.com/namtran1812/driftgraph)

`python` · `polars` · `parquet` · `pytorch`

a temporal reconstruction engine built around a deceptively simple question: *what exactly did the dataset look like at this point in time?*

handles late events, atomic checkpoints, stale-state invalidation, and crashes while preserving point-in-time correctness.

`~7.06m events/sec` · `7.45× throughput`

<br>

## security ⛨

### [sentrymesh](https://github.com/namtran1812/sentrymesh)

`go` · `postgresql` · `opentelemetry` · `prometheus` · `docker`

an ai security gateway for prompt injection, pii leakage, rag provenance, cross-team isolation, and approval-gated agent actions, with durable asynchronous auditing.

`~2.1k req/s` · `100% audit persistence in validated fault-injection runs`

<br>

## research + applied data ⌁

### [laborlens](https://github.com/namtran1812/laborlens)

`python` · `clickhouse` · `fastapi` · `fred/alfred` · `bls qcew` · `scikit-learn`

a labor-market research engine built around making sure an analysis only knows what was **actually known at that point in history**.

it reconstructs historical data vintages without look-ahead bias, detects multivariate labor-market regimes, and grounds generated analysis against the underlying economic data.

`98% intent accuracy` · `100% routing accuracy` · `100% causal-safety recall`

<br>

---

<div align="center">

### currently interested in

`c++` · `rust` · `linux` · `distributed systems` · `databases` · `compilers` · `gpu systems` · `trading infrastructure`

<br>

<sub>
i like systems where correctness, latency, and failure behavior can be measured rather than assumed.
</sub>

<br><br>

<a href="https://www.linkedin.com/in/nam2k5/">linkedin</a> · <a href="mailto:trannam18122005@gmail.com">email</a> · <a href="https://nemtranhoang.vercel.app/">website</a> · <a href="https://github.com/namtran1812">github</a>

</div>

