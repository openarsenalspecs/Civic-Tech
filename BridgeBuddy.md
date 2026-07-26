# BridgeBuddy  
### Gentle guidance, always with you.

BridgeBuddy is a secure, AI-guided onboarding and assistance platform designed to help senior citizens safely navigate and access U.S. government services. It breaks complex systems into simple, step-by-step instructions with full user confirmation at every stage, supported by a friendly AI assistant and optional personalized Chibi companion.

---

## 🧭 Overview

Government systems are often fragmented, complex, and difficult to navigate—especially for seniors. BridgeBuddy solves this by transforming every process into:

- One step per screen  
- One instruction or question at a time  
- Large, readable interface design  
- Voice and text guidance  
- Confirmation required before every action  

It acts as a **guided trust layer between users and government services**.

---

## 🌉 Core Features

### 🤖 AI Step-by-Step Guidance
- Breaks down government processes into simple steps  
- Translates legal/government language into plain English  
- Waits for user confirmation before continuing  
- Provides clarification when users are confused  
- Slows pacing automatically based on user behavior  

---

### 🧾 Secure Identity Vault
- Encrypted storage of sensitive identity documents  
- Supports:
  - Real ID / driver’s license  
  - Social Security card (SSN verification)  
  - Bank statements (30-day validation use case)  
  - Payment card verification tokens  
- Field-level encryption for sensitive data  
- Audit logging for all access  
- Reusable “Verified Identity Credential” system  

---

### 🧩 Government Program Modules (Plugin System)
Modular workflows for government services including:

- IRS account setup and access  
- Social Security Administration (SSA) services  
- Medicare enrollment  
- Medicaid (state-based modules)  
- SNAP benefits  
- Section 8 housing assistance  
- VA benefits  
- Senior tax relief programs  

Each module includes:
- eligibility rules  
- required documents  
- step-by-step guided workflows  
- fallback manual instructions when APIs are unavailable  

---

### 🏛 State Extension System
- States can build custom modules  
- Override federal workflows where needed  
- Add local senior assistance programs  
- Connect to state-specific portals  
- Example: New Jersey senior benefits integrations  

---

### 🎭 Chibi Companion Interface
A personalized visual assistant that guides users through every step.

**Features:**
- Upload photo → auto-generated chibi avatar  
- Custom chibi builder with styles and personality options  
- Persistent companion across all services  
- Step narration and visual guidance  
- Confirmation pauses at every step  
- Adaptive pacing based on user comfort  

Personality modes:
- Calm Guide  
- Cheerful Helper  
- Formal Assistant  
- Slow-Paced Tutor  

---

### 🔐 Security & Privacy Architecture
- End-to-end encryption  
- Zero-trust access model  
- Minimal data retention policies  
- Secure document handling pipeline  
- Full access audit logs  
- Separation of identity verification and raw data storage  

---

### 🧭 Step-Based UI System
- One action per screen  
- Large text optimized for seniors  
- High-contrast accessibility design  
- Voice-enabled navigation  
- Explicit confirmation before progression  
- No multi-step forms or hidden flows  

---

### 🧠 AI Workflow Control System
- AI acts as a controlled guide, not an autonomous agent  
- Workflow state machine enforces process integrity  
- Prevents skipping or mis-execution of steps  
- Ensures safe progression through sensitive actions  

---

## 🧩 System Architecture (High Level)

- Frontend: Step-based UI + accessibility-first design  
- AI Layer: Instruction + reasoning controller  
- Workflow Engine: State machine for all processes  
- Identity Vault: Secure encrypted credential system  
- Module System: Plugin-based government integrations  
- Chibi Layer: Emotional UI companion interface  

---

## 🚀 Vision

BridgeBuddy is designed to become a universal access layer for essential public services, ensuring that no one is excluded due to complexity, confusion, or digital barriers.

It replaces fragmentation with guidance, and complexity with clarity.

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
  - [https://roxanneardary.com/bridgebuddy/](https://roxanneardary.com/bridgebuddy/)

---

## 📜 License & Notice Requirements

BridgeBuddy is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- BridgeBuddy specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's `notice.md` file tracks attribution requirements and contributor acknowledgments. Any updates that add or modify contributors must also update `notice.md`.  
- When submitting a pull request, ensure all new files maintain required attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.  

For full legal details, refer to the AGPL-3.0+ license and the `notice.md` file.

---

## 🤝 Contributing

Contributions are welcome. Please ensure:
- You follow AGPL-3.0+ licensing terms  
- You maintain accessibility-first design principles  
- You preserve step-by-step UX integrity  
- You update documentation where necessary  
