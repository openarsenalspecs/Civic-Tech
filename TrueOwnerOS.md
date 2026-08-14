# TrueOwnerOS Specification
**Bringing Ownership Out of the Shadows.**  

HTML Mirror:  [https://roxanneardary.com/trueowneros-specification/](https://roxanneardary.com/trueowneros-specification/)  
---

## Purpose

TrueOwnerOS shall provide an open-source intelligence system for identifying, classifying, mapping, and analyzing mission-critical corporate properties and the relationships between property ownership, corporate control, property operation, leasing, infrastructure dependency, and public service dependency.

The system shall identify situations in which an organization operates or depends upon a mission-critical property that it does not own.

TrueOwnerOS shall transform public records, corporate disclosures, government records, geographic information, infrastructure data, financial information, and other legally usable sources into a verifiable ownership and dependency intelligence graph.

The system shall prioritize evidence, provenance, transparency, reproducibility, and human verification.

---

## Core Objectives

TrueOwnerOS shall:

- Identify mission-critical properties
- Identify property owners
- Identify ultimate corporate owners where verifiable
- Identify property operators and occupants
- Detect operator-owner mismatches
- Map corporate ownership structures
- Map landlord and tenant relationships
- Analyze lease structures
- Identify infrastructure dependencies
- Identify corporate and community concentration risks
- Analyze property and portfolio resilience
- Preserve evidence and provenance
- Provide historical ownership records
- Support AI-assisted research and analysis
- Provide machine-readable data and APIs
- Support community verification
- Maintain an auditable public knowledge base

---

# Core Modules

## Property Intelligence Module

The Property Intelligence Module shall maintain canonical records for mission-critical properties.

The module shall support:

- Property identification
- Address normalization
- Geographic coordinates
- Parcel identification
- Property classification
- Facility naming
- Property ownership records
- Property operator records
- Property occupancy records
- Property history
- Property status
- Property criticality classification
- Property service-area identification
- Property evidence records
- Property confidence scoring

The module shall support property categories including:

- Data centers
- Fulfillment centers
- Distribution centers
- Logistics facilities
- Warehouses
- Cold storage facilities
- Hospitals
- Clinics
- Medical facilities
- Pharmaceutical facilities
- Telecom facilities
- Fiber infrastructure
- Utility facilities
- Power facilities
- Manufacturing facilities
- Semiconductor facilities
- Food processing facilities
- Government facilities
- Emergency service facilities
- Transportation facilities
- Public infrastructure
- Other mission-critical facilities

---

## Mission Criticality Module

The Mission Criticality Module shall determine the operational importance of a property.

The module shall evaluate:

- Service dependency
- Population dependency
- Replacement difficulty
- Relocation difficulty
- Geographic uniqueness
- Infrastructure interdependency
- Supply chain importance
- Availability of alternative facilities
- Service-area size
- Operational continuity requirements

The module shall assign a mission-criticality classification and confidence level.

The classification methodology shall be transparent and configurable.

---

## Ownership Intelligence Module

The Ownership Intelligence Module shall identify and resolve property ownership.

The module shall support:

- Recorded owner identification
- Corporate owner identification
- LLC identification
- Subsidiary identification
- Parent-company identification
- Ultimate-owner identification
- Ownership-chain mapping
- Beneficial ownership relationships where publicly verifiable
- Historical ownership
- Acquisition tracking
- Disposition tracking
- Ownership confidence scoring

The module shall distinguish between:

- Recorded owner
- Legal owner
- Corporate parent
- Ultimate parent
- Beneficial owner where verifiable
- Investor
- Asset manager
- Property manager
- Operator
- Occupant
- Tenant
- Servicer

---

## Operator and Servicer Module

The Operator and Servicer Module shall identify the organization operating, managing, servicing, or occupying a mission-critical property.

The module shall support:

- Operator identification
- Servicer identification
- Occupant identification
- Tenant identification
- Property manager identification
- Service relationship identification
- Operator history
- Operator confidence scoring

The module shall explicitly distinguish operational control from ownership.

---

## Operator Owner Mismatch Module

The Operator Owner Mismatch Module shall identify properties where the organization operating or relying upon a property differs from the property owner.

The module shall identify relationships such as:

- Operator owned by third-party landlord
- Corporate tenant leasing mission-critical property
- Government agency leasing privately owned property
- Hospital operating from REIT-owned property
- Utility operating from third-party property
- Corporation operating from private-equity-owned property
- Critical service operating from infrastructure-fund-owned property

Each mismatch shall include:

- Property
- Owner
- Operator
- Relationship type
- Evidence
- Confidence
- Effective date where known
- Verification status

---

## Corporate Entity Resolution Module

The Corporate Entity Resolution Module shall normalize and connect corporate identities.

The module shall support:

- Corporate name normalization
- Legal entity matching
- DBA identification
- Subsidiary matching
- Parent-company matching
- Ultimate-owner matching
- Corporate alias detection
- Historical corporate names
- Corporate registration identifiers
- SEC identifiers where applicable
- Cross-source entity reconciliation

The module shall construct corporate family relationships including:

- Parent
- Subsidiary
- Affiliate
- Controlled entity
- Holding company
- Special purpose entity
- Investment entity
- Property holding entity

---

## Lease Intelligence Module

The Lease Intelligence Module shall identify and analyze property lease structures.

The module shall support:

- Lease identification
- Lease type classification
- NNN lease identification
- NN lease identification
- N lease identification
- Gross lease identification
- Modified gross lease identification
- Sale-leaseback identification
- Lease commencement
- Lease expiration
- Renewal options
- Rent escalations
- CPI-linked escalations
- Fixed escalations
- Lease obligations
- Tenant rent burden
- Lease concentration
- Lease rollover exposure
- Lease-adjusted leverage

The module shall preserve the source of each extracted lease term.

---

## Ownership Shadow Detection Module

The Ownership Shadow Detection Module shall identify ownership structures requiring additional investigation.

The module shall detect:

- Layered LLC structures
- Shell entities
- Common registered addresses
- Common management relationships
- Related-party relationships
- Related-party leases
- Rapid ownership transfers
- Repeated sale-leasebacks
- Unusual ownership chains
- Conflicting ownership records
- Incomplete ownership disclosures
- Private equity control patterns
- Infrastructure fund ownership patterns

The module shall distinguish between verified facts and AI-generated investigative indicators.

---

## Portfolio Intelligence Module

The Portfolio Intelligence Module shall analyze collections of properties controlled, owned, leased, or operated by an organization.

The module shall support:

- Corporate property portfolios
- REIT portfolios
- Private equity portfolios
- Infrastructure fund portfolios
- Institutional portfolios
- Tenant portfolios
- Landlord portfolios
- Operator portfolios
- Geographic portfolios
- Mission-critical portfolios

The module shall calculate:

- Property concentration
- Geographic concentration
- Tenant concentration
- Landlord concentration
- Critical-property exposure
- Ownership concentration
- Operator concentration

---

## Concentration Risk Module

The Concentration Risk Module shall identify excessive dependency on individual organizations, properties, landlords, operators, or geographic areas.

The module shall detect:

- Single-tenant exposure
- Single-landlord exposure
- Single-property dependency
- Single-operator dependency
- Corporate parent concentration
- REIT tenant concentration
- Geographic concentration
- Municipal dependency
- Subsidiary clustering
- False diversification
- Common-parent exposure

---

## Corporate Dependency Module

The Corporate Dependency Module shall identify properties and infrastructure upon which organizations depend.

The module shall evaluate:

- Property dependency
- Landlord dependency
- Operator dependency
- Infrastructure dependency
- Geographic dependency
- Supply chain dependency
- Service dependency
- Lease dependency

The module shall calculate configurable scores including:

- Property Control Index
- Operational Criticality Score
- Population Impact Score
- Relocation Difficulty Score
- Corporate Failure Impact Score
- Community Dependency Score
- Landlord Power Score
- Failure Impact Score

---

## Infrastructure Dependency Module

The Infrastructure Dependency Module shall map relationships between mission-critical properties and surrounding infrastructure.

The module shall identify dependencies involving:

- Electricity
- Natural gas
- Water
- Telecommunications
- Fiber
- Transportation
- Logistics
- Healthcare
- Emergency services
- Distribution networks
- Manufacturing networks

The module shall identify infrastructure clusters and potential geographic chokepoints.

---

## Infrastructure Fragility Module

The Infrastructure Fragility Module shall identify locations where multiple mission-critical systems overlap or depend upon one another.

The module shall support:

- Co-location analysis
- Dependency graphing
- Geographic proximity analysis
- Multi-system dependency detection
- Critical cluster identification
- Chokepoint identification
- Regional fragility scoring
- Service disruption modeling
- Cascading dependency analysis

---

## Supply Chain Intelligence Module

The Supply Chain Intelligence Module shall map corporate and physical dependencies across supply chains.

The module shall identify:

- Suppliers
- Manufacturers
- Distributors
- Warehouses
- Fulfillment centers
- Retailers
- Transportation nodes
- Critical logistics facilities
- Non-owned infrastructure
- Supply chain chokepoints

The module shall connect corporate relationships with physical property relationships.

---

## Private Equity Intelligence Module

The Private Equity Intelligence Module shall identify relationships between private equity ownership and mission-critical property portfolios.

The module shall support:

- PE portfolio company identification
- PE property ownership identification
- Roll-up mapping
- Sale-leaseback analysis
- Debt-loading indicators
- Asset disposition tracking
- Dividend extraction indicators
- Lease burden analysis
- Rent escalation analysis
- Property monetization tracking
- Corporate dependency analysis

The module shall present such findings as indicators requiring appropriate evidence and shall not automatically characterize lawful transactions as misconduct.

---

## Government Dependency Module

The Government Dependency Module shall identify public services operating from privately owned properties.

The module shall support:

- USPS facilities
- DMV facilities
- Social service facilities
- Emergency facilities
- Public health facilities
- Utility operations
- Municipal administration
- Courthouses
- Public schools
- Charter schools
- Government contractors
- Other public-service facilities

The module shall identify:

- Government operator
- Private owner
- Lease relationship
- Property criticality
- Public dependency
- Lease expiration where available

---

## Tenant Financial Intelligence Module

The Tenant Financial Intelligence Module shall analyze the financial resilience of organizations operating from mission-critical properties.

The module shall support:

- Credit ratings
- Bond yields
- Financial statements
- Cash flow metrics
- Debt metrics
- Lease-adjusted leverage
- Rent burden
- Financial distress indicators
- Default probability modeling
- Renewal risk modeling
- Tenant failure scenarios

Predictions shall be labeled as models or estimates rather than verified facts.

---

## Corporate Failure Simulation Module

The Corporate Failure Simulation Module shall model potential consequences of corporate, property, or landlord failures.

The module shall simulate:

- Tenant bankruptcy
- Lease default
- Landlord bankruptcy
- REIT liquidation
- Property disposition
- Rent increases
- Lease expiration
- Facility closure
- Natural disasters
- Infrastructure failures
- Corporate restructuring

The module shall produce:

- Potential property closures
- Service disruption estimates
- Population impact estimates
- Supply chain disruption estimates
- Dependency propagation
- Alternative-property analysis

---

## Resilience Analysis Module

The Resilience Analysis Module shall evaluate the ability of organizations and communities to maintain critical services when property or ownership conditions change.

The module shall support:

- Property resilience scoring
- Corporate resilience scoring
- Portfolio resilience scoring
- Municipal resilience scoring
- Regional resilience scoring
- Alternative facility identification
- Replacement difficulty analysis
- Relocation analysis
- Service continuity analysis
- Landlord dependency analysis

---

## Failure Event Registry Module

The Failure Event Registry Module shall maintain historical records of mission-critical property failures and service disruptions.

The module shall support:

- Foreclosures
- Hospital closures
- Data center outages
- Distribution center closures
- Warehouse fires
- Utility failures
- Manufacturing shutdowns
- Facility relocations
- Property abandonment
- Service-area disruptions
- Infrastructure failures

Each event shall include evidence, dates, affected properties, affected organizations, and verification status where available.

---

## AI Filing Auditor Module

The AI Filing Auditor Module shall analyze public corporate and financial disclosures.

The module shall support:

- SEC filings
- Annual reports
- Quarterly reports
- Current reports
- REIT disclosures
- Property disclosures
- Acquisition disclosures
- Disposition disclosures
- Lease disclosures
- Related-party transaction disclosures

The module shall identify:

- Ownership inconsistencies
- Lease inconsistencies
- Conflicting disclosures
- Historical disclosure changes
- Related-party relationships
- Potentially incomplete disclosures

AI findings shall remain distinguishable from verified source information.

---

## Public Records Module

The Public Records Module shall ingest and normalize legally accessible public records.

Supported sources may include:

- County assessor records
- Property tax records
- Deeds
- Corporate registrations
- Public GIS systems
- Government registries
- Bankruptcy filings
- Infrastructure registries
- Public contracts
- Government leases
- Corporate disclosures

The module shall preserve source metadata and provenance.

---

## FOIA and Public Records Request Module

The FOIA and Public Records Request Module shall support the collection and organization of government records.

The module shall support:

- FOIA requests
- State public records requests
- OPRA requests
- Request tracking
- Document collection
- Lease document collection
- Government contract collection
- Public property records
- Facility records
- Request status
- Response documentation

---

## Evidence and Provenance Module

The Evidence and Provenance Module shall provide traceability for every material database claim.

The module shall support:

- Source citations
- Evidence documents
- Source reliability
- Evidence confidence
- Data provenance
- Human verification
- AI inference labeling
- Conflicting-source detection
- Historical evidence
- Change history
- Audit trails
- Correction history
- Verification status

The system shall distinguish:

- Verified information
- Source-derived information
- AI-extracted information
- AI-inferred information
- Community-submitted information
- Unverified information

---

## Data Quality Module

The Data Quality Module shall maintain database integrity.

The module shall support:

- Duplicate detection
- Record validation
- Missing-data detection
- Conflicting-record detection
- Confidence scoring
- Source freshness
- Data expiration alerts
- Versioned datasets
- Historical snapshots
- Human review queues
- Correction workflows

---

## AI Entity Resolution Module

The AI Entity Resolution Module shall automatically identify relationships between records referring to the same entity.

The module shall support:

- Corporate name matching
- Address matching
- LLC matching
- Subsidiary matching
- Parent matching
- Property matching
- Operator matching
- Alias detection
- Historical name matching
- Duplicate detection
- Entity confidence scoring

---

## AI Property Discovery Module

The AI Property Discovery Module shall identify potential mission-critical properties from structured and unstructured sources.

The module shall support:

- Address extraction
- Facility-name extraction
- Property-type classification
- Operator identification
- Owner identification
- Corporate disclosure analysis
- Public-record discovery
- GIS discovery
- Infrastructure dataset analysis
- Evidence collection
- Confidence scoring

---

## Search and Discovery Module

The Search and Discovery Module shall provide structured access to the database.

The module shall support searches by:

- Property
- Address
- Parcel
- Corporation
- Owner
- Operator
- Tenant
- Landlord
- REIT
- Private equity group
- Location
- Property type
- Mission criticality
- Ownership mismatch
- Lease structure
- Risk score

The module shall support:

- Full-text search
- Advanced filters
- Geographic search
- Map search
- Historical search
- Evidence search

---

## Mapping and Visualization Module

The Mapping and Visualization Module shall present relationships geographically and structurally.

The module shall support:

- Property maps
- Ownership maps
- Corporate relationship graphs
- Property-owner graphs
- Operator-property graphs
- Landlord-tenant graphs
- Supply chain maps
- Infrastructure dependency maps
- Risk heatmaps
- Concentration heatmaps
- Historical ownership timelines
- Corporate portfolio visualizations
- Municipal dependency maps
- Regional infrastructure maps

---

## Public Accountability Module

The Public Accountability Module shall provide public-facing transparency tools.

The module shall support:

- Who Owns This Property?
- Who Owns This Building?
- Who Owns Your Town?
- Corporate property profiles
- REIT exposure dashboards
- Tenant dependency dashboards
- Landlord dependency dashboards
- Infrastructure vulnerability maps
- Community dependency maps
- Public ownership reports
- Downloadable public datasets

---

## Monitoring and Alert Module

The Monitoring and Alert Module shall detect material changes.

The module shall support alerts for:

- Ownership changes
- Property sales
- Lease expirations
- Corporate ownership changes
- REIT portfolio changes
- Tenant distress
- Bankruptcy
- Facility closures
- Infrastructure failures
- Disclosure changes
- Risk-score changes
- Newly identified ownership mismatches
- Newly identified mission-critical properties

---

## API Module

TrueOwnerOS shall provide programmatic access to system data and intelligence.

The API module shall support:

- REST API
- GraphQL API
- Property queries
- Corporate entity queries
- Ownership queries
- Operator queries
- Lease queries
- Risk queries
- Evidence queries
- Search queries
- Mapping queries
- Bulk data access

APIs shall return source and confidence metadata where applicable.

---

## Developer Module

The Developer Module shall provide tools for integrating with TrueOwnerOS.

The module shall support:

- Command Line Interface
- Machine-readable exports
- Bulk datasets
- API clients
- Webhooks
- Custom data connectors
- Model integration interfaces
- Plugin interfaces
- Data import tools
- Data export tools

---

## Data Interoperability Module

The Data Interoperability Module shall support standardized data exchange.

The module shall support:

- CSV
- JSON
- GeoJSON
- GIS data
- Stable property identifiers
- Corporate entity identifiers
- External registry identifiers
- Source identifiers
- Dataset versioning
- Cross-dataset reconciliation

---

## Governance and Security Module

The Governance and Security Module shall protect system integrity while maintaining open-source transparency.

The module shall support:

- Role-based access controls
- Administrative controls
- Audit logging
- Dataset integrity monitoring
- API access controls
- Provenance controls
- Data correction workflows
- Contributor verification
- Moderation workflows
- Abuse reporting
- Security reporting
- Privacy safeguards
- Unauthorized modification protection

TrueOwnerOS shall focus on corporate, institutional, governmental, and publicly documented property information.

The system shall avoid unnecessary publication of sensitive personal information.

---

## Community Verification Module

The Community Verification Module shall allow contributors to improve database accuracy.

The module shall support:

- Ownership corrections
- Operator corrections
- Property classification corrections
- Source submissions
- Evidence submissions
- Record verification
- Conflict reporting
- Community review
- Contributor attribution
- Correction history

Community submissions shall remain distinguishable from independently verified records until verification requirements are satisfied.

---

## International Ownership Module

The International Ownership Module shall extend ownership intelligence beyond a single jurisdiction.

The module shall support:

- Cross-border ownership
- Foreign parent companies
- International subsidiaries
- Offshore holding companies
- Sovereign wealth fund ownership
- International REITs
- Cross-border investment structures
- Country-level ownership concentration

Jurisdiction-specific data models shall be supported where local property and corporate records differ.

---

# Optional Plugin Modules

Optional plugins shall extend TrueOwnerOS without requiring every deployment to enable every capability.

## Financial Markets Plugin

The Financial Markets Plugin may provide:

- REIT market data
- Equity data
- Debt data
- Bond yields
- Credit spreads
- Market capitalization
- Dividend information
- Financial exposure analysis
- Property portfolio market analysis

---

## Advanced Geospatial Plugin

The Advanced Geospatial Plugin may provide:

- Satellite imagery analysis
- Parcel geometry
- Building footprint analysis
- Spatial clustering
- Proximity analysis
- Travel-time analysis
- Service-area modeling
- Geographic risk modeling

---

## Satellite and Remote Sensing Plugin

The Satellite and Remote Sensing Plugin may provide:

- Facility detection
- Construction monitoring
- Property change detection
- Industrial activity indicators
- Infrastructure expansion analysis
- Historical imagery comparison

---

## Corporate Registry Plugin

The Corporate Registry Plugin may connect jurisdiction-specific corporate registration databases.

It may provide:

- Corporate registration records
- Registered-agent information
- Entity status
- Filing history
- Corporate officers where publicly available
- Parent and subsidiary relationships

---

## Infrastructure Registry Plugin

The Infrastructure Registry Plugin may integrate specialized infrastructure datasets.

It may support:

- Telecommunications
- Electricity
- Water
- Natural gas
- Transportation
- Emergency services
- Utility infrastructure
- Critical facility registries

---

## News and Event Monitoring Plugin

The News and Event Monitoring Plugin may detect:

- Facility closures
- Property acquisitions
- Corporate restructurings
- Bankruptcy events
- Lease announcements
- Infrastructure failures
- Corporate relocations
- Major ownership changes

All automatically detected events shall require appropriate source attribution.

---

## Document Intelligence Plugin

The Document Intelligence Plugin may provide:

- OCR
- PDF extraction
- Table extraction
- Lease extraction
- Corporate filing extraction
- Document classification
- Document comparison
- Historical document comparison
- Automated evidence linking

---

## Advanced AI Research Plugin

The Advanced AI Research Plugin may provide:

- Multi-document reasoning
- Entity relationship discovery
- Automated investigative queries
- Knowledge graph expansion
- Hypothesis generation
- Evidence clustering
- Contradiction detection
- Research summaries

AI-generated conclusions shall remain clearly labeled as analysis rather than established facts.

---

## Predictive Risk Plugin

The Predictive Risk Plugin may provide:

- Property failure prediction
- Tenant distress prediction
- Lease renewal prediction
- Landlord distress prediction
- Infrastructure disruption prediction
- Corporate dependency forecasting
- Concentration risk forecasting

Predictive outputs shall include model methodology, confidence, assumptions, and limitations.

---

## Scenario Planning Plugin

The Scenario Planning Plugin may provide configurable simulations for:

- Corporate bankruptcy
- REIT liquidation
- Property sale
- Lease expiration
- Rent increases
- Infrastructure failure
- Natural disasters
- Supply chain disruption
- Service-area loss
- Multi-property failure

---

## Public Portal Plugin

The Public Portal Plugin may provide:

- Public property search
- Public ownership profiles
- Community dashboards
- Municipal dashboards
- Public maps
- Public reports
- Downloadable datasets
- Ownership transparency pages

---

## Researcher Plugin

The Researcher Plugin may provide:

- Saved investigations
- Research workspaces
- Evidence collections
- Custom queries
- Relationship graphs
- Timeline analysis
- Dataset comparison
- Citation management
- Exportable research reports

---

## Data Contribution Plugin

The Data Contribution Plugin may provide:

- Community dataset submission
- Bulk property submission
- Ownership corrections
- Evidence submission
- Source verification
- Data review queues
- Contributor attribution

---

## Notification Plugin

The Notification Plugin may deliver alerts through supported channels.

It may support:

- Email
- Web notifications
- Webhooks
- API callbacks
- Dashboard alerts

---

# Data Source Requirements

TrueOwnerOS shall prioritize legally accessible and appropriately licensed sources.

Potential sources include:

- County property records
- Property tax records
- Deeds
- Corporate registrations
- SEC filings
- Government records
- Public GIS datasets
- FOIA records
- OPRA records
- Infrastructure registries
- Bankruptcy filings
- Corporate disclosures
- Public contracts
- Publicly accessible lease disclosures
- Open geographic datasets

Each source shall be associated with provenance metadata.

---

# Data Provenance Requirements

Every material ownership, operator, lease, property, or risk claim should be traceable to one or more sources.

The system shall preserve:

- Source identity
- Source type
- Source location
- Retrieval date
- Publication date where available
- Relevant document
- Relevant record
- Extraction method
- Verification status
- Confidence level
- Historical version

---

# AI Requirements

AI functionality shall operate as an analytical layer over evidence rather than as an undisclosed source of truth.

AI systems shall:

- Preserve source references
- Distinguish extraction from inference
- Assign confidence
- Identify uncertainty
- Preserve competing interpretations
- Avoid presenting predictions as facts
- Support human verification
- Maintain reproducible processing where practical
- Preserve model and processing metadata where appropriate

---

# Risk Scoring Requirements

Risk scores shall be:

- Transparent
- Configurable
- Reproducible
- Evidence-based
- Versioned
- Explainable

Each score shall identify the factors contributing to the result.

Risk scores shall not be presented as definitive predictions when the underlying data is uncertain.

---

# Use Cases

## Investors

TrueOwnerOS may support:

- REIT tenant risk analysis
- Corporate lease exposure analysis
- Property ownership research
- Portfolio concentration analysis
- Private equity property analysis
- Sale-leaseback analysis
- Tenant dependency analysis

## Journalists

TrueOwnerOS may support:

- Corporate ownership investigations
- Property ownership investigations
- Infrastructure dependency investigations
- Public-service landlord investigations
- Corporate structure research
- Historical ownership research

## Governments

TrueOwnerOS may support:

- Emergency planning
- Infrastructure dependency analysis
- Municipal risk analysis
- Public-service dependency analysis
- Critical facility continuity planning
- Property ownership research

## Communities

TrueOwnerOS may support:

- Local ownership transparency
- Mission-critical property research
- Public-service dependency awareness
- Community infrastructure mapping
- Corporate property research  

---

# Contributing

Contributions may include:

- Data ingestion
- Entity resolution
- Property classification
- Ownership research
- AI extraction
- Risk scoring
- Graph analytics
- Geospatial analysis
- API development
- Plugin development
- Dashboard development
- Data verification
- Documentation
- Testing

All contributions shall comply with the project's licensing, attribution, provenance, privacy, and data integrity requirements.

See `CONTRIBUTING.md` for contribution guidelines.

---

# Design Principles

TrueOwnerOS shall follow these principles:

- Ownership transparency
- Evidence before inference
- Open-source development
- Publicly verifiable data
- Human-in-the-loop verification
- Clear distinction between fact and analysis
- Reproducible processing
- Data provenance
- Interoperability
- Vendor neutrality
- Modular architecture
- Extensible plugins
- Privacy-conscious public research
- Long-term preservation of historical records

---

# Vision

TrueOwnerOS is intended to become a permanent open-source intelligence layer for understanding who owns, operates, controls, leases, finances, and depends upon mission-critical real estate.

The system shall make corporate property ownership visible, connect physical assets to corporate structures, identify dependencies that are otherwise difficult to see, and preserve an evidence-based public record of changes over time.

**Ownership should never be hidden.**

**TrueOwnerOS brings ownership out of the shadows.**

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
  - [https://roxanneardary.com/trueowneros/](https://roxanneardary.com/trueowneros/)

---

## License & Notice Requirements

TrueOwnerOS is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- TrueOwnerOS specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.

---
HTML Mirror:  [https://roxanneardary.com/trueowneros-specification/](https://roxanneardary.com/trueowneros-specification/)  
