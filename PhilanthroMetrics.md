# PhilanthroMetrics Specification

**Built in the Open. Trusted in the Real World.**

## Overview

PhilanthroMetrics is an open-source public utility for analyzing charitable organizations through publicly available financial disclosures, organizational information, public communications, and funding relationships.

The platform transforms fragmented public records into a transparent, searchable, comparable, and continuously updated view of charitable organizations.

PhilanthroMetrics evaluates how effectively an organization directs its revenue toward its stated charitable mission, tracks financial performance across multiple years, analyzes public communications for mission consistency, and maps relationships between charitable organizations through an interactive Impact Graph.

The system is built around a fundamental principle:

**Transparency and full disclosure should be the backbone of every charitable endeavor.**

PhilanthroMetrics does not rely on proprietary charity ratings. Its calculations, methodologies, source records, scoring rules, and analytical models should be available for independent examination and reproducibility.

## Specification Goals

PhilanthroMetrics shall:

- Aggregate publicly available charitable organization records.
- Analyze public financial disclosures.
- Calculate standardized mission impact metrics.
- Establish a 51% minimum impact threshold.
- Assign transparent impact grades.
- Track financial performance across multiple years.
- Identify improving, stable, and declining trends.
- Map financial relationships between organizations.
- Analyze public statements against stated organizational missions.
- Preserve source provenance for significant findings.
- Provide machine-readable results.
- Support independent auditing and verification.
- Remain modular and extensible through optional plugins.
- Minimize vendor lock-in.
- Support local and self-hosted deployments.
- Keep scoring logic transparent and reproducible.

## Core Principles

### Public Data First

The system shall prioritize legally accessible public records and publicly available information.

### Source Provenance

Every financial figure, statement, classification, relationship, and score should be traceable to an identifiable source whenever technically possible.

### Reproducibility

Users should be able to understand how a score was produced and reproduce the calculation from the underlying source data.

### Transparent Scoring

Core scoring rules shall be deterministic, documented, and independently reviewable.

### Human Review

AI analysis shall assist with classification, discovery, normalization, and pattern detection while preserving human review mechanisms for disputed or ambiguous findings.

### Historical Context

Organizations shall be evaluated across multiple reporting periods whenever sufficient historical information is available.

### Organization Separation

Each charitable organization shall have an independent profile containing its own financial records, mission information, public statements, scores, trends, relationships, and source provenance.

## Core Modules

### Organization Registry Module

The Organization Registry shall maintain standardized profiles for charitable organizations.

Each profile may contain:

- Legal organization name.
- Former names and aliases.
- Registration identifiers.
- Tax identification information where publicly available and appropriate.
- Organization type.
- Registration jurisdiction.
- Registration status.
- Stated mission.
- Program descriptions.
- Official websites.
- Verified organizational social accounts.
- Public filing references.
- Historical names.
- Related organizations.
- Source provenance.

The registry shall support organization identity resolution so that records belonging to the same organization can be connected without incorrectly merging unrelated organizations.

### Public Records Ingestion Module

The Public Records Ingestion Module shall collect and normalize publicly available records.

Supported sources may include:

- IRS Form 990 filings.
- IRS nonprofit records.
- State charity registries.
- Audited financial statements.
- Annual reports.
- Public financial disclosures.
- Official organizational reports.
- Publicly available regulatory records.

The module shall preserve the original source reference and acquisition metadata for every imported record.

### Financial Disclosure Module

The Financial Disclosure Module shall extract and normalize financial information from public filings.

The module shall identify, where available:

- Total revenue.
- Total expenses.
- Program service expenses.
- Administrative expenses.
- Fundraising expenses.
- Grants received.
- Grants distributed.
- Executive compensation.
- Asset balances.
- Liability balances.
- Investment income.
- Contributions and donations.
- Other significant revenue and expenditure categories.

The module shall retain the original reported values alongside normalized values.

### Program Impact Module

The Program Impact Module shall calculate the primary financial effectiveness metric.

The primary metric shall be:

**Program Impact Ratio = Program Service Expenses ÷ Total Revenue**

The result shall be expressed as a percentage.

The system shall preserve the underlying values used in every calculation.

Organizations reporting less than 51% of revenue as program service expenses shall receive a failing impact grade.

The 51% threshold shall be a hard minimum and shall not be offset by other positive metrics.

### Impact Grading Module

The Impact Grading Module shall assign grades according to the Program Impact Ratio.

The standard grading scale shall be:

| Program Impact Ratio | Grade | Classification |
| --- | --- | --- |
| 0% to 50.9% | F | Failing Impact |
| 51% to 60% | D | Bare Minimum Impact |
| 61% to 70% | C | Moderate Impact |
| 71% to 80% | B | Strong Impact |
| 81% to 90% | A | High Impact |
| 91% to 100% | A+ | Mission-Dominant |

