# Aligned Markets

**Built Like Infrastructure, Not Speculation.**

Aligned Markets is an open source, transparent, verifiable single-issuer equity market infrastructure project designed to provide investors with comprehensive visibility into ownership, trading, corporate actions, dividends, governance, security, and market integrity.

The system is designed around a simple principle:

> **If an event affects an investor, the investor should be able to verify what happened, why it happened, and that the resulting state is correct.**

Aligned Markets is intended to be developed as regulated financial infrastructure. Operation of a live securities market, trading venue, broker-dealer function, transfer agency function, clearing or settlement activity, or related financial service may require registration, licensing, regulatory approval, qualified intermediaries, and compliance with applicable laws and regulations.

## Vision

Aligned Markets seeks to establish a market architecture where transparency is structural rather than promotional.

The platform is designed to provide:

- Verifiable ownership
- Deterministic trade execution
- Tamper-evident records
- Transparent market rules
- Secure investor identity
- KYC and AML controls
- Strong authentication
- Dividend transparency
- Corporate action automation
- Continuous market surveillance
- Shareholder governance
- Independent verification
- Public market integrity information
- Reproducible historical market state
- Open source market infrastructure

The project does not treat transparency as a dashboard layered over an opaque system. Transparency is intended to exist throughout the architecture.

## Design Philosophy

### Infrastructure Over Speculation

Aligned Markets is designed as financial infrastructure rather than a speculative trading product.

The architecture prioritizes:

- Correctness
- Security
- Reliability
- Auditability
- Determinism
- Regulatory compliance
- Investor protection
- Operational resilience

### Verification Over Trust

Participants should not need to rely exclusively on statements from the operator.

Where technically and legally appropriate, the system should allow investors, auditors, researchers, and authorized independent observers to verify system behavior independently.

### Privacy With Accountability

Investor identity must be protected while maintaining sufficient accountability for lawful market participation.

Personally identifiable information should remain separated from publicly visible market information wherever practical.

### Open Source by Design

Core market mechanics, verification methods, governance mechanisms, interfaces, and documentation should be developed as open source software.

Open source does not eliminate regulatory obligations. It makes the implementation more inspectable.

# Core Modules

## Market Engine

The Market Engine provides deterministic market execution.

Capabilities include:

- Order submission
- Order validation
- Order cancellation
- Order modification
- Price-time priority
- Deterministic matching
- Trade generation
- Market state transitions
- Trading session management
- Market halt integration
- Circuit breaker integration

The execution engine must produce reproducible outcomes from identical inputs and market state.

Execution rules must be documented, version controlled, and independently testable.

## Order Management

The Order Management module manages the lifecycle of investor orders.

Capabilities include:

- Order creation
- Order validation
- Order status tracking
- Order cancellation
- Order expiration
- Order history
- Signed order authorization
- Duplicate-order protection
- Idempotent processing
- Order event generation

Every material order-state transition should produce a verifiable event.

## Order Book

The Order Book module maintains the current market state.

Capabilities include:

- Bid management
- Ask management
- Price levels
- Available liquidity
- Order priority
- Historical snapshots
- Market depth
- Order-book reconstruction

The system should provide sufficient information for authorized participants and public transparency interfaces without exposing protected personal information.

## Settlement and Ownership

The Settlement and Ownership module maintains the authoritative relationship between securities and their lawful holders.

Capabilities include:

- Share ownership
- Ownership transfers
- Trade settlement
- Share issuance
- Share retirement
- Treasury shares
- Restricted shares
- Ownership reconciliation
- Settlement status
- Historical ownership state

The system must maintain strict controls preventing ownership records from becoming inconsistent with authorized share issuance.

## Proof of Supply

The Proof of Supply module continuously reconciles the authorized share supply.

The system should independently calculate and verify:

- Authorized shares
- Issued shares
- Outstanding shares
- Treasury shares
- Restricted shares
- Retired shares
- Shares available for trading

The system should provide cryptographically verifiable evidence that recorded ownership does not exceed the legally authorized supply.

## Immutable Event Ledger

The Event Ledger records material system events using append-only, tamper-evident records.

Events may include:

- Orders
- Cancellations
- Executions
- Settlements
- Ownership changes
- Dividends
- Corporate actions
- Governance events
- Rule changes
- Administrative actions
- Compliance events
- System events

