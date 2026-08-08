# DecisionAI

**Informed Choices. Confident Action.**

DecisionAI is an open-source AI financial intelligence platform designed to simplify investment disclosures, explain shareholder voting, evaluate investment risk, and analyze the foreseeable future through financial, market, innovation, governance, and regulatory intelligence.

The platform uses a modular architecture in which foundational capabilities are organized into independent core modules, while specialized capabilities can be added through optional plugin modules. This allows DecisionAI to remain extensible without requiring every deployment to use every intelligence capability.

---

## Core Objectives

DecisionAI is designed to help users:

- Understand what an investment actually contains and represents
- Translate complex financial disclosures into plain English
- Understand shareholder and investment votes before making a decision
- Compare the implications of different voting outcomes
- Evaluate portfolio risk during volatile conditions
- Identify safer financial paths based on available evidence
- Analyze current sales, market, and industry trends
- Track discovery, research, development, and innovation progress
- Evaluate foreseeable future scenarios
- Monitor laws and regulations affecting investments and sectors
- Automatically revise projections when significant regulatory changes occur
- Identify hidden dependencies and systemic risks
- Understand how corporate governance affects investments
- Trace AI conclusions back to their underlying sources
- Maintain an auditable history of forecasts, recommendations, and changes

---

# Modular Architecture

DecisionAI follows a modular architecture designed to separate foundational intelligence from specialized capabilities.

## Core Modules

Core modules provide the primary functionality required for DecisionAI. They are designed to operate independently where practical and communicate through defined interfaces and shared data structures.

### 1. Disclosure Intelligence Module

Processes and analyzes investment and corporate disclosure documents.

Features include:

- SEC filing analysis
- Annual report analysis
- Quarterly report analysis
- Prospectus analysis
- Fund disclosure analysis
- Corporate financial statement analysis
- Risk-factor extraction
- Fee and expense identification
- Revenue structure analysis
- Debt and obligation identification
- Governance disclosure extraction
- Material event identification
- Plain-English disclosure summaries
- Important disclosure change detection
- Disclosure comparison across reporting periods
- Source citation and document traceability

---

### 2. Investment Intelligence Module

Analyzes individual investments and their underlying characteristics.

Features include:

- Investment profile generation
- Historical performance analysis
- Volatility analysis
- Liquidity analysis
- Diversification analysis
- Credit and financial-strength indicators
- Sector exposure analysis
- Geographic exposure analysis
- Revenue exposure analysis
- Business-model analysis
- Risk-factor aggregation
- Investment dependency analysis
- Investment comparison
- Investment-level risk scoring

---

### 3. Portfolio Intelligence Module

Evaluates investments collectively rather than treating each holding independently.

Features include:

- Portfolio risk analysis
- Portfolio diversification analysis
- Concentration detection
- Sector concentration analysis
- Geographic concentration analysis
- Correlation analysis
- Hidden correlation detection
- Shared supplier exposure detection
- Shared market dependency detection
- Portfolio liquidity analysis
- Systemic exposure analysis
- Risk contribution analysis
- Portfolio stress testing
- Volatility monitoring
- Safer-path analysis during volatile conditions

---

### 4. Trend Intelligence Module

Evaluates current and historical trends that may influence investments.

Features include:

- Sales trend analysis
- Revenue trend analysis
- Market-share trends
- Customer adoption trends
- Product adoption trends
- Industry growth trends
- Regional sales trends
- Demand trends
- Competitive trends
- Pricing trends
- Supply and demand changes
- Industry-cycle analysis
- Trend acceleration and deterioration detection
- Trend divergence detection

---

### 5. Discovery & Progress Intelligence Module

Tracks developments that may affect the foreseeable future of an investment.

Features include:

- Research and development tracking
- Patent activity analysis
- Product development tracking
- Discovery pipeline monitoring
- Clinical trial and development milestone tracking where applicable
- Regulatory approval progress
- Product launch tracking
- Technology adoption tracking
- Innovation progress analysis
- Research publication monitoring
- Development milestone forecasting
- Discovery-to-market progression analysis

---

### 6. Foreseeable Future Forecasting Module