A score below 51% shall always remain an F regardless of supplemental scores.

Additional metrics may provide context but shall not override the minimum impact requirement.

### Multi-Year Analysis Module

The Multi-Year Analysis Module shall evaluate organizational performance across multiple reporting periods.

The system should collect at least three years of financial history when available and may maintain substantially longer historical records.

For each reporting year, the system shall calculate the Program Impact Ratio.

The module shall identify:

- Improving performance.
- Stable performance.
- Declining performance.
- Insufficient historical data.

Trend indicators shall use:

- ▲ Improving.
- ► Stable.
- ▼ Declining.

Trend calculations shall consider the direction and magnitude of changes across multiple reporting periods rather than relying exclusively on a single year.

The system may calculate additional measures including:

- Three-year averages.
- Five-year averages.
- Year-over-year change.
- Long-term percentage change.
- Impact ratio slope.
- Impact momentum.

### Impact Graph Module

The Impact Graph Module shall provide a visual representation of charitable organizations and their relationships.

Each organization shall appear as a graph node.

Nodes may represent:

- Organizations.
- Foundations.
- Charitable entities.
- Grant recipients.
- Related entities.

Relationships may represent:

- Grants.
- Funding.
- Transfers.
- Shared organizational relationships.
- Reported affiliations.
- Other documented financial relationships.

The graph shall support visual indicators for:

- Impact grade.
- Program Impact Ratio.
- Total program expenditures.
- Multi-year trend.
- Funding relationships.

Graph data shall retain source provenance so that relationships can be independently examined.

### Public Communications Module

The Public Communications Module shall collect and organize publicly available communications associated with an organization.

Potential sources include:

- Official social media accounts.
- Official websites.
- Press releases.
- Public statements.
- Blog posts.
- Public interviews.
- Public videos and associated descriptions.
- Public organizational announcements.

The system shall prioritize verified or otherwise attributable organizational sources.

### Mission Analysis Module

The Mission Analysis Module shall establish a structured representation of an organization's stated mission.

It shall analyze:

- Mission statements.
- Organizational purpose statements.
- Program descriptions.
- Published strategic objectives.
- Official descriptions of charitable activities.

Mission concepts shall be converted into structured topics or semantic representations that can be compared with public communications.

### Public Statement Consistency Module

The Public Statement Consistency Module shall compare public organizational communications with the organization's stated mission.

The module shall identify:

- Mission-aligned topics.
- Mission-adjacent topics.
- Potentially unrelated topics.
- Significant thematic differences.
- Changes in messaging over time.

The system shall not automatically characterize a thematic difference as fraud, deception, illegality, or misconduct.

Findings shall be presented as observations supported by source material.

Each significant finding should provide:

- Original statement.
- Publication date.
- Source.
- Organization associated with the source.
- Relevant mission statement.
- Detected topic.
- Relationship to the mission.
- AI confidence where applicable.
- Human review status.

### AI Analysis Module

The AI Analysis Module shall support:

- Document classification.
- Financial field extraction.
- Mission statement analysis.
- Topic classification.
- Semantic similarity analysis.
- Entity resolution.
- Public statement categorization.
- Anomaly detection.
- Relationship discovery.
- Source prioritization.
- Duplicate detection.

AI-generated classifications shall remain distinguishable from source facts.

AI systems shall not silently alter financial records or source documents.

### Source Provenance Module

The Source Provenance Module shall maintain evidence for every significant analytical result.

Provenance records should include:

- Source organization.
- Source type.
- Source title.
- Publication or filing date.
- Retrieval date.
- Source location.
- Relevant document section.
- Extracted information.
- Processing method.
- Transformation history.
- Confidence information where applicable.

Historical source records shall remain available when licensing and data-source terms permit.

### Transparency Module

The Transparency Module shall explain how each profile, metric, grade, and observation was generated.

Users shall be able to inspect:

- Source records.
- Financial values.
- Calculations.
- Scoring thresholds.
- Historical trends.
- AI classifications.
- Supporting statements.
- Funding relationships.

The platform shall distinguish between reported facts, calculated metrics, AI-generated observations, and human-reviewed conclusions.

### Charity Profile Module

Each organization shall have a public profile containing:

- Organization identity.
- Mission statement.
- Program descriptions.
- Financial history.
- Program Impact Ratio.
- Impact Grade.
- Multi-year trend.
- Impact Graph relationships.
- Public statement analysis.
- Transparency information.
- Source records.
- Data quality indicators.
- Review and correction information.

The profile shall provide a clear explanation of why the organization received its current grade.

### Data Quality Module

