# Carenex

**Empowering You Through Every Policy Decision**  
Official Website: [https://www.roxanneardary.com](https://www.roxanneardary.com)

---

## Overview

Carenex is an **open-source, HIPAA-compliant platform** designed to provide AI-driven health insurance recommendations, predictive claims outcomes, and transparency for insurance plan adherence.  
The platform allows users to securely upload claims, track insurer performance, and make fully informed decisions on health coverage. All data is encrypted end-to-end and sourced from official, verified sources.

Carenex supports **all types of insurance**, including individual, family, corporate, co-op, Medicare/Medicaid, and supplemental plans.

---

## Features

### User Experience & Personalization
- Multi-profile support (dependents, family members)  
- Dynamic AI Q&A for personalized data collection  
- Scenario simulation for major health events  
- Goal-based recommendations (cost, coverage, network, claims reliability)  
- Personal coverage score per plan  
- Customizable weighting (user chooses priorities)  
- Plan comparison dashboard with charts  
- Exportable PDF summaries  
- Plan renewal forecasting  
- Health savings guidance (HSA/FSA strategies)  

### Modular Design

Carenex uses a **modular architecture** that keeps the platform extensible, maintainable, and adaptable to different insurance environments. Core functionality is organized into dedicated modules, while optional capabilities can be added through a plugin system without requiring changes to the underlying platform.

### Core AI Modules

#### Policy Analysis Module
- Policy fine-print analysis
- Identification of limitations, exclusions, penalties, and coverage restrictions
- Natural language explanations of complex policy provisions
- Detection of conflicts between policy language and applicable requirements

#### Claims Prediction Module
- Predictive claims outcomes
- Claim approval likelihood
- Coverage-gap identification
- Payment and delay risk analysis
- Outcome probability modeling

#### Risk & Anomaly Module
- Fraud and risk detection for policy inconsistencies
- Fine-grained risk scoring by procedure, medication, provider, and coverage type
- Detection of unusual insurer behavior
- AI pattern detection for recurring coverage or denial patterns

#### Recommendation Module
- Personalized insurance recommendations
- Plan suitability scoring
- Cost and coverage comparisons
- User-priority weighting
- Personalized alerts for policy changes, coverage changes, or potential savings

#### Appeals & Claims Assistance Module
- AI-assisted guidance for denied claims
- Analysis of denial reasons against applicable policy provisions
- Identification of potentially relevant appeal pathways
- Organization and summarization of supporting documentation

#### Health & Treatment Analysis Module
- Outcome prediction for medications, hospitalizations, and treatments
- Scenario-based coverage modeling
- Out-of-pocket cost projections
- Procedure and treatment coverage analysis

#### Comparison & Reporting Module
- Natural language comparison reports
- Side-by-side plan analysis
- Outcome probability dashboards
- Coverage and cost summaries
- Explainable AI recommendations

---

### Optional Plugin Modules

Carenex supports optional plugins that extend the platform without expanding the core system unnecessarily. Plugins can provide specialized functionality while using standardized Carenex interfaces, permissions, and data contracts.

Optional plugins may include:

- **Pharmacy & Formulary Plugin** — medication coverage, formulary analysis, tiers, copays, and historical drug coverage
- **Provider Network Plugin** — provider, hospital, clinic, and network coverage analysis
- **Multi-State Coverage Plugin** — state-by-state plan, regulatory, network, and coverage comparisons
- **Insurance Marketplace Plugin** — marketplace plan discovery and enrollment-period analysis
- **Medicare & Medicaid Plugin** — specialized analysis for government health programs
- **Employer Insurance Plugin** — comparison of employer-sponsored plans and benefits
- **Cooperative Insurance Plugin** — analysis of cooperative and member-based insurance models
- **Supplemental Coverage Plugin** — dental, vision, disability, accident, critical illness, and supplemental coverage
- **Claims Archive Plugin** — secure organization and historical analysis of user-submitted claims
- **Insurer Accountability Plugin** — insurer adherence profiles, payment behavior, denial patterns, and historical performance
- **Regulatory Intelligence Plugin** — state and federal regulations, enforcement actions, mandates, and regulatory changes
- **Appeals Documentation Plugin** — organization and preparation of documentation for insurance appeals
- **Healthcare Cost Plugin** — procedure, treatment, facility, and out-of-pocket cost modeling
- **Telehealth Plugin** — analysis of telemedicine coverage and benefits
- **Travel Coverage Plugin** — coverage analysis for users who travel or reside across multiple states
- **Personal Health Data Plugin** — optional integration with authorized personal health data sources
- **Community Insights Plugin** — anonymized user-submitted experiences and verified community observations
- **Education Plugin** — insurance terminology, educational resources, and interactive guides
- **Notification Plugin** — enrollment deadlines, policy changes, renewals, and personalized alerts
- **Localization Plugin** — additional languages, regional requirements, and accessibility features

The modular architecture allows Carenex to maintain a **small, secure core while supporting a broad insurance ecosystem through independently maintained plugins**. Plugins can be enabled, disabled, updated, or replaced without requiring the entire platform to be rebuilt.

### Claims & Accountability
- Secure upload of denied claims, overpayments, disputes  
- Claims parsing with OCR & NLP  
- Insurance company adherence profiles & performance scores  
- Historical trend tracking (claims approval, timeliness, compliance)  
- Community transparency feed (anonymized)  
- Real-time anomaly alerts for spikes in claim denials  
- Crowdsourced claim validation  
- Insurer dispute tracker  
- Claim cost benchmarking  

### Data & Integrations
- Aggregation of official sources (CMS, state exchanges, insurer PDFs)  
- Historical policy tracking (coverage and premium changes)  
- Pharmacy coverage and cost modeling  
- Provider network mapping (hospitals, clinics, doctors)  
- Multi-state coverage comparison  
- Travel mode coverage estimation  
- Predictive formulary coverage  
- Integration with telemedicine platforms (optional)  
- Open-source API for external apps and portals  

### Security & Compliance
- Full HIPAA compliance  
- End-to-end encryption for all data  
- Anonymized analytics (optional)  
- Two-factor authentication (2FA)  
- Audit logging  
- Optional data deletion on request  
- Encrypted AI model inference  
- Regulatory compliance alerts  
- Self-sovereign data control  

### Community & Engagement
- User forum / Q&A (moderated, privacy-conscious)  
- Public leaderboard for insurer reliability and adherence  
- Educational content (guides, tutorials, videos)  
- Multi-language support  
- Notifications & reminders  
- Anonymous Q&A with verified users  
- Insurer reputation heatmap  
- Gamified claim reporting  
- Crowdsourced insights into tricky policy clauses  

### Platform & Ecosystem
- Mobile-friendly responsive web app  
- Offline PDF generation for recommendations & claims summaries  
- Cloud hosting with secure storage  
- Open-source modular codebase  
- Versioned database for policies & claims  
- Gamified savings suggestions  
- Plugin architecture for third-party modules  
- Integration with personal health apps (optional, anonymized)  
- Machine learning for price optimization & premium trend predictions  
- AI-driven alerts for open enrollment and plan switching  

### Optional / Future Features
- Health event risk modeling  
- Predictive modeling for hospital & treatment costs  
- Integration with pharmacy formulary APIs  
- Community-driven validation of claims & insurer adherence  
- Personalized “what-if” scenario modeling  
- AI-driven supplemental or hybrid plan recommendations  

---

## Installation

Carenex is fully open-source and can be deployed on **any modern web server**. Recommended stack:  
- Backend: Python / Django or Node.js  
- Frontend: React / Vue  
- Database: PostgreSQL or MySQL  
- Optional AI/ML modules: TensorFlow or PyTorch  
- Cloud hosting: AWS, GCP, Azure, or self-hosted  

```bash
# Clone the repository
git clone https://gitlab.com/Roxanne_Ardary/carenex.git
cd carenex

# Install dependencies
pip install -r requirements.txt   # or npm install for Node.js backend

# Run the development server
python manage.py runserver         # or npm start for Node.js
```

## Usage

1. Create an account and log in (2FA recommended).  
2. Complete the AI-driven Q&A to build your health profile.  
3. Browse AI-recommended insurance plans with personalized scores and predictions.  
4. Upload any denied claims or disputes to build your claims history.  
5. Compare insurers, plans, and multi-state coverage for your situation.  
6. Export PDFs or receive alerts on policy changes and open enrollment opportunities.  

---

## Contribution Guidelines

Carenex is **open-source under the GNU AGPL 3.0+ license**. Contributors are welcome to:  
- Submit verified policy updates  
- Improve AI recommendation algorithms  
- Enhance UI/UX and accessibility  
- Add integrations for telemedicine or pharmacy data  

**Important:** All contributions must follow HIPAA-compliant practices for sensitive data handling.

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
  - [https://roxanneardary.com/carenex/](https://roxanneardary.com/carenex/)

---

## License & Notice Requirements

Carenex is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- Carenex specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
