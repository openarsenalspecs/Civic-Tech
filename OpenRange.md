# OpenRange  
## A map of real-world affordability.

OpenRange is an open source civic intelligence platform that maps the **true cost of living across every town and city in America**, and connects it to jobs, income reality, and opportunity using explainable AI.

It is built under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)** and designed as public infrastructure, not a proprietary product.

---

## 🌎 What OpenRange Does

OpenRange answers one core question:

> **Where can you actually afford to live—and what can you realistically do there?**

It combines:
- Cost of living data
- Job market intelligence
- Real income modeling
- AI-assisted budgeting
- Geographic opportunity mapping
- Full transparency + auditability

---

## 🧩 Full Modular Feature System

OpenRange is built as independent but interconnected modules:

---

### 🧩 MODULE 1 — COST OF LIVING ENGINE
- 2-bedroom rent averages (real market data)
- Housing cost modeling (rent + mortgage equivalents)
- Food and grocery cost indexing
- Utilities (electric, gas, water, internet)
- Transportation costs (gas, transit, ownership)
- Insurance (health, auto, renters)
- Local tax burden estimation
- Output: monthly cost range + confidence score

---

### 🧩 MODULE 2 — TOWN & CITY DATA LAYER
- City / ZIP / metro normalization
- Income + employment statistics
- Job density scoring
- Infrastructure access scoring (healthcare, broadband, transit)
- Standardized “Town Profile Object”

---

### 🧩 MODULE 3 — AI BUDGET & LIFE PLANNER
- Natural language budget parsing
- Household modeling (single, couple, family)
- Budget feasibility scoring
- What-if simulation engine
- Relocation viability analysis
- Output: ranked viable locations + cost breakdowns

---

### 🧩 MODULE 4 — JOB MATCHING ENGINE
- Resume + skill extraction
- Semantic job matching (embeddings)
- Local + remote job aggregation
- Salary normalization (after tax + COL adjusted)
- Job viability labeling:
  - ✅ Comfortable
  - ⚠️ Tight but viable
  - ❌ Not sustainable

---

### 🧩 MODULE 5 — OPPORTUNITY INDEX ENGINE
- Income-to-cost ratio scoring
- Job availability density
- Wage growth trends
- Housing stability indicators
- Healthcare access scoring
- Output: 0–100 Opportunity Score per location

---

### 🧩 MODULE 6 — FORECASTING ENGINE
- Rent trend prediction
- Wage growth modeling
- Inflation sensitivity analysis
- Housing volatility detection
- Models: Prophet / NeuralProphet, LightGBM

---

### 🧩 MODULE 7 — COMMUNITY REALITY LAYER
- User-reported hidden costs
- Local insights and corrections
- Seasonal cost variations
- Reputation-weighted contributions

---

### 🧩 MODULE 8 — VISUALIZATION & MAP SYSTEM
- Interactive U.S. affordability map
- Cost heatmaps
- Job density overlays
- Opportunity scoring layers
- Town comparison tool

---

### 🧩 MODULE 9 — AI ORCHESTRATION LAYER
- LLM-based query routing
- Tool chaining across modules
- Unified response generation
- Explainable AI output formatting

---

### 🧩 MODULE 10 — DATA INGESTION PIPELINE
- Airbyte ingestion system
- Scrapy-based scraping pipelines
- dbt transformations
- Great Expectations validation
- Versioned datasets

---

### 🧩 MODULE 11 — SECURITY & ETHICS LAYER
- No default user tracking
- Local-only mode support
- Encrypted optional profiles
- Transparent scoring logic
- Open documentation of all models

---

### 🧩 MODULE 12 — PUBLIC API LAYER
- `/cost/{location}`
- `/jobs/match`
- `/budget/analyze`
- `/town/{id}`
- `/opportunity/score`
- `/forecast/{location}`

---

### 🧩 MODULE 13 — REAL INCOME ENGINE
- Federal/state/local tax modeling
- Benefit deduction modeling
- Child tax credit adjustments
- Disposable income calculation
- Output: true monthly income vs survival cost

---

### 🧩 MODULE 14 — LIFE QUALITY INDEX
- Safety metrics
- Healthcare access
- Education quality
- Commute burden
- Climate risk
- Broadband access
- Output: livability score + tradeoff index

---

### 🧩 MODULE 15 — MIGRATION PATH ENGINE
- Step-by-step relocation planning
- Skill upgrade recommendations
- Income progression roadmap
- Time-to-move estimation

---

### 🧩 MODULE 16 — HOUSING REALITY LAYER
- Real listing ingestion
- Vacancy rate tracking
- Time-on-market analysis
- Neighborhood-level affordability breakdown

---

### 🧩 MODULE 17 — REMOTE WORK ENGINE
- Remote/hybrid classification
- Employer restrictions database
- Time zone compatibility scoring
- Geo-adjusted salary fairness model

---

### 🧩 MODULE 18 — ECONOMIC RISK ENGINE
- Inflation sensitivity modeling
- Housing bubble detection
- Industry concentration risk
- Economic shock simulation

---

### 🧩 MODULE 19 — HOUSEHOLD MODELING ENGINE
- Multi-person household scaling
- Childcare cost modeling
- Elder care cost integration
- School district cost impact

---

### 🧩 MODULE 20 — EXPLANATION & AUDIT LAYER
- Full decision trace generation
- Data provenance tracking
- Model transparency reporting
- “Why this result?” explanations
- Bias detection system
- Query replay system
- Counterfactual analysis engine
- Full audit export capability
- Transparency mode (show all reasoning)

---

## 🤖 AI MODEL STACK

### LLM Layer
- GPT-4o / GPT-4.1 (API option)
- LLaMA 3 (self-hosted via vLLM)
- Mistral / Mixtral (open models)

### Embeddings
- sentence-transformers (e5-large, bge-large)
- FAISS or Qdrant vector search

### ML Models
- LightGBM (cost + feasibility)
- XGBoost (job classification)
- Prophet / NeuralProphet (forecasting)

---

## 🖥️ TECH STACK

### Frontend
- Next.js (TypeScript)
- Tailwind CSS
- shadcn/ui
- Mapbox GL / Leaflet
- D3.js / ECharts

### Backend
- FastAPI (Python)
- PostgreSQL + PostGIS
- TimescaleDB
- Redis

### Data Pipeline
- Airbyte
- dbt
- Scrapy
- Great Expectations
- Airflow / Prefect

### Infrastructure
- Docker
- Kubernetes
- GitLab CI/CD
- OpenTelemetry
- Prometheus + Grafana

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
  - [https://roxanneardary.com/openrange/](https://roxanneardary.com/openrange/)

---

## 📜 License & Notice Requirements

OpenRange is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
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