The Data Quality Module shall evaluate the completeness and reliability of available records.

It shall identify:

- Missing filings.
- Missing financial categories.
- Incomplete historical records.
- Conflicting records.
- Parsing errors.
- Source inconsistencies.
- Unverified organizational identities.
- Insufficient data for specific calculations.

Missing or incomplete information shall not be silently interpreted as zero.

### Correction and Review Module

Organizations and members of the public shall have a mechanism for identifying incorrect information.

Correction submissions may include:

- Incorrect organization identity.
- Incorrect source association.
- Incorrect financial extraction.
- Outdated mission statements.
- Incorrect social account attribution.
- Incorrect relationship mapping.
- Other factual corrections.

Corrections shall be documented and reviewed before modifying authoritative records.

### Audit Module

The Audit Module shall preserve a reproducible record of scoring decisions and analytical transformations.

Audit records should identify:

- Source data used.
- Calculation inputs.
- Calculation results.
- Model versions.
- Scoring methodology version.
- Processing dates.
- Human review actions.
- Corrections.
- Revisions.

Changes to scoring methodology shall produce versioned results rather than silently rewriting historical scores.

### Open Data Module

The Open Data Module shall provide machine-readable representations of organization profiles and analytical results.

The standard data format shall support:

- Organization identity.
- Financial records.
- Program Impact Ratios.
- Impact Grades.
- Historical trends.
- Source provenance.
- Messaging observations.
- Funding relationships.
- Methodology versions.

The `.charityscore.json` format shall provide a portable representation of charity analysis data.

### Search Module

The Search Module shall allow users to search organizations by:

- Name.
- Registration identifier.
- Location.
- Impact Grade.
- Program Impact Ratio.
- Trend.
- Mission topic.
- Organization type.
- Funding relationship.
- Transparency indicators.

Search results shall distinguish exact matches from AI-assisted or inferred matches.

### Comparison Module

The Comparison Module shall allow users to compare organizations using standardized metrics.

Comparisons may include:

- Program Impact Ratio.
- Impact Grade.
- Revenue.
- Program expenses.
- Administrative expenses.
- Fundraising expenses.
- Multi-year trends.
- Transparency indicators.
- Mission categories.
- Funding relationships.

The system shall clearly identify differences in reporting periods when comparing organizations.

### Notification Module

The Notification Module shall optionally notify users when tracked organizations experience significant changes.

Notifications may include:

- New financial filings.
- Grade changes.
- Trend changes.
- Significant changes in program spending.
- New public statements.
- Newly identified funding relationships.
- Corrections.
- Methodology changes.

## Optional Plugin Modules

### Government Registry Plugin

Provides connectors for government charity registries and nonprofit databases.

### IRS Data Plugin

Provides specialized ingestion and normalization of IRS nonprofit records and Form 990 data.

### State Registry Plugin

Adds state-specific charity registration and disclosure sources.

### Social Media Plugin

Connects to supported public social media APIs and public organizational accounts where access is legally and technically available.

### Web Archive Plugin

Provides historical snapshots of public organizational websites and mission statements where permitted.

### Press Monitoring Plugin

Collects public press releases and other attributable organizational communications.

### OCR Plugin

Provides specialized OCR processing for scanned financial documents.

### Advanced NLP Plugin

Adds specialized language models for financial document classification, mission analysis, and semantic comparison.

### Graph Analytics Plugin

Adds advanced network analysis for funding relationships, organizational affiliations, and grant networks.

### Geospatial Plugin

Adds geographic analysis of organizations, programs, funding, and service areas.

### Data Export Plugin

Provides additional export formats for researchers, journalists, analysts, and public data projects.

### Research API Plugin

Provides expanded programmatic access to public datasets and analytical results.

### Visualization Plugin

Provides additional graph, timeline, financial flow, and comparative visualization capabilities.

### Alerting Plugin

Provides configurable monitoring and notification capabilities for organizations and networks.

### Human Review Plugin

Provides advanced workflows for expert review, dispute resolution, annotation, and model evaluation.

## Scoring Framework

The Program Impact Ratio shall remain the foundational metric.

Supplemental metrics may provide additional context, but they shall not override the 51% minimum threshold.

Potential supplemental metrics include:

- Fundraising efficiency.
- Administrative expense ratio.
- Multi-year consistency.
- Financial transparency.
- Filing completeness.
- Revenue stability.
- Program spending growth.
- Executive compensation context.
- Funding concentration.
- Grant pass-through activity.

Supplemental metrics shall be displayed separately from the primary impact grade unless a future specification explicitly establishes a revised grading methodology.

## Impact Trend Framework

Trend analysis shall evaluate both current performance and historical direction.

A charity may therefore display:

**F ▲**

when it remains below the minimum threshold but its Program Impact Ratio is improving.

A charity may display:

**A ▼**

when it currently meets a high impact threshold but its historical efficiency is declining.

The grade and trend shall remain separate indicators so that users can distinguish current performance from direction of change.

## Mission Consistency Framework

Mission consistency analysis shall never replace financial analysis.

The system shall distinguish between:

- Financial impact.
- Mission alignment.
- Public messaging.
- Organizational activities.
- AI observations.

A public statement that differs from a mission statement shall be surfaced as a documented observation rather than automatically classified as misconduct.

## Data Governance

PhilanthroMetrics shall maintain clear distinctions between:

- Original source data.
- Normalized data.
- Calculated data.
- AI-generated analysis.
- Human-reviewed analysis.

Source records shall not be overwritten when new interpretations are produced.

Corrections shall preserve historical audit information.

## Privacy

PhilanthroMetrics shall prioritize organizational and public information.

The system shall not intentionally collect private communications or private social media content.

Public information involving individuals shall be handled according to applicable privacy, data protection, and source-use requirements.

## Responsible AI

AI models shall be used as analytical tools rather than unquestionable authorities.

The system shall:

- Preserve source evidence.
- Record model versions where appropriate.
- Distinguish AI observations from source facts.
- Provide confidence information where practical.
- Permit human review.
- Avoid unsupported accusations.
- Allow corrections.
- Preserve historical analytical results.
- Document significant model changes.

## Transparency Requirements

Every published impact grade should be accompanied by enough information to understand:

- The reporting period.
- Total revenue used.
- Program service expenses used.
- Calculated Program Impact Ratio.
- Applicable grading threshold.
- Current grade.
- Historical trend when sufficient data exists.
- Relevant source records.

Every public statement observation should identify its source and publication date whenever available.

## Extensibility

Core functionality shall remain independent of optional data providers, AI models, storage systems, and interface implementations.

Plugins should communicate with core services through documented interfaces.

The system should allow organizations and developers to replace individual components without requiring a complete platform rewrite.

## Local-First and Self-Hosted Operation

PhilanthroMetrics should support local and self-hosted deployments.

Users should be able to:

- Import public datasets.
- Run financial calculations locally.
- Process documents locally.
- Maintain local organization profiles.
- Run supported AI models locally.
- Export analysis.
- Reproduce scores without depending on a proprietary hosted service.

## Methodology Versioning

Every scoring result shall identify the methodology version used to generate it.

Changes to:

- Thresholds.
- Formulas.
- Classification rules.
- AI models.
- Data normalization.
- Trend calculations.

shall result in a new methodology version.

Historical results shall remain attributable to the methodology under which they were produced.

## Accessibility

The public interface should provide:

- Accessible navigation.
- Screen-reader compatible data.
- Text alternatives for graph information.
- Keyboard-accessible controls.
- Clear grade descriptions.
- Plain-language explanations of financial metrics.
- Downloadable data for users who cannot access interactive visualizations.

## Security

The platform shall protect:

- User accounts where applicable.
- Administrative interfaces.
- Data ingestion credentials.
- API credentials.
- Private configuration.
- Internal system metadata.

Public source data shall not be treated as trusted input without validation.

External documents shall be processed using appropriate security controls.

## Performance

The system should support large-scale processing of charitable organizations while preserving source provenance and reproducibility.

Processing should support:

- Incremental ingestion.
- Deduplication.
- Caching.
- Parallel document processing.
- Historical updates.
- Selective reprocessing.
- Versioned analytical outputs.

## Testing and Validation

Core calculations shall have automated tests covering:

- Program Impact Ratio calculations.
- Grade boundaries.
- 51% threshold enforcement.
- Multi-year trend calculations.
- Missing data handling.
- Source association.
- Organization identity resolution.
- Graph relationship integrity.
- Data serialization.

AI components should be evaluated against documented test datasets before deployment.

## Documentation

Documentation shall describe:

- Data sources.
- Data processing.
- Financial calculations.
- Scoring methodology.
- Trend methodology.
- AI models.
- Mission analysis.
- Graph construction.
- Plugin interfaces.
- Data formats.
- Privacy practices.
- Governance.
- Versioning.

## Governance

Changes to core scoring methodology shall be documented and publicly reviewable.

Changes that materially affect organization grades should include:

- The reason for the change.
- The affected methodology.
- The implementation date.
- The methodology version.
- Expected effects.
- Migration or recalculation information where applicable.

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
  - [https://roxanneardary.com/philanthrometrics/](https://roxanneardary.com/philanthrometrics/)

---

## License & Notice Requirements

PhilanthroMetrics is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- PhilanthroMetrics specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.  
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
