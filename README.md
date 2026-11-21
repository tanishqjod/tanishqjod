<div align="center">

# Tanishq Gupta
### Founder & Principal Systems Architect · Shyvora Global Technologies

**Distributed systems · Low-latency infrastructure · Cloud platforms**

[![Website](https://img.shields.io/badge/Website-shyvoraglobal.in-00E599?style=flat-square&logo=googlechrome&logoColor=white)](https://shyvoraglobal.in)
[![Email](https://img.shields.io/badge/Email-Get%20in%20touch-EA4335?style=flat-square&logo=gmail&logoColor=white)](mailto:tanishq@shyvoraglobal.in)
[![Consulting](https://img.shields.io/badge/Consulting-Available-6C63FF?style=flat-square)](mailto:tanishq@shyvoraglobal.in)

*I design and build resilient backend systems, real-time data pipelines, and cloud infrastructure—with a focus on predictable performance and operational clarity.*

</div>

---

## About

I’m the founder and principal systems architect at [Shyvora Global Technologies](https://shyvoraglobal.in). My work spans low-latency market-data systems, high-throughput event processing, and cloud-native platforms.

I care about **mechanical sympathy, bounded resource usage, fault isolation, and measurable performance**. I aim to make systems fast when things are going well—and dependable when they aren’t.

- **Focus:** distributed systems, streaming, real-time analytics, backend architecture, and infrastructure
- **Languages:** Go, Rust, Python, TypeScript, C++, and C
- **Open to:** consulting, architecture engagements, performance work, and technical advisory

## Selected work

### Shyvora XAU God · Real-time market analytics
A market-data and visualization terminal built around order-book aggregation and in-browser analysis.

- WebSocket market-depth processing and order-flow analytics
- DuckDB-Wasm for client-side analytical queries
- WebGPU-based depth visualization
- Project-reported benchmarks include sub-25 ms order-book processing and analysis of 10M+ ticks in memory

[Visit Shyvora Global](https://shyvoraglobal.in)

### Distributed event processing
A fault-tolerant streaming architecture for high-volume event workloads.

- Kafka and NATS JetStream pipelines with partitioned processing
- Backpressure and consumer-group rebalancing
- Snapshot-based recovery and operational monitoring
- Project-reported throughput: 100,000+ messages per second, with sub-50 ms p99 latency

### Cloud-native infrastructure
Deployment patterns and infrastructure automation for resilient containerized services.

- Kubernetes, Docker, Helm, and Terraform
- Network isolation, health checks, and rolling deployments
- Prometheus metrics and container resource diagnostics

## Engineering notes

The figures below are project-reported results; actual performance depends on workload and test environment.

| Area | Reported result | Approach |
| --- | ---: | --- |
| Market-data processing | `< 24.8 ms` p99 | Preallocated buffers and memory reuse |
| Event streaming | `100,000+ msgs/sec` | Partitioned Kafka/NATS processing |
| Client-side analytics | `> 1M rows/sec` | DuckDB-Wasm |
| Circuit-breaker response | `14.2 ms` | Sliding-window threshold detection |
| Soak testing | `12 hours` | Automated test and memory monitoring |

## Tools I work with

**Languages**  Go · Rust · Python · TypeScript · C++ · C  
**Streaming & APIs**  Kafka · NATS JetStream · gRPC · Protocol Buffers · WebSockets · ZeroMQ  
**Data**  ClickHouse · DuckDB · PostgreSQL · Redis · TimescaleDB  
**Cloud & operations**  Kubernetes · Docker · Helm · AWS · GCP · Terraform · OpenTelemetry · Prometheus · Grafana

## Connect

- **Email:** [tanishq@shyvoraglobal.in](mailto:tanishq@shyvoraglobal.in)
- **Website:** [shyvoraglobal.in](https://shyvoraglobal.in)
- **Consulting:** Available for architecture, performance, and cloud infrastructure engagements
- **Timezone:** IST (UTC+5:30)

<div align="center">

<sub>Built with a focus on systems that stay predictable under pressure.</sub>

</div>
