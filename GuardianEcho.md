# GuardianEcho

**Echoes of Truth, Shielded from Harm.**

GuardianEcho is an open-source, encrypted, identity-verified whistleblower reporting platform designed to help families safely report threats, misconduct, or abuse involving social service workers, educators, and government officials.

The platform is built with privacy-first architecture, strong encryption standards, and a strict separation between identity verification and report content to protect users from retaliation while maintaining report integrity.

---

## 🚨 Mission

To provide a **secure, verifiable, and anonymous reporting system** that protects families while enabling accountability in public institutions.

---

## 🔐 Key Principles

- Privacy by design  
- End-to-end encryption  
- Identity verification without exposure  
- Whistleblower protection by default  
- Open-source transparency  
- Auditability without surveillance  

---

## 🧩 Full Feature List

### 🧭 Core Platform Features
- Secure submission system for reporting threats, misconduct, or abuse  
- Structured reporting forms (incident type, location, time, narrative, evidence upload)  
- Multi-category reporting system (education, social services, law enforcement, government agencies, etc.)  
- Case tracking system with anonymized status updates  
- Unique encrypted report IDs for follow-up without revealing identity  

### 🔒 Security & Encryption
- End-to-end encryption (E2EE) for all submissions and attachments  
- Client-side encryption before data transmission  
- Zero-trust backend architecture  
- Encrypted file storage for evidence (documents, images, audio, video)  
- Secure key management and rotation system  
- Optional multi-recipient encryption for oversight bodies or legal partners  

### 🧾 Identity Verification (Privacy-Preserving)
- Real identity verification for reporters using secure verification systems  
- Separation of identity layer from reporting layer  
- Pseudonymous reporting tokens after verification  
- Anti-fraud validation to reduce abuse while preserving anonymity  
- Optional re-verification for high-risk submissions  

### 🛡️ Whistleblower Protection System
- Automatic metadata stripping (IP, device, and fingerprint minimization)  
- Anonymous report submission pipeline  
- Secure follow-up messaging without identity exposure  
- High-risk protection mode for sensitive reporters  
- Jurisdiction-aware privacy configurations  

### 📊 Case Management & Review System
- Role-based access control (RBAC) dashboard for reviewers  
- Multi-party review workflow  
- Evidence validation tools (hash verification, timestamps)  
- Case tagging and prioritization system  
- Secure internal notes (encrypted access layer)  
- Escalation workflows for urgent cases  

### 🧩 Transparency & Auditability
- Append-only audit logs  
- Cryptographic integrity verification for records  
- Tamper-evident log structures  
- Aggregated anonymized transparency reporting  
- Exportable compliance and audit reports  

### 🌐 Open Source & Developer Features
- Licensed under AGPL-3.0+  
- GitLab-based development workflow  
- Modular architecture (identity, encryption, reporting, review layers)  
- REST and GraphQL API support  
- Webhook system for NGOs and oversight integrations  
- SDK for building extensions and integrations  

### 🖥️ User Interface Features
- Mobile-first responsive design  
- Accessibility compliance (WCAG-focused)  
- Multi-language support  
- Dark mode and low-visibility “panic mode” interface  
- Offline draft saving with encrypted local storage  
- Guided reporting wizard for non-technical users  

### 🚨 Safety & Abuse Prevention
- Rate limiting and abuse detection  
- AI-assisted moderation flagging (review-only, non-blocking)  
- Duplicate report detection  
- Controlled disclosure protections against doxxing  
- Secure spam filtering system  

### 🏛️ Governance & Compliance Layer
- Jurisdiction-based deployment configuration  
- Legal compliance templates (whistleblower protections, FOIA workflows where applicable)  
- Data retention and expiration controls  
- Optional NGO/legal oversight modules  
- Regional data segregation support  

### ⚙️ Infrastructure & Deployment
- Dockerized deployment support  
- Kubernetes scaling support  
- Encrypted PostgreSQL data layer  
- GitLab CI/CD pipelines  
- Self-hosting friendly architecture  
- Optional air-gapped deployment mode  

---

## 🛠️ Tech Stack

- Frontend: React, Tailwind CSS  
- Backend: Node.js, Express.js  
- Database: PostgreSQL (encrypted layer)  
- Encryption: libsodium, OpenPGP standards  
- Deployment: Docker, Kubernetes  
- CI/CD: GitLab Pipelines  

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
  - [https://roxanneardary.com/guardianecho/](https://roxanneardary.com/guardianecho/)

---

## 📜 License & Notice Requirements

GuardianEcho is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- GuardianEcho specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's `notice.md` file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.  
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.  

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  
