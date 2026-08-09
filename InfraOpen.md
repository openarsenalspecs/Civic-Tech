# InfraOpen

**Power, Internet, Insight — All in One Place**

## Overview

InfraOpen is an open-source utility transparency and infrastructure intelligence platform designed to provide comprehensive, state-by-state information about electricity and internet utilities across the United States.

The platform combines utility provider profiles, corporate ownership, governance, billing laws, regulatory requirements, compliance monitoring, rates, infrastructure, financial information, sustainability metrics, consumer complaints, and historical records into a unified system.

InfraOpen is designed as a modular platform. Core modules provide the foundational capabilities required by the system, while optional plugin modules allow organizations and contributors to extend the platform with additional datasets, analytical capabilities, utility categories, integrations, and specialized tools without modifying the core architecture.

## Project Goals

InfraOpen is designed to:

- Improve transparency surrounding essential infrastructure.
- Provide state-by-state utility information in one location.
- Identify corporate ownership and control structures.
- Track boards of directors and corporate officers.
- Connect utility companies with applicable laws and regulations.
- Monitor billing practices and regulatory compliance.
- Track rates, fees, tariffs, and billing procedures.
- Document regulatory violations, penalties, and enforcement actions.
- Provide historical records of changes to utilities and their governing organizations.
- Map utility infrastructure and service territories.
- Provide accessible data for consumers, researchers, journalists, regulators, and developers.
- Establish an extensible foundation for additional utility categories and infrastructure systems.

## Modular Architecture

InfraOpen uses a modular architecture consisting of three primary layers:

### Core Platform

The core platform provides the foundational services required by all other modules, including:

- Database management
- Entity identification and normalization
- Data provenance
- Source management
- Historical version tracking
- Geographic data management
- Authentication and authorization
- API infrastructure
- Search and indexing
- Change detection
- Data validation
- Audit logging
- Notification infrastructure
- Configuration management
- Plugin management

### Core Modules

Core modules contain the primary features of InfraOpen. These modules establish the standard data structures and functionality used throughout the platform.

Core modules should remain focused on broadly applicable infrastructure capabilities rather than specialized integrations.

### Optional Plugin Modules

Optional plugins extend InfraOpen without making specialized functionality a dependency of the core platform.

Plugins may provide:

- Additional utility categories
- External data integrations
- Specialized compliance rules
- Advanced analytics
- Additional geographic datasets
- Specialized consumer tools
- Regulatory monitoring
- Corporate ownership intelligence
- Alternative visualization systems
- Third-party APIs
- Research tools
- Experimental functionality

Plugins should use documented interfaces and APIs provided by the core platform.

## Core Modules

### Utility Provider Module

Maintains profiles for electricity and internet utility providers.

Features include:

- Provider name
- Legal entity name
- Utility type
- Service states
- Service territories
- Parent company
- Subsidiaries
- Corporate relationships
- Regulatory jurisdiction
- Licensing information
- Provider status
- Historical records

### Corporate Ownership Module

Tracks the corporate structures behind utility providers.

Features include:

- Parent companies
- Subsidiaries
- Ownership relationships
- Ultimate parent organization
- Primary country of ownership
- Major shareholders
- Ownership changes
- Corporate mergers
- Acquisitions
- Divestitures
- Historical ownership records

### Governance Module

Maintains profiles for corporate leadership and governance.

Features include:

- Board members
- Directors
- Officers
- Executive positions
- Appointment dates
- Departure dates
- Historical positions
- Company affiliations
- Board relationships
- Source documentation
- Change tracking

### State Regulatory Module

Organizes state-specific laws and regulations governing utility operations.

Features include:

- State statutes
- Administrative regulations
- Public utility commission rules
- Regulatory orders
- Effective dates
- Expiration dates
- Regulatory agencies
- Jurisdiction
- Applicable utility categories
- Source documents
- Historical versions

### Billing & Rates Module

Tracks utility billing structures and applicable requirements.

Features include:

- Residential rates
- Commercial rates
- Industrial rates
- Fixed charges
- Usage charges
- Demand charges
- Connection fees
- Deposits
- Late fees
- Disconnection fees
- Reconnection fees
- Taxes
- Surcharges
- Credits
- Discounts
- Tariffs
- Billing procedures
- Effective dates
- Historical rate changes

### Compliance Module

Connects utility practices with applicable laws and regulations.

Features include:

- Compliance requirements
- Provider obligations
- Compliance status
- Potential violations
- Confirmed violations
- Enforcement actions
- Penalties
- Fines
- Corrective actions
- Regulatory orders
- Evidence records
- Compliance history

