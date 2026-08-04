# Kova

**Kova - Guardrails for the AI era**

Kova is a modular, AGPL-licensed AI governance and execution framework designed to enforce structured control over artificial intelligence, web access, and system-level actions. It scales from household parental controls to enterprise-grade distributed policy enforcement systems.

---

## Overview

Kova is built on the principle that AI systems should never operate without enforceable boundaries. It separates intelligence, policy, and execution into distinct layers, ensuring that all AI actions are governed, auditable, and configurable across environments.

It supports:
- Consumer environments (families, education)
- Enterprise environments (organizations, regulated systems)
- Multi-tenant distributed deployments

---

## Core Principles

- AI is **not trusted by default**
- All actions pass through a **policy enforcement layer**
- Intelligence is separated from execution
- Every action is **auditable and traceable**
- Governance is **modular, scalable, and configurable**

---

## Feature List

### Core AI System
- Local-first AI runtime supporting open-source LLMs
- Optional cloud model integration through policy gateway
- Multi-model orchestration with task-based routing
- Context-aware AI engine with controlled memory boundaries
- Role-based AI profiles (Child, Teen, Pre-Teen Guided, Mature Minor, Adult)
- Age-based AI behavior adaptation

---

### Age-Based Governance System (Movie-Style Ratings)
- K (Kids)
- T (Teen)
- PG (Pre-Teen Guided)
- M (Mature Minor)
- A (Adult)

- Policy-driven system controlling AI, web, and system access
- Strict separation between under-18 and 18+ profiles
- No monitoring or reporting for Adult (A) profiles
- AI behavior dynamically adapts based on assigned category

---

### Policy & Guardrail Engine
- Real-time enforcement of AI inputs, outputs, and tool usage
- Rule-based + semantic hybrid policy system
- Content classification system:
  - Educational, Productivity, Entertainment, Social Media, Gaming
  - Violence (tiered), Adult Content, Gambling, Drugs, Self-harm, Misinformation
- Dynamic policy matrix mapping age categories to permissions
- Hard-block and soft-warning enforcement modes

---

### Parental Control System
- Household admin dashboard
- Website blocklists and allowlists per profile
- Category-based internet filtering
- Time-based usage limits (bedtime, study schedules, quotas)
- Emergency system-wide lockout mode
- Secure admin authentication required for configuration

---

### Web Access Control & Filtering
- DNS-level domain filtering
- Network-layer enforcement independent of AI layer
- Browser-level URL interception
- AI-generated links validated against policy before display
- Safe Search enforcement integration
- Prevention of bypass via alternate browsers or network routes

---

### AI Action & Execution Framework
- Controlled execution pipeline:
  - AI Intent → Policy Evaluation → Authorization → Execution
- Plugin-based tool system (file, web, system integrations)
- Sandboxed execution environment
- No direct AI system access
- Full audit logging of all actions

---

### Parental Activity Reporting (Under-18 Only)
- Reports available only for profiles under 18
- No monitoring for Adult (A) profiles
- On-demand, scheduled, and event-based reporting
- Includes:
  - AI usage summaries
  - Website activity and blocked attempts
  - Application usage and time tracking
  - Policy violations and alerts
- Configurable detail levels (summary, standard, detailed, safety-only)
- Secure admin authentication required
- Immutable audit log source

---

### Monitoring & Transparency Layer
- Append-only activity logs for under-18 profiles
- Explainable AI decisions for blocked/allowed actions
- Usage analytics per profile
- Exportable audit reports
- Real-time or scheduled monitoring dashboards

---

### Multi-User Household System
- Multiple isolated user profiles
- Data and memory separation per profile
- Admin-controlled configuration system
- Secure override and recovery mechanisms
- No cross-profile memory leakage

---

### Safety & Risk Detection
- Detection of self-harm, abuse, and high-risk content
- Hybrid filtering (rule-based + semantic AI)
- Configurable safety strictness by age category
- Emergency intervention mode
- Escalation alerts for guardians or admins

---

### OS-Level Integration Layer
- Cross-platform support (Windows, macOS, Linux)
- Application-level access control
- File system permissions with AI mediation
- Network and internet control per profile
- Focus mode and distraction blocking
- System-level enforcement independent of AI runtime

---

### Extensibility & Developer Framework
- Plugin-based architecture for tools and policies
- Policy scripting layer for advanced customization
- API gateway for external integrations
- Modular system for replacing AI models or policy engines
- Event-driven architecture for real-time extensions
- AGPL-3.0+ licensed core

---

### Performance & Architecture
- Lightweight, low-latency core system
- Hardware-aware optimization (CPU/GPU/quantized models)
- Offline-first operation with optional cloud scaling
- Sandboxed AI execution environment
- Scalable from single device to enterprise clusters

---

### Enterprise Scalability
- Multi-tenant architecture (household, organization, enterprise)
- Centralized policy orchestration across fleets
- Role-based and attribute-based access control (RBAC/ABAC)
- Horizontal scaling across distributed systems
- High availability and failover support
- API-first enterprise integration design

---

### Security Model
- Zero-trust architecture between all system layers
- Policy-enforced execution (no direct AI-to-system control)
- Encrypted communication between modules
- Signed policy updates and configuration changes
- Tamper-resistant audit logging
- Full traceability of system actions

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
  - [https://roxanneardary.com/kova/](https://roxanneardary.com/kova/)  

---

## License & Notice Requirements

Kova is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
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
