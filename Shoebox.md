# Shoebox+

**Your Health Savings, Optimized.**

## Overview

Shoebox+ is an open-source, AI-powered Health Savings Account (HSA) optimization platform designed to help users understand, manage, and maximize the long-term financial value of their HSA.

Rather than treating an HSA solely as a spending account, Shoebox+ helps users coordinate contributions, qualified medical expenses, receipt preservation, reimbursement planning, investment strategies, employer benefits, and financial institution selection. The system continuously evaluates the user's circumstances and available strategies to help identify opportunities for improved tax efficiency and long-term growth.

Shoebox+ is designed around a modular architecture. Core modules provide the fundamental HSA management and optimization capabilities, while optional plugin modules extend the platform with additional integrations, data sources, financial services, AI providers, and specialized functionality.

## Design Principles

Shoebox+ is built around the following principles:

- **User-controlled financial data**
- **Open-source transparency**
- **Modular architecture**
- **Local-first data management where practical**
- **AI-assisted decision making**
- **Explainable recommendations**
- **Source-backed tax and regulatory information**
- **Continuous strategy reassessment**
- **Human approval before consequential actions**
- **Interoperability and vendor independence**
- **Privacy and security by design**

## Core Specification

Shoebox+ provides a unified system for collecting financial and medical expense information, maintaining supporting documentation, evaluating HSA strategies, and presenting actionable recommendations.

The platform does not assume that one strategy is optimal for every user. Instead, the AI evaluates the user's objectives, financial circumstances, HSA configuration, available benefits, applicable tax rules, account characteristics, and risk preferences to co-create potential strategies with the user.

---

# Core Modules

## 1. User Profile & Financial Data Module

Maintains the structured information required to evaluate HSA strategies.

### Features

- Secure user account management
- User financial profile
- Income information
- Tax filing status
- Applicable tax jurisdiction
- HSA eligibility information
- HSA contribution information
- Employer contributions
- Current HSA balance
- HSA investment balance
- Medical spending patterns
- Reimbursement preferences
- Investment preferences
- Risk tolerance
- Financial objectives
- User-defined constraints
- Historical financial data
- Structured data import and export

---

## 2. Receipt & Medical Expense Module

Provides the foundation for the Shoebox strategy by preserving documentation associated with qualified medical expenses.

### Features

- Receipt uploads
- Image uploads
- PDF uploads
- Digital document uploads
- Receipt OCR
- Medical expense data extraction
- Date-of-service extraction
- Provider extraction
- Amount extraction
- Payment method recording
- Expense categorization
- Qualified-expense classification
- User verification of extracted information
- Duplicate receipt detection
- Missing-information detection
- Original document preservation
- Immutable document archiving
- Receipt metadata
- Expense records
- Reimbursement status tracking
- Reimbursement history
- Searchable receipt database
- Database retrieval by:
  - Date
  - Provider
  - Amount
  - Category
  - Reimbursement status
  - Expense status
- Receipt tagging
- User notes
- Document version history
- Audit trail

---

## 3. Shoebox Strategy Module

Manages long-term reimbursement planning based on preserved medical expense records.

### Features

- Track unreimbursed qualified medical expenses
- Maintain reimbursement eligibility records
- Calculate accumulated reimbursable expenses
- Model immediate reimbursement
- Model deferred reimbursement
- Compare reimbursement timing strategies
- Project potential HSA investment growth
- Estimate opportunity cost of reimbursement
- Maintain receipt-to-expense relationships
- Maintain expense-to-reimbursement relationships
- Generate reimbursement plans
- Generate reimbursement batches
- Identify receipts requiring additional documentation
- Track reimbursement history
- Preserve documentation supporting reimbursement decisions

The module is designed to distinguish between **recording an expense**, **establishing reimbursement eligibility**, and **actually withdrawing funds**.

---

## 4. HSA Contribution Optimization Module

Evaluates contribution opportunities based on applicable limits, tax treatment, employer contributions, and user objectives.

### Features