Provides forward-looking analysis based on available evidence rather than relying exclusively on historical performance.

Features include:

- Adjustable forecasting horizons
- Short-term forecasting
- Medium-term forecasting
- Long-term trend analysis
- Conservative scenarios
- Expected scenarios
- Aggressive-growth scenarios
- Crisis scenarios
- Multi-scenario comparison
- Forecast confidence measurements
- Forecast uncertainty ranges
- Trend-based projections
- Sales-based projections
- Discovery and innovation-based projections
- Market-condition projections
- Event-driven forecast revisions
- Historical forecast accuracy tracking

Forecasts should clearly distinguish between observed facts, model projections, assumptions, and uncertainty.

---

### 7. Governance & Voting Intelligence Module

Explains investment-related voting decisions in terms that ordinary investors can understand.

Features include:

- Shareholder proposal analysis
- Proxy statement analysis
- Voting-item summaries
- Plain-English voting explanations
- Yes-vote outcome descriptions
- No-vote outcome descriptions
- Short-term voting implications
- Long-term voting implications
- Governance impact analysis
- Executive compensation proposal analysis
- Merger and acquisition proposal analysis
- Corporate governance proposal analysis
- Shareholder-rights analysis
- Historical voting behavior analysis
- Shareholder-pressure analysis

#### Vote Simulation Sandbox

The module can model potential consequences associated with different voting outcomes.

Users can examine:

- What may happen if a proposal passes
- What may happen if a proposal fails
- Potential governance changes
- Potential financial implications
- Potential strategic implications
- Potential regulatory implications
- Potential long-term effects

The system should present simulations as scenarios rather than guaranteed outcomes.

#### Power Structure Mapping

Maps the distribution of corporate influence.

Features include:

- Institutional ownership mapping
- Insider ownership mapping
- Major shareholder identification
- Voting-power analysis
- Shareholder concentration
- Voting bloc analysis
- Corporate control visualization

---

### 8. Regulatory Intelligence Module

Continuously monitors laws, regulations, regulatory actions, and policy developments that may affect investments.

Features include:

- Federal law monitoring
- State law monitoring
- International law monitoring
- Sector-specific regulation monitoring
- Regulatory agency monitoring
- Regulatory rule changes
- Legislative proposal tracking
- Regulatory enforcement monitoring
- Effective-date tracking
- Jurisdiction mapping
- Sector-to-law relationship mapping
- Investment-to-regulation relationship mapping
- Plain-English legal summaries
- Regulatory impact identification

#### Policy Pipeline Intelligence

Tracks legislation and policy developments before they become law.

Features include:

- Proposed legislation tracking
- Bill progression monitoring
- Committee progression
- Legislative status changes
- Regulatory proposal monitoring
- Policy momentum analysis
- Potential impact identification
- Probability modeling where sufficient evidence exists
- Early-warning alerts

Probabilities must be clearly identified as model estimates rather than facts.

#### Law Timeline Replay

Allows users to examine historical and hypothetical regulatory scenarios.

Features include:

- Historical law timelines
- Effective-date analysis
- Historical portfolio exposure
- What-if regulatory scenarios
- Retrospective regulatory analysis
- Historical forecast comparison

#### Regulatory Impact Engine

Connects regulatory changes to affected investments and forecasts.

When a relevant law or regulation changes, the system can:

- Identify affected investments
- Identify affected sectors
- Identify affected geographic regions
- Identify affected business activities
- Recalculate relevant risk factors
- Revise applicable forecasts
- Update scenario assumptions
- Flag affected voting decisions
- Preserve the previous forecast for comparison
- Record the reason for the revision

---

### 9. Risk & Scenario Intelligence Module

Provides deeper analysis of financial and systemic risks.

Features include:

- Volatility analysis
- Liquidity risk analysis
- Concentration risk
- Credit risk indicators
- Regulatory risk
- Market risk
- Sector risk
- Geographic risk
- Operational risk indicators
- Supply-chain risk
- Geopolitical exposure
- Discovery and innovation risk
- Event-shock modeling

#### Cascade Risk Modeling

Analyzes how events affecting one company or sector may spread through connected investments.