Cryptographic linking, timestamping, integrity verification, and independent replication should be supported.

## Market Replay

The Market Replay module reconstructs historical market states.

Capabilities include:

- Historical order-book reconstruction
- Trade replay
- Execution verification
- Ownership reconstruction
- Corporate action reconstruction
- Dividend-event reconstruction
- Rule-version reconstruction
- Historical state comparison

An independent verifier should be able to reproduce historical outcomes using the applicable market rules and recorded inputs.

## Identity and KYC

The Identity module provides secure participant identity management.

Capabilities include:

- KYC onboarding
- Identity verification
- Investor eligibility verification
- AML screening integration
- Identity lifecycle management
- Account recovery
- Identity status management
- Regulatory recordkeeping

Identity information should be isolated from public market records wherever legally and technically appropriate.

## Authentication and Access Security

The Authentication module protects investor accounts and administrative systems.

Capabilities include:

- Multi-factor authentication
- Two-factor authentication
- WebAuthn and passkey support
- Hardware security key support
- Session management
- Device management
- Login monitoring
- Account lockout controls
- Risk-based authentication
- Administrative access controls

Trading authorization should require stronger controls than ordinary account access where appropriate.

## Cryptographic Authorization

The Cryptographic Authorization module provides verifiable authorization for sensitive actions.

Capabilities include:

- Digital signatures
- Signed orders
- Signed administrative actions
- Key rotation
- Key revocation
- Transaction authorization
- Non-repudiation
- Signature verification

Sensitive keys should be protected through appropriate hardware-backed security infrastructure.

## Investor Privacy

The Privacy module separates identity from market transparency.

Capabilities may include:

- Pseudonymous market identifiers
- Privacy-preserving ownership proofs
- Selective disclosure
- Data minimization
- Access-controlled personal records
- Cryptographic eligibility proofs

Privacy mechanisms must not interfere with lawful regulatory access or required reporting.

## Dividend Engine

The Dividend Engine manages the lifecycle of dividend events.

Capabilities include:

- Dividend declarations
- Ex-dividend processing
- Record-date snapshots
- Shareholder eligibility
- Dividend calculations
- Payment instructions
- Payment reconciliation
- Failed-payment handling
- Tax reporting support
- Dividend history

The system should provide an auditable reconciliation between declared dividends, eligible shares, calculated obligations, and completed payments.

## Corporate Action Engine

The Corporate Action Engine manages events affecting securities or ownership.

Supported actions may include:

- Stock splits
- Reverse splits
- Share buybacks
- Rights offerings
- New share issuance
- Share retirement
- Spin-offs
- Dividend events
- Other authorized corporate actions

Every corporate action should have a defined lifecycle, versioned rules, authorization records, and auditable results.

## Capital Formation

The Capital Formation module supports authorized issuance of securities.

Capabilities may include:

- New share issuance
- Investor subscriptions
- Rights offerings
- Capital raise processing
- Allocation records
- Subscription verification
- Issuance reconciliation
- Disclosure integration

Capital formation functionality must be implemented only within applicable securities laws and approved offering structures.

## Market Surveillance

The Market Surveillance module monitors trading activity for potentially abusive or manipulative behavior.

Detection categories may include:

- Wash trading
- Spoofing
- Layering
- Excessive cancellation
- Coordinated trading
- Abnormal order timing
- Concentration anomalies
- Unusual liquidity withdrawal
- Price manipulation indicators
- Account relationship patterns

Surveillance should produce explainable alerts, preserve evidence, support investigation workflows, and maintain appropriate confidentiality.

## Coordinated Activity Analysis

The Coordinated Activity module analyzes relationships between trading events and participant activity.

It may identify:

- Synchronized order placement
- Correlated account activity
- Repeated trading relationships
- Unusual timing clusters
- Coordinated accumulation
- Coordinated distribution
- Abnormal cross-account behavior

Detection systems must distinguish statistical correlation from confirmed misconduct and should not automatically treat an alert as proof of manipulation.

## AI Market Monitoring

The AI Monitoring module provides optional analytical assistance for market surveillance.

Capabilities may include:

- Anomaly detection
- Behavioral clustering
- Pattern recognition
- Liquidity analysis
- Temporal analysis
- Risk scoring
- Investigative prioritization

