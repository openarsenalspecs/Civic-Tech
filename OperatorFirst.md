# OperatorFirst

**See what your systems actually experience.**

OperatorFirst is an open-source, self-hosted observability platform designed for operators who need verifiable truth from their infrastructure. It uses distributed probe networks, cryptographically signed results, and consensus-based validation to provide monitoring that is transparent, auditable, and operator-owned.

---

## Why OperatorFirst

Traditional monitoring tools rely on centralized systems, black-box logic, and unverifiable results. OperatorFirst replaces trust with proof.

Instead of asking “Is it up?”, OperatorFirst helps you answer:
**“What is each part of my system actually experiencing right now?”**

---

## Core Principles

- **Operator Ownership** – You control the entire monitoring stack  
- **Verifiable Data** – Every result is signed and auditable  
- **Distributed Reality** – Multiple probes validate system state  
- **No Black Boxes** – Everything is inspectable and reproducible  
- **GitOps-Native** – Monitoring defined as code  

---

## Features

### 1. Core Monitoring Platform
- Self-hosted control plane (Docker / Kubernetes / bare metal)
- Distributed probe network across edge, cloud, and on-prem environments
- Multi-protocol checks (HTTP, DNS, TCP, TLS, ICMP, gRPC, WebSockets)
- Real browser synthetic monitoring with full user journey simulation

### 2. Distributed Truth System
- Multi-region probe execution
- Consensus-based outage detection (quorum models)
- Cross-region experience comparison
- Probe mesh architecture for scalable global coverage

### 3. Cryptographic Verification Layer
- Signed probe results (tamper-evident monitoring data)
- Append-only evidence log
- Replayable historical system states
- Verifiable uptime history

### 4. Monitoring as Code (GitOps-Native)
- YAML-based declarative check definitions
- Git versioned monitoring configuration
- Automatic deployment via scheduler
- Environment-specific monitoring rules

### 5. Scheduling & Execution Engine
- Distributed job scheduling system
- Queue-based execution (NATS / Kafka / Redis Streams)
- Load-balanced probe assignment
- Dynamic scaling across probe nodes

### 6. Event Correlation & Root Cause Engine
- Cross-signal correlation (DNS, latency, TLS, HTTP failures)
- Incident timeline reconstruction
- Baseline anomaly detection
- Root cause inference for system-level insights

### 7. Plugin Ecosystem (Extensibility Layer)
- WASM-based sandboxed plugin runtime
- Multi-language SDK support (Rust, Go, TypeScript, WASM)
- Custom checks for APIs, databases, queues, and protocols
- Hot-reloadable plugins with versioning and canary execution
- Secure execution model with resource limits and capability control

### 8. Storage & Evidence System
- High-performance time-series storage (ClickHouse)
- Metadata and configuration storage (PostgreSQL)
- Immutable object storage for raw evidence (screenshots, logs, traces)
- Full incident replay capability

### 9. Alerting & Integrations
- Pluggable alerting system (Slack, email, webhooks, PagerDuty, etc.)
- Noise reduction via correlation filtering
- Severity scoring and prioritization engine

### 10. Operator Experience Layer
- Real-time incident dashboard
- Blast radius visualization
- Operational timeline reconstruction
- Drift detection and early warning signals

### 11. Federated & Scalable Architecture
- Multi-cluster federation support
- Edge-native lightweight probes
- Self-healing probe networks
- High availability control plane

### 12. Privacy & Sovereignty Features
- Fully self-hosted deployment
- Air-gapped mode support
- No vendor telemetry
- Full data ownership guarantees

### 13. API & Developer Platform
- REST and gRPC APIs
- WebSocket streaming for real-time events
- Programmatic check management
- Exportable metrics (Prometheus / OpenTelemetry-compatible)

### 14. Advanced Features
- Reality replay engine for historical reconstruction
- Internet experience mapping across regions
- Multi-signal incident intelligence
- Predictive degradation detection (future extension)

---

## Specification Branding License (SBL)

### Standard
- Fully AGPL-3.0+ compliant system
- Copyleft enforced for network deployments
- Required attribution:
  - Roxanne Ardary
  - https://www.roxanneardary.com/

### Optional

- **Specification Branding License (SBL)**
  - Attribution-free commercial deployment
  - Pricing based on scale, usage, and deployment scope
  - [https://roxanneardary.com/operatorfirst/](https://roxanneardary.com/operatorfirst/)

---

## License & Notice Requirements

OperatorFirst is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- OperatorFirst specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's `notice.md` file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
