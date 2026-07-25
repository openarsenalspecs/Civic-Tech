# TrueOwnerOS  
### Bringing Ownership Out of the Shadows.

---

## Overview

**TrueOwnerOS** is an open-source intelligence (OSINT) platform that maps **mission-critical corporate properties** and reveals the **true ownership structures behind them**.

It identifies when a company relies on a **building it does not own**, exposing hidden vulnerabilities across:

- Corporations  
- REITs  
- Private Equity Groups  
- Global Infrastructure Funds  
- Government Facilities  
- Hospitals, Utilities, and Critical Services  

TrueOwnerOS converts disparate public records into a **unified, AI-powered ownership graph**.

---

## Mission

To create the **world’s public ledger of mission-critical real estate ownership**, enabling:

- Transparency  
- Risk awareness  
- Economic stability  
- Infrastructure resilience  
- Public accountability  

Ownership *is power*, and power should be visible.

---

## Key Features

### 🔍 Ownership Intelligence  
- Resolves shell companies and LLC networks  
- Maps corporate family trees  
- Identifies operator–owner mismatches  
- Reveals hidden control structures  

---

### 🏢 Mission-Critical Property Classification  
AI automatically classifies:

- Data centers  
- Fulfillment & logistics hubs  
- Hospitals & clinics  
- Telecom & fiber nodes  
- Power & utility sites  
- Manufacturing plants  
- Government leased facilities  
- Emergency services  
- Public infrastructure sites  

---

### 📄 Lease Structure Intelligence  
Extracts and interprets:

- Triple-net (NNN), NN, N  
- Sale-leasebacks  
- Lease durations & expirations  
- Rent escalators  
- Tenant concentration risk  
- Lease-adjusted leverage metrics  

---

### 🕵️ Ownership Shadow Detection  
Flags properties with:

- Shell LLC ownership  
- Related-party leases  
- Suspicious sale-leaseback cycles  
- High escalation rent abuse  
- Inadequate disclosures  
- Private equity extraction patterns  

---

### 🔗 Corporate Dependency Scores  
For each operator:

- **Operational Criticality Score (OCS)**  
- **Population Impact Score (PIS)**  
- **Relocation Difficulty Score (RDS)**  
- **Corporate Failure Impact Score (CFIS)**  

---

### 📉 Concentration Risk Detection  
Reveals:

- REITs overly reliant on a single tenant  
- Cities overly reliant on one corporation  
- Corporations dependent on one landlord  
- Subsidiary clusters creating false diversification  

---

## Advanced Intelligence Modules

### 🗺️ Infrastructure Fragility Mapping  
Detects co-located and interdependent systems:

- Power + telecom + hospital zones  
- Industrial + logistics chokepoints  
- Multi-system failure clusters  

Marks **“If this building fails, the town fails”** sites.

---

### 🧩 Corporate Collapse Simulation Engine  
Simulates impacts of:

- Tenant bankruptcy  
- Lease defaults  
- Rent hikes  
- Natural disasters  
- REIT liquidations  
- Infrastructure failure events  

Produces:

- Closure forecasts  
- Service loss maps  
- Population impact reports  
- Supply chain disruption analysis  

---

### 🚚 Supply Chain Dependency Mapping  
AI identifies:

- Supplier → distributor → retailer chains  
- Dependency on non-owned infrastructure  
- Critical logistics nodes  
- Chokepoints in national supply webs  

---

### 💰 Private Equity Extraction Scanner  
Flags:

- Debt stacking  
- Asset stripping  
- Aggressive sale-leasebacks  
- Rent inflation strategies  
- Dividend extraction patterns  

Detects corporate hollowing before collapse.

---

### 🏛️ Government & Public Dependency Tracking  
Maps privately owned:

- USPS hubs  
- DMV offices  
- Social services buildings  
- Emergency facilities  
- Utility operations  
- Charter schools  
- Courthouses & public admin sites  

Shows where **public services rely on private landlords**.

---

### 📉 Tenant Credit & Failure Modeling  
Automatically ingests:

- Credit ratings  
- Bond yields  
- SEC filings  
- Cash flow metrics  
- Lease-adjusted debt  

Predicts:

- Default probability  
- Renewal likelihood  
- Rent stress exposure  

---

### 🌍 Global Ownership Mapping  
Supports:

- Cross-border corporate structures  
- Offshore holding companies  
- Sovereign wealth fund ownership  
- International REITs  

---

### 🔥 Failure Event Registry  
Tracks:

- Foreclosures  
- Hospital closures  
- Data center outages  
- Distribution hub fires  
- Utility failure incidents  

Correlates failures with **ownership risk structures**.

---

### 🧭 Resilience Scoring System  
Each corporation receives:

- **Property Control Index (PCI)**  
- **Landlord Power Score (LPS)**  
- **Failure Impact Score (FIS)**  
- **Community Dependency Score (CDS)**  

---

### 📂 FOIA Integration Layer  
Supports and stores:

- Government records  
- Lease disclosures  
- Procurement contracts  
- Public building ownership files  

All FOIA results can be added to the public dataset.

---

## System Architecture

### 🔗 Data Sources
- SEC Filings (10-K, 10-Q, 8-K)  
- County property records  
- Corporate registrations  
- FOIA/OPRA documents  
- Telecom & utility registries  
- Infrastructure maps  
- Public GIS data  
- Bankruptcy filings  

---

### 🔄 Processing Pipeline
1. Ingest raw data  
2. Normalize entities  
3. Resolve ownership  
4. Identify operators  
5. Extract lease structure  
6. Assign risk scores  
7. Build graph models  
8. Expose via APIs  

---

## Data Model (Simplified)

```text
/entities
  entity_id
  name
  parent_id
  ultimate_owner

/properties
  property_id
  address
  geo
  category
  mission_critical_level

/ownership
  property_id
  owner_entity
  ownership_type

/operators
  property_id
  operator_entity
  lease_type
  lease_end
  rent_terms

/risk
  property_id
  risk_score
  dependency_indicators
  ```

# API Access

TrueOwnerOS offers:

- REST API
- GraphQL API
- Command Line Interface
- Bulk data download endpoints

Example query:
```bash
GET /properties?operator=Microsoft&ownership_mismatch=true
```

## Use Cases

### Investors
- REIT tenant risk  
- Corporate lease exposure  
- Private equity extraction detection  

### Journalists
- Hidden ownership tracing  
- Infrastructure vulnerability stories  
- Public service landlord investigations  

### Governments
- Emergency planning  
- Infrastructure dependency mapping  
- Municipal risk analysis  

### Communities
- “Who owns the building my hospital is in?”  
- Local infrastructure reliance awareness  

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
  - [https://roxanneardary.com/trueowneros/](https://roxanneardary.com/trueowneros/)

---

## License & Notice Requirements

TrueOwnerOS is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- TrueOwnerOS specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---

## Contributing

We welcome contributions in:

- Data ingestion  
- AI extraction models  
- Risk scoring algorithms  
- Dashboard UI  
- Graph analytics  
- Documentation  

See `CONTRIBUTING.md`.

---

## Vision

TrueOwnerOS aims to become:

- The global standard for ownership transparency  
- The public’s infrastructure intelligence layer  
- A research tool for economic & civic stability  
- A permanent record of who controls mission-critical real estate  

**Ownership should never be hidden.**  
TrueOwnerOS makes it visible.  
