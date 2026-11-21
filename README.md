<div align="center">

# ⚡ Tanishq Gupta (`tanishqjod`)
### **Founder & Principal Systems Architect** | **Distributed Systems · Low-Latency Infrastructure · Cloud Platforms**

[![Website](https://img.shields.io/badge/Website-shyvoraglobal.in-00E599?style=for-the-badge&logo=googlechrome&logoColor=white)](https://shyvoraglobal.in)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Tanishq_Gupta-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/)
[![Email](https://img.shields.io/badge/Email-tanishq@shyvoraglobal.in-EA4335?style=for-the-badge&logo=gmail&logoColor=white)](mailto:tanishq@shyvoraglobal.in)
[![Contracts](https://img.shields.io/badge/Consulting-%2490%2Fhr%20USD-FFB800?style=for-the-badge&logo=cashapp&logoColor=black)](mailto:tanishq@shyvoraglobal.in)

```rust
const ARCHITECT: Engineer = Engineer {
    name: "Tanishq Gupta",
    role: "Founder & Principal Systems Architect @ Shyvora Global",
    core_focus: ["High-Throughput Streaming", "Sub-25ms Orderbooks", "Zero-GC Pipelines"],
    primary_runtime: ["Go", "Rust", "Python", "TypeScript", "C++"],
    infrastructure: ["Kubernetes", "Kafka", "ClickHouse", "DuckDB-Wasm", "Docker", "AWS/GCP"],
    motto: "If it pauses for Garbage Collection under news volatility, it is broken.",
};
```

---

</div>

## 📌 Executive Summary

I architect and bulletproof distributed systems and mission-critical financial backend engines designed to withstand extreme market volatility and high-concurrency bursts. 

As **Founder & Principal Systems Architect at [Shyvora Global Technologies](https://shyvoraglobal.in)**, I build sovereign low-latency execution engines, high-throughput event buses, and zero-downtime distributed storage layers. My engineering philosophy centers on **mechanical sympathy, zero-allocation data structures, deterministic latency boundaries, and rigorous fault isolation**.

- 🚀 **Flagship Terminal**: Engineered **Shyvora XAU God** — sub-25ms WebSocket L2 market depth engine with in-browser DuckDB-Wasm analytics (>1M rows/s) and WebGPU orderflow visualization.
- ⚡ **Scale & Throughput**: Built reactive Kafka & NATS JetStream event streaming platforms sustaining **100,000+ msgs/sec** with sub-50ms p99 latencies.
- 🛡️ **Zero-GC & High Resilience**: Engineered zero-allocation memory buffers (`Float64Array` typed byte slabs) and automated 14.2ms sliding-window circuit breakers certified over a **12-hour soak audit with zero memory leaks**.
- 💼 **Available For**: High-impact remote consulting retainers ($90/hr USD | 20 hrs/wk), Principal Backend Architectures, and Advisory.

---

## 🏗️ Systems Architecture Blueprint: The Zero-GC Orderbook Engine

```mermaid
flowchart LR
    subgraph INGESTION ["1. Ingestion Tier"]
        WS["WebSocket / FIX 4.4 Feed<br/>(L2 BBO & Depth Ticks)"] --> RING["Circular Ring Buffer<br/>(Disruptor Pattern)"]
    end

    subgraph ENGINE ["2. Core Microstructure Engine"]
        RING --> SLAB["Pre-Allocated Memory Slabs<br/>(Zero-GC Float64Array)"]
        SLAB --> CB["14.2ms Sliding-Window<br/>Risk Circuit Breaker"]
        CB --> MATCH["L2 Delta Book & CVD Aggregator<br/>(Sub-25ms E2E)"]
    end

    subgraph DISTRIBUTION ["3. Telemetry & Analytics"]
        MATCH --> DUCK["DuckDB-Wasm OLAP<br/>(>1,000,000 rows/sec)"]
        MATCH --> GPU["WebGPU Shaders<br/>(120 FPS Depth Heatmap)"]
        MATCH --> KAFKA["Kafka / ClickHouse<br/>(Immutable Audit Ledger)"]
    end

    classDef primary fill:#1e1e2e,stroke:#00E599,stroke-width:2px,color:#fff;
    classDef secondary fill:#181825,stroke:#89b4fa,stroke-width:1px,color:#fff;
    class WS,RING,SLAB,CB,MATCH,DUCK,GPU,KAFKA primary;
```

---

## 📊 Quantitative Benchmarks & Production Proof

| Performance Metric | Traditional Microservices Stack | Shyvora Sovereign Architecture | Engineering Mechanism |
| :--- | :---: | :---: | :--- |
| **P99 Ingestion Latency** | `120ms – 400ms` (GC spikes) | **`< 24.8ms`** | Zero-allocation byte slabs & memory reuse |
| **Client-Side Analytical OLAP** | `Server roundtrip (>850ms)` | **`> 1,000,000 rows/sec`** | In-browser DuckDB-Wasm integration |
| **Risk Circuit Breaker Trip** | `Manual / 1500ms+` | **`14.2ms`** | Sliding-window automated threshold tripwire |
| **Test Coverage & Integrity** | Ad-hoc unit tests | **164 Passing Test Suites** | Full regression, concurrency, & soak harness |
| **Memory Leak Soak Audit** | Uncontrolled RSS drift | **0 KB leak over 12-hr soak** | Deterministic buffer pooling & static bounds |

---

## 🛠️ Technology Stack & Competencies

```
Systems & Languages    :: Go (Golang) · Rust · Python · TypeScript · C++ · Modern C
Event Streaming & IPC  :: Apache Kafka · NATS JetStream · gRPC · Protocol Buffers · WebSockets · ZeroMQ
Databases & Storage    :: ClickHouse · DuckDB / DuckDB-Wasm · PostgreSQL · Redis (Lua) · TimescaleDB
Cloud & Infrastructure :: Kubernetes (K8s) · Docker · Helm · AWS (EKS, VPC, S3) · GCP · Terraform
Observability & Ops    :: OpenTelemetry · Prometheus · Grafana · Distributed Tracing (Jaeger) · eBPF
Protocols & Standards  :: FIX 4.4 · L2/L3 Orderbooks · TCP/UDP Socket Optimization · HTTP/2
```

---

## 🚀 Featured Engineering Projects

### 👑 [Shyvora XAU God — Sovereign Trading Engine](https://shyvoraglobal.in)
> **Institutional Gold Microstructure & Real-Time Telemetry Terminal**
* Sub-25ms L2 orderbook aggregation with zero-allocation Float64Array ring buffers.
* Real-time Cumulative Volume Delta (CVD), orderflow delta heatmap rendered via WebGPU at 120 FPS.
* Client-side DuckDB-Wasm queries analyzing 10M+ ticks in-memory with complete data privacy.
* Validated with 164 automated test suites and a certified 12-hour zero-memory-leak soak test.

### 🌐 High-Throughput Distributed Event Engine
> **Fault-Tolerant Distributed Message Broker & Processing Pipeline**
* Partitioned event stream handling 100,000+ requests/sec utilizing consistent hashing partitions.
* Implemented credit-based backpressure flow control to eliminate consumer buffer overflow.
* Dynamic consumer group partition rebalancing with fault-tolerant state snapshot recovery.

### ☸️ Cloud-Native VPC Topologies & Kubernetes Operators
> **Automated Sovereign Deployment & Multi-Region VPC Isolation**
* Tailored Infrastructure-as-Code for self-hosted sovereign container deployments.
* Hardened network isolation policies, automated health probes, and zero-downtime rolling upgrades.
* Prometheus metrics exporters profiling container cgroup CPU/memory pressure and socket bottlenecks.

---

## 📈 GitHub Activity & Engineering Telemetry

<div align="center">

<img src="https://github-readme-stats.vercel.app/api?username=tanishqjod&show_icons=true&theme=tokyonight&hide_border=true&count_private=true" width="48%" />
<img src="https://github-readme-stats.vercel.app/api/top-langs/?username=tanishqjod&layout=compact&theme=tokyonight&hide_border=true" width="48%" />

<br/>

<img src="https://github-readme-streak-stats.herokuapp.com/?user=tanishqjod&theme=tokyonight&hide_border=true" width="96%" />

</div>

---

## 💬 Let's Connect & Collaborate

- 💼 **Consulting & Retainers**: Available for high-impact contracts ($90/hr USD) — distributed backend architecture, performance tuning, and cloud migrations.
- 🏢 **Enterprise Inquiries**: [tanishq@shyvoraglobal.in](mailto:tanishq@shyvoraglobal.in)
- 🌐 **Company**: [Shyvora Global Technologies](https://shyvoraglobal.in)
- 📍 **Timezone**: IST (UTC +5:30) with seamless 4+ hour daily overlap with US EST/PST and European market hours.

<div align="center">
<sub>Designed & Architected by <strong>Tanishq Gupta</strong> • Founder & Principal Systems Architect</sub>
</div>
