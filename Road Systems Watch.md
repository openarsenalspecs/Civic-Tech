# Road Systems Watch

*A living map of infrastructure activity.*

Road Systems Watch is an open-source civic infrastructure transparency platform that tracks, maps, and explains road construction activity across jurisdictions. It combines citizen reporting, public project data, contracting records, and AI-driven analysis to create a continuously updated system for understanding how roads are built, funded, maintained, and repeatedly repaired over time.

---

## 🧭 Overview

Road Systems Watch transforms infrastructure from static records into a **living system of activity**. Each road becomes a continuously updated profile that includes work history, funding sources, responsible agencies, and contracting companies when identified.

The goal is to improve transparency and understanding of public infrastructure without assumptions or accusations—focusing instead on structured, traceable data.

---

## 🎯 Core Objectives

- Map all road construction activity across jurisdictions  
- Track the full lifecycle of infrastructure projects  
- Identify funding structures behind public works  
- Document contracting companies involved in projects  
- Visualize repeated or cyclical road repairs  
- Provide citizens with a structured reporting system  
- Create a unified infrastructure intelligence layer  

---

## 🧠 Key Features

### 🗺️ Interactive Infrastructure Map
- Visual map of roads and active projects  
- Filters by city, county, and state  
- Layered view of project types and statuses  
- Geographic clustering of infrastructure activity  

---

### 🧾 Road Project Profiles
Each road has a persistent profile including:
- Road name and segment  
- City / Town / County / State  
- Full project history timeline  
- Work type (resurfacing, reconstruction, utility cuts, drainage, etc.)  
- Project status (planned, active, completed, recurring)  

---

### 🔁 Infrastructure Cycle Tracking
- Detects repeated construction on the same road segments  
- Identifies frequent resurfacing or repair cycles  
- Flags high-activity infrastructure corridors  
- Builds a long-term timeline of road interventions  

---

### 💰 Funding Transparency Engine
AI-assisted analysis of funding sources:
- State transportation budgets  
- Federal infrastructure programs  
- County and municipal capital funds  
- Utility-driven infrastructure work  
- Public bid and grant data  

Each funding breakdown may include:
- Explicit sources (documented)  
- Inferred sources (AI-synthesized with confidence scoring)  

---

### 🏗️ Contracting Company Mapping
Tracks companies involved in infrastructure projects:
- Primary contractors  
- Subcontractors (when available)  
- Engineering firms  
- Construction management firms  

Includes:
- Contract award history  
- Corridor-level contractor activity  
- Relationship between contractors and repeated work zones  

---

### 📢 Citizen Reporting System
Users can submit:
- Road conditions  
- Photos and evidence  
- Reports of ongoing construction  
- Observations of repeated work cycles  

All reports are structured by:
- Road  
- City / Town  
- County  
- State  

---

### 📊 Project Timeline Viewer
- Chronological view of all road activity  
- Phase-based breakdown of construction projects  
- Historical comparison of repeated interventions  

---

### 🧠 AI Infrastructure Analysis Layer
- Extracts structured data from public records  
- Links roads, funding, and contractors  
- Identifies project patterns across jurisdictions  
- Generates infrastructure activity summaries  

All AI outputs are:
- Source-aware  
- Confidence-scored  
- Clearly labeled as explicit or inferred  

---

## 🏛️ Jurisdiction Structure

Every record is organized by:

- Road  
- City / Town  
- County  
- State  

Example:
- Road: Route 70  
- City: Cherry Hill  
- County: Camden County  
- State: New Jersey  

---

## 🧱 System Philosophy

Road Systems Watch is designed as a **neutral infrastructure intelligence system**, not a complaint or enforcement platform.

It prioritizes:
- Transparency over speculation  
- Structure over narrative  
- Data traceability over assumptions  
- Public understanding of infrastructure systems  

---

## 🔧 Suggested Tech Stack

- Frontend: React + MapLibre or Leaflet  
- Backend: FastAPI or Node.js  
- Database: PostgreSQL + PostGIS  
- Storage: S3-compatible object storage  
- AI Layer: document ingestion + entity extraction pipeline  
- Graph Layer: infrastructure knowledge graph (roads ↔ funding ↔ contractors ↔ projects)  

---

## 📌 Example Road Profile Output

**Route 70 – Cherry Hill, Camden County, New Jersey**

- Active projects: resurfacing + utility coordination  
- Funding sources:
  - State transportation capital program  
  - Federal highway assistance  
  - Utility coordination funding  
- Contracting companies:
  - Primary contractor: (from public bid records when available)  
  - Engineering firm: (if disclosed)  
- Pattern: High-frequency repair corridor  
- Status: Multi-phase infrastructure cycle  

---

## 🚀 Vision

Road Systems Watch aims to become a national infrastructure intelligence layer that enables:

- Clear visibility into public works  
- Understanding of infrastructure funding flows  
- Tracking of contractor involvement over time  
- Detection of recurring infrastructure interventions  
- Better-informed civic engagement  

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
  - [https://roxanneardary.com/road-systems-watch/](https://roxanneardary.com/road-systems-watch/)  

---

## 📦 License & Notice Requirements

Road Systems Watch is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
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