AI-generated alerts must remain explainable, reviewable, and subject to human investigation.

AI systems must not independently determine legal culpability.

## Market Transparency

The Transparency module provides public and investor-facing information about market operation.

Capabilities may include:

- Market status
- Order-book information
- Trade history
- Trading volume
- Ownership statistics
- Share supply information
- Corporate actions
- Dividend history
- Governance activity
- System status
- Market integrity indicators

Public disclosures must respect privacy, securities law, confidentiality obligations, and applicable market-data requirements.

## Ownership Transparency Graph

The Ownership Graph provides a visual representation of aggregate ownership structure.

It may display:

- Ownership concentration
- Major holder changes
- Insider holdings
- Voting power
- Share distribution
- Ownership movement
- Historical concentration

The system must avoid exposing protected personal information.

## Market Integrity Score

The Market Integrity module calculates transparent indicators of market health.

Potential factors include:

- Liquidity stability
- Ownership concentration
- Trading concentration
- Order-book resilience
- Surveillance activity
- Governance participation
- System availability
- Data integrity
- Verification status

The score must publish its methodology and distinguish measurable system conditions from subjective judgments.

## Market Health Dashboard

The Market Health module provides real-time operational information.

Metrics may include:

- System availability
- Order-processing latency
- Settlement status
- Ledger integrity
- Verification status
- Market liquidity
- Trading activity
- Circuit breaker status
- Security status

## Market Stress Simulation

The Simulation module allows authorized users and researchers to model hypothetical market conditions.

Scenarios may include:

- Liquidity shocks
- Large shareholder sales
- Rapid buying
- Dividend changes
- Corporate actions
- Market halts
- Trading concentration
- Infrastructure failures

Simulation environments must remain isolated from production systems.

## Circuit Breakers and Market Halts

The Market Protection module provides controlled responses to abnormal conditions.

Capabilities include:

- Volatility halts
- Liquidity-based pauses
- Technical halts
- Emergency suspension
- Controlled reopening
- Auction-based reopening
- Halt notifications
- Halt audit records

All halt mechanisms must be governed by documented rules.

## Governance

The Governance module provides transparent administration of market rules and shareholder participation.

Capabilities include:

- Governance proposals
- Shareholder voting
- Rule proposals
- Rule versioning
- Governance records
- Voting eligibility
- Voting verification
- Decision publication

Governance mechanisms must remain subject to applicable corporate and securities law.

## Rule Change System

Market rules must be versioned and independently identifiable.

Rule changes should follow:

- Proposal
- Disclosure
- Review
- Approval
- Time lock
- Activation
- Historical archival

The active rule set must always be identifiable for any historical market event.

## Emergency Governance

The Emergency Governance module provides controlled procedures for extraordinary circumstances.

Potential events include:

- Security breaches
- Critical infrastructure failure
- Regulatory intervention
- Data corruption
- Market integrity incidents
- Catastrophic operational events

Emergency authority must be limited, documented, logged, and subject to post-event review.

## Insider Transparency

The Insider Transparency module provides enhanced disclosure and monitoring for company insiders and other legally defined persons.

Capabilities may include:

- Insider ownership records
- Trade disclosures
- Planned trading windows
- Restricted periods
- Corporate event restrictions
- Disclosure history

All functionality must comply with applicable insider trading laws and regulations.

## Investor Notifications

The Notification module delivers important investor communications.

Events may include:

- Dividend declarations
- Corporate actions
- Governance proposals
- Voting deadlines
- Market halts
- Insider disclosures
- Rule changes
- Security events
- Account events

## Shareholder Communications

The Shareholder Communications module provides controlled communication between the company and verified shareholders.

Capabilities may include:

- Official announcements
- Shareholder questions
- Governance discussions
- Investor information
- Meeting notices
- Voting communications

## Audit

The Audit module maintains records necessary for internal and external verification.

Capabilities include:

- Administrative audit logs
- Security audit records
- Financial reconciliation
- Market-rule verification
- System integrity verification
- Access auditing
- Compliance evidence
- Historical audit packages

## Independent Verification

Aligned Markets supports independent verification participants.

Authorized verification nodes may validate:

