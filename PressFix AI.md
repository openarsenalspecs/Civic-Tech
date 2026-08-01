# PressFix AI

PressFix AI is an open-source WordPress optimization engine that analyzes site structure, performance, SEO signals, and Google Search Console issues to generate clear, explainable, and actionable optimization recommendations.

It is designed around a **human-in-the-loop decision system**, ensuring no changes are applied automatically without user approval.

**Tagline:**  
Optimization without guesswork.

---

# Core Philosophy

PressFix AI is built on three principles:

- **No guesswork** — recommendations are grounded in real site data
- **No blind automation** — users remain in control of every decision
- **Explainable optimization** — every suggestion includes reasoning and impact

---

# Features

## 🧠 Site Intelligence Engine
- Scans active WordPress theme and plugins
- Detects performance bottlenecks
- Evaluates content depth and structure
- Identifies navigation complexity issues
- Basic UX and layout heuristics analysis

---

## ⚡ Performance Optimization Analysis
- Detects missing caching layers
- Identifies image optimization gaps
- Flags render-blocking issues (heuristic-based)
- Evaluates plugin load impact
- Suggests performance-focused plugin improvements

---

## 🔍 SEO & Indexing Insights
- Detects SEO configuration gaps
- Identifies missing metadata patterns
- Flags structural SEO issues
- Evaluates content distribution and depth
- Integrates Search Console issue analysis (via upload or API)

---

## 📊 Google Search Console Integration
- Upload CSV exports from Google Search Console
- Normalize and categorize issues:
  - Indexing problems
  - Crawl errors
  - Mobile usability issues
  - Core Web Vitals signals
- Maps issues to root causes
- Generates fix recommendations per issue type

---

## 🛠️ Fix Engine (Core System)
- Converts detected issues into structured fixes
- Separates:
  - Plugin-based fixes
  - Theme/code-level fixes
- Provides step-by-step remediation guidance
- Supports bulk issue resolution grouping

---

## 🔌 Plugin Recommendation System
- Controlled plugin dataset (no uncontrolled AI hallucinations)
- Categorized recommendations:
  - SEO plugins
  - Performance optimization plugins
  - Redirect management tools
  - Accessibility enhancements
- Compatibility-aware filtering
- Performance impact awareness

---

## 🧩 Human-in-the-Loop Decision System
- Every recommendation requires user approval
- No automatic installation or configuration changes
- Clear “Approve / Skip” decision flow
- Each fix includes:
  - Explanation
  - Expected impact
  - Risk level

---

## 🤖 AI Explanation Layer (Optional)
- Provides natural language explanations
- Prioritizes issues by severity and impact
- Helps users understand technical problems
- Does not override deterministic logic

---

## 🧭 Issue Prioritization Engine
- Ranks issues by:
  - SEO impact
  - Performance impact
  - Site visibility importance
- Highlights critical vs low-priority issues
- Groups related problems into actionable clusters

---

## 🧪 Safety & Control Systems
- No autonomous plugin installation
- No automatic site changes
- All actions require explicit approval
- Transparent recommendation logic

---

# Architecture Overview

- **Analyzer** → collects site data
- **GSC Parser** → imports Search Console issues
- **Issue Mapper** → converts issues into structured fixes
- **Fix Engine** → generates remediation steps
- **Plugin Dataset** → controlled recommendation source
- **API Layer** → exposes endpoints
- **Admin UI** → dashboard and review interface

---

# Example Workflow

1. Install PressFix AI plugin
2. Run site analysis
3. Review optimization report
4. Upload Search Console issues (optional)
5. View mapped fixes and plugin recommendations
6. Approve or reject each fix manually
7. Apply changes selectively

---

# Roadmap

- Real-time Search Console API integration
- Automatic theme-level issue detection
- Plugin auto-configuration after approval
- Continuous site monitoring mode
- Self-hosted AI model support
- Multi-site management dashboard

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
  - [https://roxanneardary.com/pressfixai/](https://roxanneardary.com/pressfixai/)

---

## License & Notice Requirements

PressFix AI is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- PressFix AI specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's `notice.md` file tracks attribution requirements and contributor acknowledgments. Any update that adds new contributors or modifies attribution must also update `notice.md`.
- When submitting changes, ensure attribution headers are preserved where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, refer to the AGPL-3.0+ license and the `notice.md` file.
