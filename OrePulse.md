# OrePulse

**Tagline:** Where Geology Meets Technology

---

## 🌐 Project Overview

**OrePulse** is an open-source platform designed to map, track, and analyze all economically relevant magnetic minerals across the United States, including:

- **Magnetite**  
- **Iron sands**  
- **Rare earth elements (REEs)**  
- Other **magnetic sediments** feasible for mining  

OrePulse combines **geospatial mapping, corporate intelligence, and predictive analytics** to provide a transparent, interactive, and educational tool for researchers, industry professionals, journalists, and the public.

---

## 🔑 Features

### 1. Geospatial & Geological
- LIDAR-based terrain and magnetic susceptibility mapping  
- Mineral deposit mapping by state and site  
- Mine boundaries and claim information (active, historical, abandoned)  
- Predictive mineral mapping with AI/ML  
- Historical mining footprint visualization  
- Environmental overlays: protected areas, water bodies, wetlands, wildlife habitats  
- Mine feasibility scoring (cost, difficulty, environmental impact)  
- 3D geological visualization  

### 2. Corporate & Legal Intelligence
- Company profiles (legal name, incorporation state, SEC filings)  
- Founders, officers, and board members  
- Subsidiary and parent company networks  
- Shell company identification and connections  
- Board member influence mapping  
- Funding and investment tracking  
- Financial health indicators and risk scoring  
- Real-time news and alerts  
- Transparency scoring and regulatory compliance flags  

### 3. Mineral & Production Tracking
- Detailed mineral composition and deposit grades  
- Mining status tracking: active, proposed, closed, reclaimed  
- Production volumes and commodity pricing  
- Supply chain mapping from extraction to manufacturing  
- Extraction methods and energy usage  

### 4. Public-Facing Tools
- Interactive geospatial map with filtering and search  
- Profiles for mines, minerals, companies, and people  
- Network visualization of corporate and personal connections  
- Dashboards and charts for production, deposits, and transparency  
- Downloadable datasets (CSV, GeoJSON, Shapefile)  
- API access for developers and researchers  
- Crowdsourced reporting and observation tools  
- Educational modules  

### 5. Security, Compliance & Safety
- Export control and regulatory tracking  
- Safety and hazard reporting (OSHA, environmental inspections)  
- Environmental impact scoring  

### 6. Analytics & Insights
- Network analysis of companies, people, and deposits  
- Trend reporting for mining growth, rare-earth supply, and environmental impact  
- Comparison tools across states, companies, and mineral types  
- Scenario modeling for policy or resource changes  
- Predictive analytics for mineral discovery  

### 7. Advanced Technology
- IoT sensor integration from active mines  
- Blockchain ledger for mineral provenance and supply chain transparency  
- VR/AR visualization of mining sites and geophysical data  
- AI/ML models for predictive mapping and risk analysis  

### 8. Infrastructure & Automation
- PostGIS for geospatial storage and queries  
- Graph database (Neo4j) for relationships and networks  
- Automated ETL pipelines for geological, corporate, and personal data  
- Scheduled updates for all datasets  
- Data validation and quality standards  

### 9. Community & Governance
- Contributor guides and documentation  
- Open-source AGPL 3.0+ license with mandatory attribution  
- Issue tracking and project roadmap  
- Data moderation and verification team  
- Public transparency dashboards  

---

## 🛠 Installation & Usage

1. **Clone the repository:**
```bash
git clone https://gitlab.com/Roxanne_Ardary/orepulse.git
```
2. **Set up the database:**
   - PostgreSQL + PostGIS for geospatial data  
   - Neo4j for corporate and relationship networks  

3. **Load initial datasets:**  
   - USGS Mineral Resources Data System (MRDS)  
   - BLM Mining Claims  
   - State geological surveys  
   - Corporate data via OpenCorporates and SEC filings  

4. **Run the ETL pipelines:**  
   - Normalize, clean, and populate PostGIS + Neo4j  

5. **Start the web interface:**  
   - Frontend: React + Mapbox GL  
   - Backend: Node.js or Python Flask  
   - Dashboards and network visualizations accessible at `/dashboard`

## 🤝 Contributing

We welcome contributions from the community:  

- Fork the repository and submit merge requests  
- Add new datasets or improve geospatial mapping  
- Develop additional dashboards, charts, or analytics  
- Ensure all contributions follow **AGPL 3.0+** licensing  

---

## ⚠ Disclaimer

OrePulse collects **only publicly available data**. Accuracy of external sources is the responsibility of users. OrePulse does **not provide legal, financial, or operational advice**.  

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
  - [https://roxanneardary.com/orepulse/](https://roxanneardary.com/orepulse/)

---

## License & Notice Requirements

- OrePulse specifications are free to use with attribution. A Specification Branding License can be negotiated upon request. is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- OrePulse specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