The system should distinguish between an automated finding, an alleged violation, a regulatory finding, and a confirmed legal violation. InfraOpen should not automatically characterize a company as legally non-compliant solely because an automated rule identifies a potential discrepancy.

### Infrastructure Module

Maps physical and digital infrastructure.

Electricity infrastructure may include:

- Generation facilities
- Transmission infrastructure
- Distribution infrastructure
- Substations
- Transformers
- Interconnections
- Storage facilities
- Service territories

Internet infrastructure may include:

- Fiber networks
- Wireless infrastructure
- Internet service territories
- Access points
- Public Wi-Fi locations
- Network nodes
- Community connectivity infrastructure

### Financial Module

Tracks publicly available financial and economic information.

Features include:

- Revenue
- Operating expenses
- Net income
- Profit margins
- Debt
- Credit ratings
- Capital expenditures
- Infrastructure investment
- Subsidies
- Tax incentives
- Grants
- Rate cases
- Financial history

### Energy & Sustainability Module

Tracks electricity generation and environmental characteristics.

Features include:

- Energy source
- Generation mix
- Coal
- Natural gas
- Nuclear
- Hydro
- Wind
- Solar
- Battery storage
- Renewable generation
- Emissions
- Carbon intensity
- Renewable commitments
- Sustainability targets
- Grid modernization

### Reliability Module

Tracks utility service reliability.

Features include:

- Outage frequency
- Outage duration
- Reliability metrics
- Service interruptions
- Planned outages
- Emergency outages
- Restoration times
- Reliability investments
- Historical reliability trends

### Consumer Complaints Module

Organizes publicly available consumer complaint and dispute information.

Features include:

- Complaint type
- Complaint date
- Provider
- Regulatory agency
- Subject
- Resolution
- Enforcement referral
- Resolution date
- Historical complaint trends

### Historical Records Module

InfraOpen should preserve historical information rather than replacing old records with current values.

Historical tracking should include:

- Ownership changes
- Board changes
- Officer changes
- Rate changes
- Regulatory changes
- Compliance changes
- Infrastructure changes
- Provider mergers
- Provider acquisitions
- Service territory changes
- Data corrections

Every significant change should have a timestamp, source, and provenance record.

### Data Provenance Module

Every important record should be traceable to its source.

Provenance records should include:

- Source organization
- Source title
- Source location
- Publication date
- Effective date
- Retrieval date
- Data contributor
- Verification status
- Supporting documentation
- Data confidence
- Previous version

The provenance system is essential for maintaining public trust and allowing users to independently verify information.

### Geographic Information Module

Provides geographic organization and mapping capabilities.

Features include:

- State boundaries
- Counties
- Municipalities
- Utility territories
- Infrastructure locations
- Service areas
- Coverage maps
- Geographic relationships
- Spatial searches
- GIS data imports and exports

### API Module

Provides programmatic access to InfraOpen data.

The API should support:

- Provider searches
- Company searches
- Ownership queries
- Governance queries
- Regulatory queries
- Billing queries
- Compliance queries
- Infrastructure queries
- Geographic queries
- Historical queries
- Source and provenance queries

### Search Module

Provides unified search across the InfraOpen database.

Users should be able to search for:

- Companies
- Utility providers
- Parent companies
- Board members
- Officers
- States
- Laws
- Regulations
- Rates
- Compliance records
- Infrastructure
- Historical events

### Notification Module

Provides alerts when important information changes.

Potential notifications include:

- Ownership changes
- Board appointments
- Officer changes
- Rate changes
- New regulatory rules
- Compliance findings
- Enforcement actions
- Infrastructure changes
- Provider status changes

## Optional Plugin Modules

Optional plugins allow InfraOpen to expand without increasing the complexity of the core platform.

### Internet Utility Plugin

Adds expanded support for the future transition of internet access into a regulated utility.

Potential features include:

- Internet utility providers
- Internet utility regulations
- Household connectivity requirements
- Utility pricing
- Network access requirements
- Provider coverage
- Public Wi-Fi requirements
- Infrastructure sharing
- Community connectivity
- Internet service compliance

### Public Wi-Fi Plugin

Tracks public connectivity infrastructure.

Features may include:

- Business hotspots
- Municipal hotspots
- Provider-operated hotspots
- Public access locations
- Coverage areas
- Availability
- Authentication requirements
- Network ownership
- Infrastructure status

### Utility Comparison Plugin

