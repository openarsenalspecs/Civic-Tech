# Demographica

**Analytics That Speak Your Language**

Demographica is an open-source civic data platform that transforms government-published demographic datasets into clear, searchable, and interactive insights for any geographic area. It allows users to explore population, income, housing, education, employment, and migration data across cities, ZIP codes, counties, states, and countries through a unified system.

---

## 🌍 Overview

Demographica is designed as a **modular, hierarchical, and globally extensible demographic intelligence system**. It aggregates official public datasets and standardizes them into a consistent format for analysis, visualization, and developer access.

The platform is built to support:
- United States state → county → city → ZIP structures
- International expansion via country-specific adapters
- Custom geographic regions and boundaries

---

## 🧱 Modular Architecture

Demographica is built as independent modules that can be extended or replaced without affecting the core system.

### 1. Core Platform Module
- Location search and normalization
- Central API routing
- Geographic identifier mapping (ZIP, FIPS, GEOID)
- Module registry system

### 2. Geographic Intelligence Module
- Spatial queries and boundary detection
- GeoJSON generation
- Map-ready dataset formatting
- PostGIS-based spatial indexing

### 3. Demographics Module
- Population statistics
- Age, gender, and ethnicity distribution
- Household composition
- Education levels

### 4. Housing Module
- Homeownership rates
- Rent and housing cost data
- Vacancy and occupancy rates
- Housing affordability indicators

### 5. Economic & Employment Module
- Employment and unemployment rates
- Industry distribution
- Occupational breakdowns
- Income and wage statistics

### 6. Trends & Analytics Module
- Historical demographic trends
- Migration patterns
- Growth rate analysis
- Multi-region comparisons

### 7. Visualization Module
- Interactive maps and dashboards
- Charts and statistical graphs
- Choropleth heatmaps
- Comparative region views

### 8. API & Integration Module
- RESTful API access
- Bulk data endpoints
- Developer query interface
- Machine-readable outputs

### 9. Data Ingestion Module
- Government data extraction pipelines
- Data cleaning and normalization
- Scheduled updates and synchronization
- Multi-source integration layer

### 10. Performance & Infrastructure Module
- Caching layer for fast queries
- Background processing jobs
- Scalable request handling
- Containerized deployment support

### 11. Plugin & Extension Module
- Community-built data connectors
- Custom visualization plugins
- External dataset integrations
- Extensible architecture for new data sources

### 12. Governance & Licensing Module
- Attribution tracking system
- Data provenance logging
- Open-source compliance enforcement
- Transparency auditing tools

---

## 🗺️ Geographic Hierarchy System

Demographica uses a structured geographic tree:

Country → State/Province → County/District → City → ZIP/Postal Code → Census Tract

### United States Model
- State-level partitions for all 50 states
- County-level aggregation and caching
- City and ZIP-level detailed breakdowns
- Census tract support for granular analysis

### International Expansion
Demographica supports a pluggable country adapter system:
- Canada: Province → Census Division → Municipality → Postal Code
- United Kingdom: Nation → Region → County → District → Postcode
- Extensible model for any country

Each adapter normalizes:
- Geographic hierarchy
- Statistical categories
- Government data sources

---

## 📊 Core Features

### Location Intelligence
- Search by ZIP, city, county, or custom region
- Automatic geocoding and boundary resolution
- Standardized geographic identifiers

### Demographic Insights
- Population totals and density
- Age distribution
- Race and ethnicity composition
- Household and family structure

### Housing Analytics
- Rent and home value metrics
- Ownership vs rental breakdowns
- Housing availability and vacancy rates

### Economic Data
- Employment and unemployment rates
- Industry and occupation breakdowns
- Income distribution metrics

### Trend Analysis
- Multi-year population tracking
- Economic growth trends
- Migration flow analysis
- Regional comparisons

### Visualization
- Interactive geographic maps
- Heatmaps for demographic indicators
- Charts and dashboards
- Side-by-side region comparisons

### Developer API
- RESTful endpoints for all datasets
- Structured JSON responses
- Bulk data querying support
- Integration-ready architecture

### Data Export
- CSV export for spreadsheets
- JSON export for APIs
- PDF reporting for analysis summaries

---

## ⚙️ Technology Stack

- Backend: Python (FastAPI) or Node.js (Express)
- Database: PostgreSQL with PostGIS extension
- Frontend: React with TypeScript
- Visualization: D3.js and Chart.js
- Mapping: MapLibre with OpenStreetMap
- Data Processing: Pandas, GeoPandas, Shapely
- Infrastructure: Docker, optional Redis caching layer
- Data Sources:
  - U.S. Census Bureau (ACS, TIGER/Line)
  - Bureau of Labor Statistics
  - HUD housing datasets
  - CDC public health data
  - USDA rural statistics

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
  - [https://roxanneardary.com/demographica/](https://roxanneardary.com/demographica/)  

---

## ⚖️ License & Notice Requirements

Demographica is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the AGPL-3.0+ terms.  
- Under Section 7 of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- The project's notice.md file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update notice.md.  
- When submitting a pull request, ensure that any new files maintain attribution requirements where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.  

For full legal details, refer to the AGPL-3.0+ license and the notice.md file.