- Annual contribution limit tracking
- Coverage-type analysis
- Employer contribution tracking
- Employee contribution tracking
- Contribution deadline tracking
- Contribution utilization analysis
- Payroll contribution analysis
- Direct contribution analysis
- Contribution timing analysis
- Federal tax impact modeling
- State tax treatment modeling
- Payroll tax treatment modeling
- Contribution scenario comparison
- Remaining contribution capacity
- Excess contribution detection
- Contribution alerts
- Future contribution projections

The module evaluates the user's circumstances against the current applicable rules rather than relying on static assumptions.

---

## 5. Investment Optimization Module

Evaluates how HSA assets may be allocated according to the user's objectives, timeline, liquidity requirements, and risk tolerance.

### Features

- HSA investment account analysis
- Cash allocation analysis
- Investment allocation analysis
- Asset allocation modeling
- Risk tolerance assessment
- Investment horizon analysis
- Portfolio diversification analysis
- Fee analysis
- Historical performance analysis
- Scenario modeling
- Portfolio comparisons
- Rebalancing recommendations
- Liquidity analysis
- Long-term growth projections

### Portfolio Simulation & Risk Modeling

- Monte Carlo simulations
- Multiple return scenarios
- Volatility modeling
- Drawdown analysis
- Market stress testing
- Inflation scenarios
- Contribution scenarios
- Reimbursement scenarios
- Cash-versus-investment comparisons
- Long-term probability analysis
- User-defined assumptions
- Sensitivity analysis

Shoebox+ presents simulations as scenarios rather than guarantees of future investment performance.

---

## 6. Tax & IRS Intelligence Module

Maintains the regulatory knowledge required for HSA strategy evaluation.

### Features

- IRS rule monitoring
- HSA tax-rule monitoring
- Official IRS publication tracking
- Relevant statutory and regulatory source tracking
- Contribution-limit updates
- Qualified-expense rule updates
- Distribution-rule updates
- Reimbursement-rule updates
- Tax-treatment updates
- Payroll-tax treatment monitoring
- State tax treatment monitoring
- Regulatory change detection
- Rule versioning
- Effective-date tracking
- Historical rule preservation
- Source citations
- Strategy impact analysis
- User-specific change alerts

### Strategy Reassessment

When a material rule changes, Shoebox+ can reassess affected strategies and identify potential actions such as:

- Changing contribution amounts
- Changing contribution timing
- Reviewing reimbursement plans
- Reviewing account structures
- Reviewing investment allocations
- Reviewing employer benefit elections
- Reviewing financial institution choices
- Reviewing previously generated strategies

Recommendations require user review before consequential financial actions are taken.

---

## 7. AI Strategy Co-Creation Module

Provides the intelligence layer that coordinates the other core modules.

### Features

- Conversational financial planning
- User goal discovery
- Financial situation analysis
- HSA strategy generation
- Multiple strategy alternatives
- Strategy comparison
- Trade-off analysis
- Tax-effect modeling
- Growth modeling
- Risk analysis
- Liquidity analysis
- User preference incorporation
- User-defined constraints
- Explainable recommendations
- Source-backed recommendations
- Assumption disclosure
- Confidence indicators
- User approval workflows
- User rejection workflows
- Strategy revision
- Strategy history
- Decision history
- Recommendation audit trails

The AI does not simply produce a single answer. It can present alternative strategies and collaborate with the user to determine which strategy best fits the user's objectives and constraints.

---

## 8. Financial Institution Optimization Module

Evaluates HSA providers and account structures based on user-specific requirements.

### Features

- HSA provider research
- Account feature comparison
- Interest-rate comparison
- Account-fee comparison
- Investment-option comparison
- Investment-fee comparison
- Minimum-balance analysis
- Cash-management analysis
- Reimbursement capabilities
- Payroll integration analysis
- Transfer capabilities
- Account accessibility analysis
- Provider scoring
- User-specific provider ranking
- Provider change monitoring
- Fee-change monitoring
- Feature-change monitoring
- New-provider monitoring
- Opportunity detection
- Switching analysis
- Transfer and rollover research
- Estimated benefit of changing providers

The system can recommend reviewing or changing institutions when a materially better opportunity becomes available.

---

## 9. Employer Benefits Optimization Module

Evaluates employer-provided benefits that may interact with the user's HSA strategy.

### Features

