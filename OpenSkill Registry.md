# OpenSkill Registry

**Keep Experience Working.**

OpenSkill Registry is a privacy-first, AI-powered, open-source platform that connects verified individuals with real-world skills to short-term, part-time, and micro-gig opportunities in their local communities.

Built as civic infrastructure under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**, the system is designed to strengthen local economies while preserving dignity, privacy, and autonomy.

---

## 🔧 Core Concept

A verified, encrypted, AI-driven skill network where:

- Retirees and job seekers list real-world skills
- Employers and individuals find trusted local talent
- AI matches people to work based on skill, location, and availability
- Micro-gigs and “instant work” opportunities can be activated in real time

This is not a gig app.  
It is a **local workforce intelligence system**.

---

## 🧩 Full Modular Feature Set

### 1. Identity, Verification & Trust Module
- Verified citizen onboarding (government ID required)
- Optional biometric/selfie verification
- Encrypted identity vault (never exposed in search layer)
- Zero-knowledge proof-based identity validation
- Employer/business verification system
- Role-based access control (retiree, employer, requester, admin)
- Privacy controls (alias mode, location masking, visibility toggles)

---

### 2. Skill Profile & Registry Module
- Unlimited multi-skill tagging per user
- Skill proficiency levels (self-reported + optional endorsements)
- Industry categorization system
- Experience history abstraction layer
- Certification and credential uploads (encrypted)
- Availability scheduling (hourly, seasonal, project-based)
- Work preference configuration (remote, hybrid, local)

---

### 3. AI Search & Matching Module
- Natural language search (“retired electrician near me for 2 weeks”)
- Semantic skill search (embedding-based matching)
- Location-aware ranking (town, radius, commute time)
- Availability-aware filtering
- Experience-level matching
- Intelligent recommendations for workers and employers
- Skill similarity graph matching

---

### 4. Geographic & Local Matching Module
- Town-based skill indexing
- Radius-based search (configurable distance)
- ZIP and municipality mapping
- Commute-time optimization
- Regional labor demand heatmaps
- Local workforce gap detection

---

### 5. Employer & Job Posting Module
- Short-term job postings (hours to weeks)
- Skill-based job definitions (no resumes required)
- Contract, gig, advisory, and mentorship roles
- Employer dashboards
- AI-generated candidate shortlists
- Saved searches and role templates

---

### 6. “I Work for Tips” Micro-Gig Module
- “Available Now” instant status toggle
- Micro-task postings (1–4 hour jobs)
- Tip-based or flexible payment models
- Real-time AI matching of nearby workers
- Skill-category filtering for instant work
- Emergency income mode (priority matching)
- One-click request-to-hire system

**Safety & Controls**
- Verified identity required for participation
- Masked communication until mutual acceptance
- Reputation tracking for completed gigs
- Spam and fraud detection systems
- Optional trusted-circle-only mode

---

### 7. Communication & Engagement Module
- End-to-end encrypted messaging
- Mutual consent contact unlocking
- Scheduling and coordination tools
- Notification system (email/SMS optional)
- Interview and task confirmation flows

---

### 8. Data Privacy & Encryption Module
- AES-256 field-level encryption for all PII
- Public skill index separated from private identity vault
- Zero-knowledge identity storage architecture
- Encrypted search indexing (metadata only exposure)
- Secure key rotation system
- GDPR/CCPA-aligned compliance structure

---

### 9. AI Skill Graph & Knowledge Layer
- Skill ontology graph
- Embedding-based semantic similarity engine
- Industry clustering of skills
- Cross-domain skill transfer detection
- Workforce demand prediction per region
- Career trajectory modeling (non-invasive)

---

### 10. Reputation & Trust Signals Module
- Verified work completion tracking
- Structured employer feedback system
- Optional skill endorsements
- Reliability scoring (time-based, not popularity-based)
- Fraud detection signals

---

### 11. Admin & Governance Module
- Full audit logging (tamper-resistant)
- Moderation dashboard
- Verification review workflows
- Abuse reporting system
- Transparency reporting tools
- Contribution tracking for open-source governance

---

### 12. Open Source & Developer Module (AGPL-3.0+)
- Fully open-source AGPL 3.0+ licensing
- Public API (rate-limited)
- Plugin architecture for municipalities and organizations
- Self-hostable deployment (Docker + Kubernetes)
- Community contribution system
- Extension system for integrations

---

### 13. Infrastructure & Deployment Module
- Microservices architecture (containerized)
- PostgreSQL core database
- OpenSearch indexing and retrieval
- Redis caching layer
- Vector database (Weaviate or equivalent)
- CI/CD pipelines for contributions
- Infrastructure-as-code (Terraform / Pulumi)

---

## 🧠 System Summary

OpenSkill Registry combines:

**Identity verification + Skill intelligence + AI matching + Local workforce activation + Real-time micro-gigs**

All built on a **privacy-first, AGPL 3.0+ open-source foundation**.

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
  - [https://roxanneardary.com/openskill-registry/](https://roxanneardary.com/openskill-registry/)  

---

## 📜 License & Notice Requirements

OpenSkill Registry is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
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
