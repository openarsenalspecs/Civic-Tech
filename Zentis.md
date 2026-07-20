# Zentis

**Infrastructure for interpretive governance.**

Zentis is a dual-layer governance intelligence system designed to separate and analyze platform policy enforcement and legal risk exposure. It provides structured, explainable scoring of content under both policy rules and probabilistic legal interpretation, without making legal determinations.

---

## Core Concept

Modern digital platforms blend policy enforcement and legal interpretation into opaque systems. Zentis separates these domains into independent analytical layers:

- Platform policy compliance (what a system *chooses* to enforce)
- Legal risk modeling (what *may* create exposure under law)
- User-controlled governance context (how interpretation is applied)

Zentis does not decide law. It structures interpretation.

---

## Feature List

### 1. Dual Analysis Engine
- Independent **Policy Engine (PPIS)** and **Legal Risk Engine (LRPS)**
- Prevents conflation of platform rules and legal interpretation
- Modular scoring architecture for each layer

---

### 2. Policy Compliance System (PPIS)
- Parses platform-specific Terms of Service and community guidelines
- Detects likely policy violations
- Supports multiple policy profiles per platform
- Outputs:
  - Violation likelihood score (0–1)
  - Matched policy categories
  - Suggested moderation action (allow, label, limit, remove)

---

### 3. Legal Risk Probability System (LRPS)
- Classifies content into legal risk categories:
  - Defamation
  - Fraud indicators
  - Harassment signals
  - Threat/coercion patterns
  - Privacy risks
  - Copyright signals
- Produces probabilistic risk scores (not legal conclusions)
- Jurisdiction-aware modeling with default baseline assumptions

---

### 4. Jurisdiction Context Layer
- Supports region-aware interpretation (US, EU, and configurable extensions)
- Defaults to **United States federal baseline when unknown**
- Allows explicit jurisdiction override
- Applies conservative multi-jurisdiction interpretation when ambiguous

---

### 5. User Sovereignty & Control Layer
- User-configurable governance sensitivity settings
- Optional enabling/disabling of analysis layers
- Transparent scoring outputs
- Local-first or self-host deployment support
- No forced behavioral enforcement model

---

### 6. Citizen Publisher Framework
- Users are treated as independent content publishers within the system
- Clear separation of:
  - platform analysis
  - user responsibility
- System does not assume editorial ownership of user-generated content

---

### 7. Explainable AI Output Layer
- Human-readable reasoning for all flags and scores
- Evidence-based explanation traces
- Explicit uncertainty reporting
- Context gap identification (missing intent, missing jurisdiction, etc.)

---

### 8. Audit & Transparency System
- Versioned policy and scoring models
- Reproducible analysis outputs
- Full decision trace logging
- Audit-ready structured reports

---

### 9. Content Processing Pipeline
- Input normalization (language, format, context detection)
- Entity extraction (people, organizations, claims)
- Intent classification (informational, persuasive, harmful, etc.)
- Feature extraction for downstream scoring models

---

### 10. Modular Policy Packs
- Plug-in architecture for different platform policies
- Version-controlled rule sets
- Custom community guideline support
- Replaceable governance logic modules

---

### 11. Safety & Interpretation Boundary Layer
- Explicit separation of:
  - policy enforcement signals
  - legal risk estimates
  - non-authoritative explanations
- No binary legal conclusions permitted
- Designed to prevent over-assertion of legal authority

---

### 12. AGPL 3.0+ Open Governance Model
- Fully open-source core under AGPL 3.0+
- Required attribution to:
  - Roxanne Ardary
  - [roxanneardary.com](https://www.roxanneardary.com/)
- Forkable and auditable system design
- No proprietary enforcement lock-in

---

### 13. Multi-Output Reporting System
Each analysis produces structured outputs:
- Policy violation score
- Legal risk probability score
- Confidence score
- Explanation layer
- System flags
- Recommended actions (non-binding)

---

### 14. Extensible Governance API
- External plugin support for:
  - policy models
  - legal category extensions
  - third-party moderation systems
- Designed for interoperability and composability

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
  - [https://roxanneardary.com/zentis/](https://roxanneardary.com/zentis/)

---

## License & Notice Requirements

Zentis is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- Zentis specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
