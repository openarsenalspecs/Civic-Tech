# BuildOracle

**BuildOracle — Where Cities Plan Smarter.**

BuildOracle is an open-source AI-powered zoning, environmental simulation, and development compliance platform that evaluates the full impact of proposed building projects before approval. It combines legal reasoning, blueprint analysis, environmental modeling, infrastructure forecasting, and economic impact analysis into a single unified system for urban planning decisions.

---

## 🚀 Core Features

### 🏛️ AI Zoning & Legal Compliance Engine
- Parses municipal, state, and federal zoning codes
- Converts legal text into structured, machine-readable rules
- Detects zoning violations automatically
- Supports overlays (historic districts, flood zones, environmental protection zones)
- Maintains jurisdiction-specific rule separation

---

### 🏗️ Blueprint & Building Plan Analysis
- Supports CAD, BIM (IFC), and PDF blueprint ingestion
- Extracts:
  - building height
  - footprint area
  - unit count
  - parking allocation
  - setbacks and coverage ratios
- Converts architectural plans into structured spatial datasets

---

### 🌿 Environmental Simulation System (Core Module)
- Stormwater runoff modeling (EPA SWMM integration)
- Flood risk simulation based on terrain + rainfall data
- Soil erosion and slope stability modeling
- Heat island effect simulation
- Air quality and emissions impact estimation
- Biodiversity and habitat disruption modeling
- Watershed and groundwater impact analysis

---

### 🧠 Sustainable Design Recommendation Engine
- Detects high-risk or non-compliant designs
- Recommends improvements automatically
- Prioritizes sustainable solutions:
  - green roofs
  - permeable pavement
  - bioswales and rain gardens
  - low-carbon materials
  - passive solar design
- Provides redesign alternatives with simulated outcomes

---

### 🏙️ Infrastructure Impact Modeling
- Water system demand forecasting
- Sewer capacity analysis
- Electrical grid load estimation
- Traffic congestion simulation
- School enrollment impact projection
- Emergency services capacity assessment

---

### 💰 Economic & Financial Analysis Engine
- Construction cost estimation
- Property tax revenue projection
- Local job creation modeling
- Long-term municipal ROI forecasting
- Project financial risk scoring

---

### 📊 AI Impact Reporting System
- Generates full compliance and impact reports:
  - zoning compliance summary
  - environmental impact report
  - infrastructure stress analysis
  - economic feasibility report
- Provides structured decision-ready outputs for zoning officers
- Includes violation breakdowns and mitigation pathways

---

### 🌐 Visualization & Digital Twin Layer
- 3D building rendering (Three.js)
- GIS mapping overlays (Mapbox / Deck.gl)
- Terrain visualization
- Flood and environmental simulation overlays
- City-scale digital twin support (future expansion)

---

### 🔁 Iterative Design Feedback Loop
- Developers can modify designs based on AI feedback
- Instant re-simulation of updated plans
- Before/after comparison of environmental and zoning impact
- Continuous optimization toward compliance and sustainability

---

## 🧩 System Architecture

BuildOracle is designed as a modular system:

- **Core Orchestrator Module**
- **Zoning & Compliance Module**
- **Blueprint Analysis Module**
- **Environmental Simulation Module**
- **Sustainable Recommendation Module**
- **Infrastructure Modeling Module**
- **Economic Analysis Module**
- **Reporting Module**
- **Visualization Module**

Each module operates independently and communicates through shared data pipelines and APIs.

---

## ⚙️ Tech Stack

### AI & Reasoning
- LLaMA 3 / Mistral (legal + reasoning models)
- LangChain (multi-step reasoning workflows)
- Haystack (document retrieval)

### Blueprint & Vision
- OpenCV
- Detectron2
- PyTorch
- IFC / BIM parsing libraries

### GIS & Spatial Systems
- PostGIS
- QGIS
- GeoServer
- OpenStreetMap
- Mapbox GL

### Environmental Simulation
- EPA SWMM (stormwater modeling)
- GRASS GIS
- HydroMT
- Climate, soil, and hydrology datasets

### Backend
- Python
- FastAPI
- PostgreSQL
- GraphQL
- Redis

### Frontend & Visualization
- React
- Next.js
- Deck.gl
- Three.js

### Data Pipelines
- Apache Kafka
- Apache Airflow

---

## 🧠 Design Principles

- **Transparency First** — every decision is traceable to rules or data
- **Modularity** — every system component is replaceable
- **Jurisdiction Flexibility** — supports multi-level governance
- **Explainable AI** — no black-box approvals
- **Sustainability Priority** — environmental mitigation is always recommended first

---

## 🌍 Mission

To modernize urban planning by creating a transparent, AI-assisted system that helps cities evaluate environmental, economic, and infrastructural impact before construction begins.

---

## License & Notice Requirements

BuildOracle is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
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

---

## 🔗 BuildOracle

**Where Cities Plan Smarter.**