- Ledger integrity
- Share supply
- Trade sequence
- Market state
- Dividend calculations
- Corporate actions
- Governance results

Verification results should be independently signed and archived.

## Global Verification Network

The Global Verification Network extends independent verification to external organizations such as:

- Universities
- Research institutions
- Auditors
- Financial researchers
- Qualified independent observers

The network is intended to create continuous external validation without granting independent nodes unauthorized control over the market.

## Disaster Recovery

The Disaster Recovery module provides operational resilience.

Capabilities include:

- Geographic redundancy
- Encrypted backups
- Backup integrity verification
- Recovery testing
- Failover procedures
- Disaster recovery exercises
- Business continuity procedures

## Security Operations

The Security Operations module monitors infrastructure and application security.

Capabilities include:

- Security event monitoring
- Threat detection
- Access monitoring
- Vulnerability management
- Incident response
- Security logging
- Key management
- Security testing

## Bug Bounty

Aligned Markets should maintain a responsible vulnerability disclosure program.

Security researchers should have a documented process for reporting vulnerabilities without exposing investors or the market to unnecessary risk.

## Open Audit Program

The Open Audit module supports independent examination of:

- Market algorithms
- Ledger integrity
- Security controls
- Financial reconciliation
- Governance processes
- Surveillance systems

Public disclosure of audit findings should balance transparency with security and legal requirements.

## Data API

The Data API provides controlled access to market information.

Potential resources include:

- Market data
- Historical trades
- Market statistics
- Corporate actions
- Dividend history
- Governance records
- System status
- Verification records

API access must respect privacy, security, licensing, and regulatory requirements.

## Developer Sandbox

The Developer Sandbox provides a non-production environment for:

- Trading simulations
- API development
- Market-model testing
- Surveillance research
- Governance experiments
- Integration testing

No sandbox activity may affect production ownership or settlement records.

## Research Laboratory

The Research module provides a framework for studying:

- Market microstructure
- Market fairness
- Surveillance
- Governance
- Ownership concentration
- Liquidity
- Economic behavior
- Cryptographic verification
- Financial system resilience

## Historical Transparency Library

The Historical Library provides searchable access to authorized historical information.

Materials may include:

- Trade records
- Market states
- Corporate actions
- Dividend records
- Governance decisions
- Rule versions
- Audit results
- Verification records

## Fee Transparency

All applicable fees should be clearly disclosed.

The system should provide transparent information about:

- Trading fees
- Settlement costs
- Payment costs
- Administrative fees
- Other investor charges

Hidden fees and undisclosed preferential arrangements are contrary to the project's transparency principles.

## Operational Sustainability

The Sustainability module may measure:

- Energy consumption
- Infrastructure utilization
- Operational efficiency
- Data-center efficiency
- Environmental impact

## Compliance Automation

The Compliance module supports regulatory and legal reporting workflows.

Capabilities may include:

- Regulatory data collection
- Reporting preparation
- Record retention
- Compliance alerts
- Investor eligibility controls
- Transaction monitoring
- Audit evidence

The system is intended to support compliance, not replace qualified legal, regulatory, compliance, accounting, or financial professionals.

# Optional Plugin Modules

Aligned Markets uses a modular architecture in which optional capabilities can be added without changing the fundamental market engine.

## Alternative Settlement Plugin

Provides integrations with approved settlement providers and financial infrastructure.

## Banking Rails Plugin

Provides integrations for authorized payment systems supporting investor deposits, withdrawals, and dividend payments.

## Tax Reporting Plugin

Provides jurisdiction-specific tax reporting and documentation.

## Advanced KYC Plugin

Provides additional identity verification, document verification, sanctions screening, and jurisdiction-specific compliance capabilities.

## Accreditation Verification Plugin

Provides investor eligibility verification where an offering or market structure requires accredited-investor or other eligibility status.

## Zero-Knowledge Verification Plugin

Provides optional privacy-preserving proofs for ownership and eligibility.

## Advanced Surveillance Plugin

Provides specialized surveillance models beyond the core monitoring system.

## Institutional Verification Plugin

Provides interfaces for qualified independent auditors, researchers, and verification organizations.

## External Market Data Plugin

Provides optional integrations with authorized external market-data providers.

## Multi-Currency Plugin