Examples include:

- Supplier disruption
- Commodity-price changes
- Interest-rate changes
- Credit-market stress
- Sector downturns
- Regulatory changes
- Supply-chain disruptions
- Major corporate failures

#### Hidden Correlation Engine

Identifies relationships that may not be obvious from portfolio categories alone.

Examples include:

- Shared suppliers
- Shared customers
- Shared financing dependencies
- Shared geographic exposure
- Shared regulatory exposure
- Shared commodities
- Shared technology infrastructure
- Shared economic drivers

---

### 10. Explainability & Evidence Module

Provides transparency into how DecisionAI reaches its conclusions.

Features include:

- Source tracing
- Filing citations
- Regulatory source citations
- Data timestamps
- Forecast assumptions
- Model inputs
- Confidence indicators
- Uncertainty indicators
- Evidence classification
- “Explain this decision” functionality
- Contradiction detection
- Historical comparison
- AI output audit trails

The system should distinguish between:

- Verified source information
- Historical information
- Current observations
- Model-generated projections
- Scenario assumptions
- AI interpretation
- Uncertainty

---

### 11. Intelligence Ingestion Module

Provides a common ingestion layer for information used by the other core modules.

Potential data sources include:

- SEC EDGAR
- Government datasets
- Legislative databases
- Regulatory agency publications
- Financial market data
- Corporate filings
- Patent databases
- Research publications
- Company disclosures
- Industry data
- Public news sources
- Other legally accessible datasets

Features include:

- Scheduled ingestion
- Real-time or near-real-time ingestion where supported
- Source validation
- Duplicate detection
- Document versioning
- Data normalization
- Timestamping
- Provenance tracking
- Change detection
- Data-quality monitoring

---

### 12. Alert & Monitoring Module

Continuously monitors information relevant to the user's investments.

Features include:

- New disclosure alerts
- Material-change alerts
- Forecast revision alerts
- Regulatory alerts
- Legislative alerts
- Voting deadline alerts
- Risk alerts
- Volatility alerts
- Investment deterioration alerts
- Discovery milestone alerts
- Sales trend alerts
- Portfolio exposure alerts

---

### 13. Audit & Decision History Module

Maintains a historical record of DecisionAI's analysis.

Features include:

- Recommendation history
- Forecast history
- Forecast revision history
- Regulatory change history
- Voting analysis history
- Data-source history
- Model-version tracking
- Decision timestamps
- User action history
- Audit trails
- Historical comparison tools

This allows users to determine what DecisionAI knew, when it knew it, and how its conclusions changed as new information became available.

---

# Optional Plugin Modules

Optional plugins extend DecisionAI without requiring specialized functionality in every installation.

Plugins should use documented interfaces and should not require modifications to unrelated core modules.

### Potential Plugin Categories

#### Alternative Data Plugins

- Industry-specific datasets
- Commodity data
- Supply-chain data
- Economic datasets
- Public procurement data
- Specialized market indicators

#### Sector Intelligence Plugins

- Healthcare
- Biotechnology
- Energy
- Technology
- Financial services
- Real estate
- Manufacturing
- Transportation
- Agriculture
- Telecommunications
- Consumer goods
- Utilities

Sector plugins can provide specialized terminology, datasets, risk models, regulatory mappings, and forecasting factors.

#### Legal & Regulatory Plugins

- Federal regulatory intelligence
- State regulatory intelligence
- International regulatory intelligence
- Sector-specific legal databases
- Regulatory enforcement tracking
- Jurisdiction-specific analysis

#### Forecasting Plugins

- Alternative forecasting models
- Sector-specific forecasting models
- Economic forecasting
- Commodity forecasting
- Demand forecasting
- Scenario models
- Custom institutional models

#### Governance Plugins

- Specialized voting analysis
- Institutional voting behavior
- Proxy analysis
- Shareholder activism tracking
- Corporate control analysis

#### Market Intelligence Plugins

- Market sentiment
- News analysis
- Competitive intelligence
- Industry-cycle analysis
- Market discovery tracking

#### Visualization Plugins

