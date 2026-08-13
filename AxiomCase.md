# AxiomCase

**Know what happened. Know what to do.**

AxiomCase is a modular, state-aware consumer dispute intelligence system that transforms raw complaints into structured case files, maps them to jurisdiction-specific consumer protection laws, and generates actionable resolution pathways.

It is designed to help users understand disputes clearly, organize evidence, and identify practical next steps across all U.S. states.

---

## Core Features

### 1. Case Intake & Structuring
- Converts freeform complaint text into structured case files
- Extracts parties, transactions, dates, and key events
- Builds a unified timeline of dispute activity
- Separates facts, claims, and user-provided context

---

### 2. Evidence Processing
- Supports receipts, invoices, emails, and chat logs
- OCR extraction for scanned or image-based documents
- Links evidence directly to timeline events
- Flags missing or conflicting documentation

---

### 3. State-Aware Legal Mapping
- Accepts any U.S. state as jurisdiction input
- Loads relevant consumer protection statutes per state
- Maps case facts to applicable legal frameworks
- Includes consumer protection agency references
- Maintains modular, extensible legal dataset per jurisdiction

---

### 4. Issue Detection & Classification
- Identifies potential dispute categories:
  - billing errors
  - deceptive practices
  - unauthorized charges
  - service misrepresentation
  - tax misapplication
- Assigns confidence levels to detected issue types
- Clearly separates user claims vs inferred issues
- Avoids definitive legal conclusions

---

### 5. Resolution Path Engine
- Generates structured next-step options:
  - merchant dispute resolution steps
  - refund request frameworks
  - chargeback guidance paths
  - regulatory escalation routes
- Prioritizes resolution paths by likelihood of success
- Adapts recommendations based on jurisdiction rules

---

### 6. Consumer Protection Routing
- Maps cases to appropriate agencies such as:
  - state consumer protection divisions
  - attorney general offices
- Generates submission-ready complaint summaries
- Provides structured filing templates
- Includes industry-specific escalation guidance when applicable

---

### 7. Public Accountability Summary Generator
- Produces neutral, structured case summaries
- Separates:
  - verified facts
  - user-reported claims
  - business responses
  - corrected vs unresolved issues
- Maintains chronological transparency of events
- Designed for documentation, not accusation

---

### 8. Dispute Timeline Engine
- Constructs chronological dispute reconstruction
- Tracks charge changes, corrections, and adjustments
- Highlights escalation points
- Visualizes progression from issue → resolution

---

### 9. Case Intelligence Layer
- Detects patterns across similar disputes
- Identifies missing evidence that may strengthen cases
- Provides probabilistic resolution insights
- Supports structured reasoning over historical case patterns

---

### 10. Export & Reporting Tools
- Export case files as structured JSON or PDF reports
- Generate consumer dispute dossiers for escalation
- Produce credit card dispute summaries
- Maintain versioned case history archives

---

### 11. Modular Architecture (AGPL-Friendly Design)
- Fully self-hostable system
- Plugin-based legal dataset ingestion
- Extensible state-by-state rule system
- Designed for local-first or server deployment
- API-first architecture for integration

---

### 12. Transparency & Safety Layer
- Separates facts, claims, and AI analysis
- No definitive legal conclusions
- No assertions of wrongdoing as fact
- Evidence-weighted reasoning outputs
- Fully traceable reasoning chain for outputs

---

## System Identity

**AxiomCase — Know what happened. Know what to do.**

A structured intelligence layer that turns consumer disputes into clear, actionable, jurisdiction-aware case frameworks.

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
  - [https://roxanneardary.com/axiomcase/](https://roxanneardary.com/axiomcase/)

---

## License & Notice Requirements

AxiomCase is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- AxiomCase specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  