Provides support for authorized multi-currency valuation, payment, and dividend workflows.

## International Compliance Plugin

Provides jurisdiction-specific compliance modules for approved international participation.

## Advanced Governance Plugin

Provides additional shareholder governance mechanisms such as proposal workflows, delegated voting, advisory voting, and specialized governance analytics.

## Research Analytics Plugin

Provides advanced statistical analysis and research tooling for approved users.

## AI Research Plugin

Provides optional experimental AI models for market analysis, simulation, and surveillance research.

## Notification Provider Plugin

Supports integrations with approved email, messaging, push notification, and other communication providers.

## Accessibility Plugin

Provides enhanced accessibility capabilities for investors and administrators.

## Localization Plugin

Provides international language, formatting, date, time, and jurisdiction-specific presentation support.

# Plugin Principles

Optional plugins must:

- Maintain the integrity of the core market engine
- Respect security boundaries
- Respect privacy controls
- Maintain auditability
- Provide documented interfaces
- Avoid undisclosed market advantages
- Preserve deterministic behavior where applicable
- Clearly disclose external dependencies
- Remain independently testable

Plugins must not silently modify core market rules or bypass compliance controls.

# Verification Model

Aligned Markets is designed around multiple layers of verification.

## Transaction Verification

Each material transaction should be independently validated against:

- Authorized identity
- Account permissions
- Available securities
- Applicable market rules
- Order state
- Settlement state

## Ledger Verification

Ledger integrity should be continuously checked through:

- Cryptographic hashes
- Event sequence validation
- Signature verification
- Replicated records
- Consistency checks

## Supply Verification

The system should continuously reconcile:

- Authorized supply
- Issued supply
- Outstanding supply
- Treasury holdings
- Investor holdings
- Retired securities

## Historical Verification

Historical market states should be reproducible using:

- Recorded events
- Applicable rules
- Corporate actions
- Ownership records
- Settlement records

# Regulatory Architecture

Aligned Markets is designed with regulatory compliance as a foundational requirement.

Depending on the final structure and activities, regulatory considerations may include:

- Securities registration or exemption
- Broker-dealer requirements
- Trading venue requirements
- Alternative Trading System requirements
- Transfer agent requirements
- Clearing and settlement requirements
- KYC and AML obligations
- Investor eligibility requirements
- Market surveillance
- Recordkeeping
- Reporting
- Tax documentation
- Corporate governance
- Privacy and data protection

The technical architecture must be developed alongside qualified securities counsel, compliance professionals, financial institutions, and applicable regulators.

Open source licensing does not create an exemption from financial regulation.

# Investor Protection

Investor protection is a primary design requirement.

The system should provide:

- Clear disclosures
- Secure account access
- Transparent market rules
- Verifiable ownership
- Accurate dividend calculations
- Market surveillance
- Error correction procedures
- Complaint and dispute processes
- Business continuity
- Data protection
- Regulatory reporting

# Market Integrity Charter

Aligned Markets is founded on the following commitments:

- No hidden market mechanics
- No undisclosed preferential execution
- No intentional information asymmetry
- No unauthorized creation of securities
- No silent rule changes
- No unexplained ownership changes
- No concealed corporate actions
- No undisclosed fees
- No anonymous production access
- No bypassing of required regulatory controls

Where confidentiality is legally required, the system should preserve confidentiality while maintaining verifiable evidence of compliance.

# Development Principles

Development should prioritize:

- Security before convenience
- Correctness before performance
- Determinism before complexity
- Auditability before abstraction
- Modularity before coupling
- Open standards before proprietary dependencies
- Reproducibility before trust
- Investor protection before feature expansion

# Future Expansion

The architecture is designed to support future development without compromising the single-issuer foundation.

Potential future capabilities include:

- Expanded verification networks
- Advanced privacy-preserving proofs
- Additional settlement integrations
- Multi-jurisdiction compliance
- Expanded corporate action support
- Advanced market simulations
- Institutional research access
- Additional investor services

Any expansion must remain consistent with the project's transparency, security, governance, and regulatory principles.  

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
  - [https://roxanneardary.com/alignedmarkets/](https://roxanneardary.com/alignedmarkets/)

---

## License & Notice Requirements

Aligned Markets is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- Aligned Markets specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.  
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  