Provides consumer comparison tools for multiple utility providers.

Comparison categories may include:

- Rates
- Fees
- Reliability
- Complaint history
- Compliance history
- Renewable energy
- Service coverage
- Infrastructure investment

### Advanced Compliance Plugin

Provides more sophisticated regulatory analysis.

Features may include:

- Rule engines
- Automated tariff analysis
- Regulatory document parsing
- Cross-state regulatory comparisons
- Potential violation detection
- Compliance scoring
- Regulatory change monitoring

### Corporate Intelligence Plugin

Provides expanded corporate relationship analysis.

Features may include:

- Corporate ownership graphs
- Board interlocks
- Subsidiary networks
- Mergers and acquisitions
- Shareholder relationships
- Corporate family trees
- Historical corporate structures

### Lobbying & Political Activity Plugin

Tracks publicly available information regarding utility industry political activity.

Potential data includes:

- Lobbying expenditures
- Lobbying registrations
- Political contributions
- Public policy filings
- Regulatory advocacy
- Legislative activity

### Environmental Intelligence Plugin

Provides deeper analysis of environmental performance.

Features may include:

- Emissions analysis
- Generation mix trends
- Renewable development
- Environmental permits
- Storage deployment
- Resource planning
- Environmental enforcement

### Reliability Analytics Plugin

Provides advanced analysis of utility reliability.

Features may include:

- Reliability scoring
- Outage pattern analysis
- Restoration performance
- Geographic reliability analysis
- Historical outage trends
- Infrastructure risk analysis

### Consumer Billing Analyzer Plugin

Provides advanced consumer billing analysis.

Features may include:

- Bill reconstruction
- Rate calculation
- Tariff comparison
- Fee analysis
- Billing anomaly detection
- Historical bill comparison
- Estimated versus actual usage analysis

### Data Quality Plugin

Provides automated quality-control tools.

Features may include:

- Duplicate detection
- Missing data detection
- Conflicting source detection
- Outdated record detection
- Source verification
- Confidence scoring
- Data completeness scoring

### Research & Analytics Plugin

Provides tools for researchers and analysts.

Features may include:

- Statistical analysis
- Trend analysis
- Historical comparisons
- Exportable datasets
- Custom queries
- Research workspaces
- Data visualization

### Cross-Utility Plugin

Expands InfraOpen beyond electricity and internet.

Potential future utility categories include:

- Water
- Natural gas
- Wastewater
- Telecommunications
- District heating
- Public transportation infrastructure

## Data Architecture

InfraOpen should use a relational database architecture capable of maintaining complex relationships and historical records.

The data model should prioritize:

- Stable entity identifiers
- Normalized company records
- Many-to-many relationships
- Historical versioning
- Geographic relationships
- Source provenance
- Temporal data
- Auditability
- Extensibility

PostgreSQL is the preferred core database architecture, with appropriate geographic extensions for GIS functionality.

## Data Ingestion

Data ingestion should be modular and source-specific.

Potential sources include:

- State public utility commissions
- State government agencies
- Federal regulatory agencies
- Federal energy datasets
- Federal communications datasets
- Corporate filings
- Annual reports
- Regulatory filings
- Utility tariffs
- Public enforcement records
- Government GIS datasets
- Public corporate records

Each ingestion connector should be independently maintained and should produce normalized records compatible with the InfraOpen data model.

## Verification System

InfraOpen should distinguish between raw data, normalized data, verified data, and analytical conclusions.

A verification workflow should include:

1. Source acquisition
2. Data normalization
3. Entity matching
4. Validation
5. Source verification
6. Human review when necessary
7. Publication
8. Historical versioning
9. Continuous monitoring

Automated systems may identify potential discrepancies, but significant compliance findings should remain distinguishable from confirmed regulatory or legal determinations.

## Update System

InfraOpen should continuously monitor information that changes over time.

Update categories include:

- Corporate leadership
- Ownership
- Rates
- Tariffs
- Laws
- Regulations
- Compliance records
- Infrastructure
- Service territories
- Financial information
- Reliability information

Each record should retain its previous state so that users can understand what changed, when it changed, and what source documented the change.

## Dashboard

The InfraOpen dashboard should provide an accessible interface for exploring the database.

Potential dashboard sections include:

- National overview
- State overview
- Utility directory
- Company profiles
- Ownership maps
- Governance profiles
- Billing and rates
- Compliance
- Infrastructure maps
- Reliability
- Sustainability
- Consumer information
- Historical changes
- Data sources

