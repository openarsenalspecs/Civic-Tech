# Sapient Eval

**Empirical benchmarking for synthetic minds.**

Sapient Eval is an open-source, AGPL-3.0+ compliant benchmarking framework for evaluating locally hosted and remotely served AI systems across accuracy, speed, efficiency, and reasoning quality. It provides a modular, spec-driven evaluation architecture designed to standardize how AI performance is measured across industries and model types.

---

## Features

### 🧠 Modular Benchmark Engine
A flexible evaluation core that executes standardized or fully custom benchmark pipelines. Every component of the system is replaceable, extensible, and designed for research-grade reproducibility.

---

### 📊 Industry Spec System (BMS)
Define structured evaluation environments using a YAML-based Benchmark Specification system.

- Industry-specific benchmark definitions (legal, finance, healthcare, engineering, general)
- Configurable task categories and evaluation rules
- Weighted scoring models per domain
- Constraint definitions (latency, tokens, tools, etc.)
- Fully shareable and versioned spec files

---

### 🔌 Universal Model Adapter Layer
Connect any AI system through a standardized interface.

- Local model support (Ollama, llama.cpp, vLLM, etc.)
- HTTP/API-based models
- GPU server deployments
- Plugin-based adapter architecture
- Multi-model orchestration and comparison support

---

### ⚖️ Multi-Dimensional Scoring System
Evaluates models across multiple measurable dimensions.

- Accuracy scoring (exact match + semantic similarity)
- Reasoning quality evaluation
- Latency and throughput tracking
- Token efficiency measurement
- Resource usage (CPU/GPU/memory estimation)
- Custom weighted scoring formulas per benchmark spec

---

### 🧪 Reproducible Benchmark Execution
Ensures every test run is consistent and auditable.

- Deterministic execution controls (seed locking)
- Versioned datasets and benchmark packs
- Re-runnable evaluation pipelines
- Regression testing across model versions
- Fully traceable evaluation logs

---

### 🔁 Model Comparison Engine
Compare multiple models under identical evaluation conditions.

- Side-by-side model benchmarking
- Task-level performance breakdowns
- Historical performance tracking
- Regression detection between model versions
- Leaderboard generation per industry or category

---

### 📦 Benchmark Registry System
A structured ecosystem for reusable and shareable benchmarks.

- Community-contributed benchmark packs
- Version-controlled datasets
- Industry-specific benchmark libraries
- Local or distributed registry support
- Optional synthetic dataset generation tools

---

### 🧩 Task Execution Framework
Supports diverse AI evaluation workloads.

- Question answering benchmarks
- Structured extraction tasks
- Multi-step reasoning challenges
- Code generation + validation
- Agent/tool-use simulation testing
- Rubric-based evaluation tasks

---

### 📈 Reporting & Visualization Layer
Transforms benchmark results into actionable insights.

- JSON, Markdown, and HTML report generation
- Performance dashboards
- Speed vs accuracy visualizations
- Task-level breakdown analytics
- CI/CD exportable reports

---

### 🧠 LLM-as-Judge Evaluation Module (Optional)
Advanced evaluation mode for subjective or complex outputs.

- Configurable judge models
- Rubric-based scoring systems
- Multi-judge consensus evaluation
- Bias-control configuration options
- Fully optional and replaceable scoring layer

---

### ⚡ Local-First Architecture
Designed for offline-first and self-hosted environments.

- No cloud dependency required
- Fully local inference benchmarking support
- Secure execution environments
- Air-gapped deployment capability
- Private dataset support

---

### 🔄 Continuous Benchmarking Integration
Integrates directly into development workflows.

- CI/CD pipeline support
- Automated regression detection
- Scheduled benchmark execution
- Model update tracking
- Performance drift alerts

---

### 🧱 Plugin-Based Extensibility
Extend Sapient Eval without modifying the core system.

- Custom evaluation modules
- Custom scoring functions
- New model adapters
- Industry-specific benchmark packs
- External tool integrations

---

### 🌐 Open Evaluation Standard
Built as a transparent and reproducible AI evaluation framework.

- Fully open benchmark specification format
- Transparent scoring logic
- No hidden ranking mechanisms
- Community-driven benchmark evolution
- AGPL-3.0+ enforced openness

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
  - [https://roxanneardary.com/sapient-eval/](https://roxanneardary.com/sapient-eval/)  

---

## License & Notice Requirements

Sapient Eval is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, refer to the AGPL-3.0+ license and the project's `notice.md` file.