- Employer HSA contribution analysis
- Employer contribution tracking
- Employer benefit-plan analysis
- Payroll contribution analysis
- HSA contribution optimization
- FSA interaction analysis
- Limited-purpose FSA analysis
- Employer incentive analysis
- Benefits election analysis
- Benefits comparison
- Open-enrollment planning
- Employer-benefit change alerts
- Total benefits optimization
- Employer-versus-individual contribution analysis

---

## 10. Analytics & Reporting Module

Transforms user data and strategy information into understandable reports.

### Features

- HSA balance reporting
- Contribution reporting
- Employer contribution reporting
- Medical expense reporting
- Reimbursement reporting
- Unreimbursed expense reporting
- Investment reporting
- Tax-impact estimates
- Strategy comparisons
- Historical performance tracking
- Projected growth
- Cash-flow analysis
- Portfolio analysis
- Financial institution comparisons
- IRS-rule impact reports
- CPA-ready reports
- Exportable reports
- CSV export
- PDF export
- Structured data export

---

## 11. Alerts & Monitoring Module

Continuously monitors the user's HSA environment for relevant changes.

### Features

- Contribution-limit alerts
- Contribution-capacity alerts
- IRS rule-change alerts
- Qualified-expense alerts
- Receipt alerts
- Missing-document alerts
- Duplicate-receipt alerts
- Reimbursement alerts
- Employer-benefit alerts
- Investment alerts
- Portfolio-rebalancing alerts
- Financial institution alerts
- Fee-change alerts
- Better-account opportunity alerts
- Open-enrollment reminders
- Strategy-review reminders

---

## 12. Knowledge & Community Module

Provides access to relevant knowledge while maintaining separation between verified regulatory information and community-generated information.

### Features

- HSA knowledge base
- Strategy library
- IRS source index
- Financial education resources
- Community strategy discussions
- Anonymized best-practice analysis
- Community-submitted strategies
- Strategy comparison
- Knowledge tagging
- Source classification
- Community content ratings
- Source credibility indicators
- AI-assisted knowledge retrieval

Community information is clearly distinguished from authoritative tax and regulatory sources.

---

## 13. Security, Privacy & Audit Module

Protects sensitive financial and medical expense information.

### Features

- Encryption at rest
- Encryption in transit
- Secure authentication
- Access controls
- Role-based permissions
- Session management
- Secure document storage
- Data minimization
- User-controlled data retention
- Data export
- Data deletion
- Audit logging
- AI recommendation logging
- Data-access logging
- Document-access logging
- Configuration history
- Strategy history
- Security event monitoring

---

# Optional Plugin Modules

Shoebox+ supports optional plugins that extend the core platform without requiring every installation to include every integration.

Plugins should have defined interfaces and must not compromise the integrity of the core strategy engine.

## AI Provider Plugins

Optional integrations with external or local AI systems.

### Examples

- Local language models
- Cloud AI providers
- Specialized financial reasoning models
- OCR AI providers
- Document intelligence services
- Embedding providers
- Retrieval systems

---

## Financial Institution Plugins

Connect Shoebox+ to supported financial institutions and HSA providers.

### Examples

- HSA account data synchronization
- Balance synchronization
- Transaction synchronization
- Investment-position synchronization
- Account-fee retrieval
- Provider feature retrieval
- Transfer information retrieval

---

## Receipt & Document Plugins

Extend document ingestion and processing.

### Examples

- Mobile camera integration
- Scanner integration
- Cloud document storage
- Advanced OCR
- Medical billing document parsing
- Email receipt ingestion
- Secure document synchronization

---

## Healthcare Data Plugins

Optional integrations for retrieving medical expense information.

### Examples

- Healthcare provider portals
- Pharmacy records
- Insurance explanation-of-benefits documents
- Medical billing systems
- Patient portals
- Health data standards

---

## Tax Data Plugins

Extend tax-rule and jurisdiction coverage.

### Examples

- Federal tax data
- State tax data
- Tax jurisdiction databases
- Legislative monitoring
- Regulatory publication feeds
- Tax research databases

---

## Employer Benefits Plugins

Connect to employer benefits systems where supported.

### Examples

- Benefits portals
- HSA payroll systems
- Employer contribution systems
- Open-enrollment systems
- Benefits-plan documents

