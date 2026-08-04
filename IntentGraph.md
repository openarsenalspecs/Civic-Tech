# IntentGraph

**Expose the Intent. Protect the User.**

IntentGraph is an open-source AI-powered privacy intelligence system that detects cookies, trackers, and hidden data-sharing behaviors across the web, then explains their origin, purpose, and risk in plain language.

Instead of simply blocking tracking, IntentGraph maps it—turning invisible data flows into understandable, auditable structures.

---

## 🚀 Features

### 🔍 Core Detection & Tracking Analysis
- Real-time detection of cookies (first-party and third-party)
- Detection of tracking scripts, pixels, and beacons
- Identification of storage-based tracking (localStorage, sessionStorage, IndexedDB)
- Network request interception tied to tracking behavior
- Cross-site tracking detection
- Identity synchronization detection across domains
- Detection of fingerprinting signals (canvas, audio, entropy-based methods)

---

### 🧠 AI Intent Engine
- AI-based classification of tracker intent (ads, analytics, identity sync, essential, etc.)
- Behavioral inference from runtime web activity
- Detection of discrepancies between declared and actual behavior
- Confidence scoring for intent classification
- Continuous rule-based + ML hybrid evaluation system
- Explainable AI outputs for every detected tracker

---

### 🌐 Tracker Origin & Supply Chain Mapping
- Full lineage tracing of cookies and trackers
- Visualization of third-party data flows
- Ad-tech and analytics ecosystem mapping
- Detection of data broker relationships
- Cross-domain identity linking graph
- Tracker ecosystem clustering

---

### 📊 Privacy Policy vs Reality Analysis
- NLP parsing of privacy policies
- Comparison between stated policy and actual behavior
- Detection of undisclosed third-party sharing
- Summarization of legal language into plain English
- Highlighting of misleading consent claims

---

### ⚖️ Risk Scoring Engine
- Per-cookie risk scoring (0–100)
- Domain-level privacy risk evaluation
- Persistence analysis (session vs long-term tracking)
- Severity classification (low, medium, high, critical)
- Transparent explanations for all risk scores

---

### 🧭 User Explanation Layer
- Plain-language explanations for all tracking behavior
- Beginner and advanced explanation modes
- Context-aware privacy warnings
- “What this means” summaries for non-technical users

---

### 🗺️ Visualization Engine
- Interactive tracker relationship graphs (D3.js)
- Cookie lineage trees
- Cross-domain identity maps
- Real-time tracking activity visualization
- Session-based tracking timelines

---

### 📤 Reporting & Export
- Exportable privacy reports (JSON, Markdown, PDF-ready)
- Website-specific “Data Exposure Reports”
- Cross-site tracking audit logs
- Developer-friendly machine-readable outputs
- Research-ready datasets (opt-in only)

---

### 🛡️ Privacy-First Architecture
- Fully local-first processing by default
- No required cloud APIs
- Optional anonymized research mode
- Encrypted local audit logs
- Offline-capable operation

---

### 🔧 Developer & Open Source Features
- Modular plugin architecture for detection rules
- Open rule sets for tracker classification
- GitLab CI/CD pipeline ready
- Fully documented internal API
- Reproducible analysis engine
- AGPL-3.0+ compliant open-source structure

---

## ⚙️ Tech Stack

### Browser Extension Layer
- TypeScript
- React
- Vite
- Manifest V3 (Chromium)
- WebExtensions API (Firefox support)
- D3.js visualization layer

### AI & Analysis Engine
- Python 3.12+
- FastAPI
- ONNX Runtime (local inference)
- spaCy / Transformers (NLP policy analysis)
- Scikit-learn (baseline models)

### High-Performance Core
- Rust (tracking detection engine)
- Tokio async runtime
- WebAssembly modules
- Serde serialization

### Data & Storage
- SQLite (default local database)
- DuckDB (advanced analytics mode)
- JSONL event logs
- Optional encrypted storage layer (SQLCipher)

### Visualization
- D3.js
- Sigma.js (large graph rendering)
- Canvas/WebGL rendering support

---

## 🧭 Philosophy

IntentGraph is built on three principles:

- **Transparency over obscurity**
- **Understanding over blocking**
- **User control over silent consent**

The goal is not to break the web, but to make it understandable.

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
  - [https://roxanneardary.com/intentgraph/](https://roxanneardary.com/intentgraph/)

---

## 📄 License & Notice Requirements

IntentGraph is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