## Consumer Tools

InfraOpen should provide practical tools for the public.

Potential tools include:

- Utility provider lookup
- Bill estimator
- Billing comparison
- Rate comparison
- Compliance lookup
- Provider ownership lookup
- Infrastructure map
- Service territory lookup
- Complaint history
- Regulatory document lookup
- Change alerts

## API and Open Data

InfraOpen should make its non-restricted data available through an open API and standardized export formats.

Potential formats include:

- JSON
- CSV
- GeoJSON
- SQL
- RDF or other linked-data formats where appropriate

API access should provide clear documentation and preserve source and provenance information.

## Plugin Development

Plugins should:

- Use documented core APIs.
- Avoid modifying core functionality unnecessarily.
- Maintain independent configuration.
- Clearly document external dependencies.
- Include appropriate tests.
- Preserve data provenance.
- Follow project licensing requirements.
- Provide migration documentation when introducing new database structures.

Experimental plugins may be developed independently before consideration for inclusion in the primary InfraOpen distribution.  

## Security

Security is a core requirement because InfraOpen may contain extensive information about critical infrastructure.

The platform should incorporate:

- Secure authentication
- Role-based permissions
- Audit logging
- Input validation
- API security
- Secrets management
- Dependency monitoring
- Secure data ingestion
- Rate limiting
- Security reporting procedures

Sensitive information should not be collected merely because it is technically obtainable. InfraOpen should prioritize lawful, publicly available information relevant to infrastructure transparency.

## Legal and Regulatory Accuracy

InfraOpen is an information and transparency platform, not a court or regulatory agency.

The platform may identify potential discrepancies between reported practices and applicable requirements. Such findings should be clearly labeled and supported by source documentation.

The system should distinguish between:

- Data discrepancy
- Potential compliance issue
- Reported violation
- Regulatory investigation
- Regulatory finding
- Confirmed enforcement action
- Resolved violation

This distinction is important for maintaining accuracy and preventing unsupported legal conclusions.

## Documentation

Documentation should be maintained alongside the software and data architecture.

Documentation should cover:

- Installation
- Configuration
- Database schema
- API
- Data sources
- ETL connectors
- Verification procedures
- Compliance rules
- Plugin development
- Contribution procedures
- Security
- Data licensing
- Governance

## Roadmap

### Phase 1: Foundation

- Establish the core database architecture.
- Create the company and provider entity model.
- Establish state-level organization.
- Implement source and provenance tracking.
- Build the initial API.
- Create basic provider profiles.

### Phase 2: Electricity

- Add electricity manufacturers and distributors.
- Add corporate ownership information.
- Add boards and officers.
- Add state regulatory information.
- Add billing laws and procedures.
- Add rates and tariffs.
- Implement initial compliance analysis.

### Phase 3: Infrastructure

- Add GIS functionality.
- Map service territories.
- Add generation and distribution infrastructure.
- Add reliability information.
- Add historical infrastructure records.

### Phase 4: Internet Utility Infrastructure

- Add internet providers.
- Add internet utility regulatory structures.
- Track network infrastructure.
- Track public Wi-Fi infrastructure.
- Support future utility-access requirements.

### Phase 5: Advanced Intelligence

- Add automated change detection.
- Add advanced compliance analysis.
- Add corporate relationship analysis.
- Add consumer billing analysis.
- Add predictive and historical analytics.

### Phase 6: Plugin Ecosystem

- Publish plugin APIs.
- Establish plugin documentation.
- Create plugin validation standards.
- Enable third-party integrations.
- Expand into additional utility categories.

---

## Roadmap

- [ ] Expand coverage to all 50 U.S. states  
- [ ] Integrate real-time electricity and internet outage monitoring  
- [ ] Add predictive compliance alerts using machine learning  
- [ ] Enable full cross-utility comparison (water, gas, electricity, internet)  
- [ ] Launch public dashboard with interactive maps and analytics  
- [ ] Blockchain-backed verification of critical data  

---

## Disclaimer

InfraOpen is provided as an open-source transparency and research platform. Information may be incomplete, delayed, or subject to changes in underlying laws, regulations, corporate structures, or public records.

Users should consult the applicable government agency, regulatory filing, utility tariff, law, regulation, or other authoritative source before relying on InfraOpen information for legal, financial, regulatory, or operational decisions.

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
  - [https://roxanneardary.com/infraopen/](https://roxanneardary.com/infraopen/)

---

## License & Notice Requirements

InfraOpen is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- InfraOpen specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