---

## Notification Plugins

Provide additional notification channels.

### Examples

- Email
- SMS
- Push notifications
- Desktop notifications
- Calendar integrations

---

## Investment Data Plugins

Extend market and investment research capabilities.

### Examples

- Market-data providers
- Fund-data providers
- ETF data
- Mutual-fund data
- Portfolio analytics
- Risk-model providers

---

## Community Plugins

Allow installations to connect to optional community infrastructure.

### Examples

- Community knowledge repositories
- Strategy libraries
- Discussion systems
- Anonymized benchmarking
- Community contribution systems

---

# Plugin Architecture

Plugins should:

- Use documented interfaces
- Declare their capabilities
- Declare required permissions
- Declare external dependencies
- Respect user privacy settings
- Preserve auditability
- Avoid modifying authoritative tax rules directly
- Clearly identify external data sources
- Fail safely when unavailable
- Allow users to disable or remove them
- Maintain version compatibility
- Avoid vendor lock-in

Core Shoebox+ functionality must remain usable without optional plugins wherever practical.

---

# Data Architecture

Shoebox+ separates source documents from structured financial records.

A typical expense record may contain:

- Unique expense identifier
- User identifier
- Source document identifier
- Date of service
- Provider
- Expense category
- Amount
- Payment method
- Qualified-expense status
- Verification status
- Reimbursement status
- Reimbursement date
- Reimbursement amount
- Source references
- User notes
- Audit metadata

Original receipts and supporting documents are preserved separately from the structured records used by the AI and strategy engine.

---

# Strategy Lifecycle

Shoebox+ uses a continuous strategy lifecycle:

1. **Collect**
   - Gather user financial information and supporting documentation.

2. **Verify**
   - Validate extracted data and identify missing or conflicting information.

3. **Understand**
   - Evaluate the user's HSA, financial objectives, benefits, expenses, and constraints.

4. **Research**
   - Retrieve applicable tax rules, financial institution information, investment data, and other relevant sources.

5. **Model**
   - Calculate potential outcomes across multiple strategies.

6. **Co-Create**
   - Present alternatives and allow the user to adjust priorities and constraints.

7. **Recommend**
   - Produce explainable, source-backed recommendations.

8. **Approve**
   - Require user confirmation before consequential actions.

9. **Record**
   - Preserve the selected strategy, assumptions, sources, and decision history.

10. **Monitor**
    - Continuously monitor changes affecting the strategy.

11. **Reassess**
    - Recalculate strategies when user circumstances, markets, providers, or tax rules change.

---

# Accuracy & Regulatory Design

Shoebox+ is designed to distinguish between:

- Authoritative tax rules
- Regulatory guidance
- Financial institution data
- Market data
- Community information
- AI-generated analysis
- User-provided information
- Assumptions and projections

Recommendations should identify the information supporting them and disclose material assumptions.

Tax rules and financial information are time-sensitive. Shoebox+ should therefore associate relevant rules and recommendations with effective dates and source references rather than treating tax information as permanently static.

Shoebox+ is an educational and decision-support system. Users remain responsible for reviewing recommendations and determining whether a strategy is appropriate for their circumstances.

---

# Privacy & Data Ownership

Shoebox+ is designed to give users control over sensitive financial and medical-expense information.

The architecture supports:

- Local-first deployments
- Self-hosted deployments
- Encrypted storage
- User-controlled exports
- User-controlled deletion
- Optional external integrations
- Minimal external data transmission
- Transparent plugin permissions

External AI, financial, healthcare, or document services should only receive information required for the enabled functionality and permitted by the user's configuration.

---

# Contributing

Contributions are welcome in areas including:

- Core HSA functionality
- Receipt and document processing
- Tax-rule research
- Strategy modeling
- Investment simulations
- Financial institution research
- Employer benefit integrations
- Security
- Privacy
- Testing
- Documentation
- Optional plugins

See [CONTRIBUTING.md](CONTRIBUTING.md) for contribution requirements and development procedures.

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
  - [https://roxanneardary.com/shoebox/](https://roxanneardary.com/shoebox/)

---

## License & Notice Requirements

Shoebox+ is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- Shoebox+ specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  