- Advanced portfolio graphs
- Risk maps
- Regulatory heatmaps
- Corporate power maps
- Dependency graphs
- Forecast timelines
- Systemic-risk networks

#### Notification Plugins

- Email notifications
- Desktop notifications
- Mobile notifications
- Messaging integrations
- Custom webhook integrations

#### AI Model Plugins

- Local LLMs
- Specialized financial models
- Specialized legal models
- Local embedding models
- Custom classification models
- User-hosted inference systems

Plugins should remain optional so that users can operate DecisionAI with locally hosted or minimal configurations where appropriate.

---

# Plugin Architecture Principles

DecisionAI plugins should:

- Have clearly defined interfaces
- Be independently installable
- Declare dependencies
- Declare required data sources
- Declare required permissions
- Maintain source provenance
- Preserve auditability
- Avoid modifying unrelated core modules
- Support versioning
- Fail safely when unavailable
- Clearly identify plugin-generated analysis
- Respect user privacy
- Avoid unnecessary external data transmission

Plugin-generated forecasts and recommendations should remain distinguishable from core DecisionAI analysis.

---

# AI Safety, Accuracy & Transparency

DecisionAI is intended to provide financial intelligence, analysis, education, and decision-support information.

It should not represent probabilistic forecasts as guaranteed outcomes.

The system should:

- Identify uncertainty
- Display supporting evidence
- Identify assumptions
- Preserve source provenance
- Distinguish facts from projections
- Record model versions
- Record data timestamps
- Identify stale or incomplete data
- Flag conflicting information
- Avoid fabricated sources
- Avoid presenting unsupported conclusions as facts
- Preserve historical forecasts for later evaluation

Financial, legal, regulatory, and market information should be independently verified when decisions have significant consequences.

---

# Privacy & Security

DecisionAI should follow a privacy-first architecture.

Core security objectives include:

- Encryption of sensitive information
- Secure authentication
- Authorization controls
- Role-based access control where required
- Secure credential management
- Audit logging
- Data minimization
- Configurable data retention
- Secure API communications
- Local deployment support
- Self-hosting support
- Separation of user data from public intelligence datasets

---

# Technology Architecture

The initial architecture may use:

### Frontend

- Next.js
- React
- TypeScript
- Tailwind CSS
- Recharts
- D3.js

### Backend

- Python
- FastAPI
- Pydantic
- PostgreSQL
- Redis
- Celery

### AI & Machine Learning

- Large language models
- Hugging Face Transformers
- Embedding models
- Retrieval-augmented generation
- Document processing pipelines
- Statistical forecasting
- Time-series models
- Machine-learning forecasting models

### Infrastructure

- Docker
- Docker Compose for development and smaller deployments
- Kubernetes for larger deployments where appropriate
- Nginx
- GitLab CI/CD

The architecture should remain model-agnostic wherever practical so that users and contributors can integrate different AI models and forecasting systems.

---

# Development Principles

DecisionAI development should prioritize:

- Modularity
- Open-source software
- Transparency
- Explainability
- Reproducibility
- Source provenance
- Privacy
- Security
- Data quality
- Model accountability
- Human oversight
- Vendor independence
- Local and self-hosted deployment
- Extensibility through plugins

No single AI provider, financial data provider, regulatory data provider, or cloud platform should become an unnecessary architectural dependency.

---

# Future Development

Potential future capabilities include:

- More sophisticated systemic-risk modeling
- Expanded international regulatory intelligence
- Additional sector intelligence plugins
- Improved forecasting validation
- Community-developed forecasting models
- Local AI deployment improvements
- Advanced portfolio simulation
- Expanded corporate governance intelligence
- Additional alternative-data integrations
- Automated forecast accuracy evaluation
- Community-maintained regulatory mappings

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
  - [https://roxanneardary.com/decisionai/](https://roxanneardary.com/decisionai/)

---

## License & Notice Requirements

DecisionAI is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- DecisionAI specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments. Any updates that add contributors or modify attribution must also update `notice.md`.  
- When submitting a pull request, ensure that any new files maintain attribution requirements where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, refer to the AGPL-3.0+ license and the `notice.md` file.
