# CivicTrust
**Verifying Actions, Protecting Communities**
- HTML Mirror:  [https://roxanneardary.com/civictrust-specification/](https://roxanneardary.com/civictrust-specification/)

---

CivicTrust is an open-source, privacy-first accountability system for autonomous agents and distributed automated systems. It provides universal infrastructure for verifiable identity, human-anchored stewardship, traceable actions, privacy-preserving verification, constitutional governance, and enforceable accountability.

CivicTrust is designed to operate without dependence on Big Tech identity providers, proprietary KYA platforms, centralized ownership systems, or blockchain-only identity and accountability mechanisms.

The system uses a modular architecture in which core capabilities operate as independent modules while remaining interoperable through shared CivicTrust protocols, APIs, schemas, and verification mechanisms.

# Purpose

CivicTrust establishes a common accountability layer for autonomous systems.

The system is designed to ensure that:

- Every participating agent can establish a verifiable identity.
- Every autonomous agent has a human or organizational steward.
- Agent capabilities and authority can be independently verified.
- Significant actions can produce cryptographically verifiable records.
- Constitutional rules can be expressed as machine-readable policies.
- Violations can trigger defined enforcement actions.
- Verification can occur without unnecessary disclosure of personal information.
- Independent networks can establish their own trust policies while remaining interoperable.
- Communities can audit participating systems without surrendering control to a centralized provider.
- Autonomous systems remain accountable to identifiable human responsibility.

## Human-in-the-Loop Governance

CivicTrust supports human approval, review, escalation, intervention, and accountability for actions that require human authority.

---

# Core Modules

## Identity Core

The Identity Core provides cryptographic identity services for humans, agents, organizations, nodes, and other authorized entities.

Features include:

- Decentralized identifiers
- Cryptographic key management
- Identity creation
- Identity verification
- Identity resolution
- Identity rotation
- Key rotation
- Identity revocation
- Identity recovery
- Delegated identity authority
- Multi-key identities
- Identity status
- Cross-network identity verification
- Identity federation
- Identity metadata minimization
- Identity lifecycle management
- Identity proof generation
- Identity proof verification

The Identity Core separates identity verification from unnecessary disclosure of personal information.

## Stewardship Core

The Stewardship Core establishes the human accountability relationship for autonomous agents.

Features include:

- Proof-of-Human Stewardship
- Human steward registration
- Agent-to-steward relationships
- Organization-to-agent relationships
- Multiple steward support
- Delegated stewardship
- Steward authorization
- Steward revocation
- Agent ownership transfer
- Emergency stewardship procedures
- Steward activity records
- Steward accountability records
- Steward status verification
- Steward succession
- Steward dispute handling
- Agent suspension by steward
- Agent retirement by steward

The Stewardship Core provides a clear accountability chain without requiring public disclosure of unnecessary personal information.

## Credential Core

The Credential Core manages verifiable claims concerning identities, authority, capabilities, roles, certifications, and relationships.

Features include:

- Verifiable credentials
- Credential issuance
- Credential verification
- Credential presentation
- Credential expiration
- Credential revocation
- Credential suspension
- Credential renewal
- Selective disclosure
- Credential status verification
- Credential chaining
- Credential versioning
- Capability credentials
- Stewardship credentials
- Agent authorization credentials
- Organization credentials
- Cross-network credential verification
- Credential policy enforcement
- Credential history
- Credential provenance

The Credential Core should support established open credential standards where practical.

## Constitution Core

The Constitution Core provides the policy and governance enforcement layer.

Features include:

- Machine-readable constitutions
- Policy definitions
- Rule evaluation
- Permission policies
- Agent capability restrictions
- Required disclosure policies
- Required logging policies
- Stewardship requirements
- Data handling requirements
- Communication policies
- Operational restrictions
- Constitutional versioning
- Constitutional amendments
- Policy inheritance
- Policy exceptions
- Compliance evaluation
- Violation detection
- Enforcement actions
- Policy simulation
- Policy testing
- Constitutional audit records
- Constitutional history
- Rule dependency management
- Policy conflict detection
- Policy precedence
- Emergency policy controls

Constitutions may be defined at the network, organization, agent class, or individual agent level, subject to applicable governance rules.

## Action and Evidence Core

The Action and Evidence Core creates verifiable records of significant agent activity.

Features include:

- Cryptographically signed actions
- Action identifiers
- Event identifiers
- Timestamped events
- Append-only records
- Tamper-evident records
- Hash-linked records
- Merkle-based verification
- Action provenance
- Evidence collection
- Evidence integrity verification
- Action sequencing
- Action relationships
- Agent activity history
- Evidence export
- Evidence verification
- Audit evidence packages
- Event retention policies
- Evidence retention policies
- Evidence access controls
- Selective evidence disclosure

The Action and Evidence Core should allow an authorized verifier to establish what happened, which agent performed an action, under whose authority the agent operated, and whether the record has been altered.

## Audit Log Core

The Audit Log Core maintains the operational audit trail for CivicTrust networks.

Features include:

- Agent audit logs
- Steward audit logs
- Credential audit logs
- Governance audit logs
- Constitution audit logs
- Security audit logs
- Administrative audit logs
- Log integrity verification
- Log indexing
- Log search
- Log retention
- Log archival
- Log export
- Audit trail reconstruction
- Independent log verification
- Distributed log synchronization

Audit logs should support privacy-preserving access controls and should not expose sensitive information unnecessarily.

## Trust Registry Core

The Trust Registry Core maintains information required to evaluate trust relationships.

Features include:

- Trusted issuer registry
- Agent registry
- Steward registry
- Organization registry
- Credential registry
- Revoked identity registry
- Revoked credential registry
- Revoked key registry
- Compromised identity registry
- Trust authority registry
- Federation registry
- Registry synchronization
- Registry versioning
- Registry snapshots
- Registry verification
- Registry history
- Public verification endpoints
- Local trust policies
- Network trust policies

Trust registries may be independently operated and synchronized according to federation policies.

## Verification Core

The Verification Core allows agents, organizations, communities, and independent auditors to verify CivicTrust claims.

Features include:

- Identity verification
- Stewardship verification
- Credential verification
- Signature verification
- Action verification
- Evidence verification
- Constitution compliance verification
- Policy verification
- Trust registry verification
- Revocation verification
- Key status verification
- Reputation verification
- Cross-network verification
- Selective disclosure verification
- Zero-knowledge verification

Verification should be possible without requiring the verifier to trust a single centralized service.

## Privacy Core

The Privacy Core provides privacy-preserving mechanisms throughout CivicTrust.

Features include:

- Selective disclosure
- Zero-knowledge proofs
- Anonymous credential support
- Pseudonymous identifiers
- Metadata minimization
- Data minimization
- Encrypted storage
- Encrypted communication
- Local-first processing
- Privacy-preserving verification
- Consent-based disclosure
- Data retention controls
- Data access controls
- Privacy policy enforcement
- Identity compartmentalization
- Private agent relationships

The Privacy Core should ensure that accountability does not require unnecessary surveillance.

## Reputation Core

The Reputation Core provides evidence-based reputation information for agents, stewards, organizations, and trust authorities.

Features include:

- Agent reputation
- Steward reputation
- Organization reputation
- Trust authority reputation
- Reputation history
- Reliability metrics
- Integrity metrics
- Transparency metrics
- Constitutional compliance metrics
- Audit history
- Community attestations
- Reputation decay
- Reputation recovery
- Reputation disputes
- Reputation evidence
- Reputation verification
- Reputation portability

Reputation must be evidence-based and should not become an opaque centralized score that cannot be independently evaluated.

## Communication Core

The Communication Core provides secure communication between participating entities.

Features include:

- Agent-to-agent communication
- Agent-to-human communication
- Human-to-agent communication
- Organization-to-agent communication
- Encrypted messaging
- Signed messages
- Message verification
- Secure channels
- Peer-to-peer communication
- Event notifications
- Message routing
- Communication authorization
- Communication policy enforcement
- Message integrity verification
- Communication audit records

The Communication Core should support interoperable secure messaging protocols.

## Governance Core

The Governance Core provides mechanisms for managing CivicTrust networks and their constitutional systems.

Features include:

- Governance structures
- Steward governance
- Community proposals
- Policy proposals
- Constitutional amendments
- Voting mechanisms
- Delegated voting
- Governance records
- Governance transparency
- Governance roles
- Council management
- Authority delegation
- Governance disputes
- Emergency governance procedures
- Governance audit trails

Governance mechanisms should remain configurable so independent CivicTrust networks can establish their own legitimate governance structures.

## Compliance Core

The Compliance Core evaluates agents and organizations against applicable rules and policies.

Features include:

- Constitution compliance
- Policy compliance
- Credential compliance
- Stewardship compliance
- Logging compliance
- Privacy compliance
- Operational compliance
- Configuration compliance
- Compliance reports
- Compliance evidence
- Compliance alerts
- Compliance history
- Remediation workflows
- Compliance verification
- Compliance status

## Incident Core

The Incident Core manages violations, security events, suspected abuse, and accountability incidents.

Features include:

- Incident creation
- Incident classification
- Incident evidence collection
- Incident investigation
- Incident escalation
- Steward notification
- Auditor notification
- Agent suspension
- Agent quarantine
- Credential suspension
- Credential revocation
- Key revocation
- Remediation tracking
- Incident resolution
- Incident history
- Incident reporting

## Security Core

The Security Core protects CivicTrust infrastructure and cryptographic assets.

Features include:

- Secure key storage
- Key rotation
- Key revocation
- Key recovery
- Multi-signature authorization
- Hardware security module support
- Trusted platform module support
- Secure enclave integration
- Cryptographic verification
- Secure configuration
- Access controls
- Authentication
- Authorization
- Security event monitoring
- Supply chain integrity
- Dependency verification
- Secure update mechanisms

## Federation Core

The Federation Core allows independently operated CivicTrust networks to interoperate.

Features include:

- Network federation
- Cross-network identity verification
- Cross-network credential verification
- Cross-network trust
- Cross-network reputation
- Federation policies
- Federation authorization
- Federation registries
- Federation discovery
- Federation synchronization
- Federation revocation
- Federation dispute handling
- Federation governance

Federation must remain optional so a deployment can operate independently without joining an external network.

## API Core

The API Core provides standardized interfaces for CivicTrust functionality.

Features include:

- REST APIs
- GraphQL APIs
- WebSocket interfaces
- Event APIs
- Verification APIs
- Identity APIs
- Credential APIs
- Stewardship APIs
- Logging APIs
- Governance APIs
- Reputation APIs
- Federation APIs
- Webhook support
- Authentication
- Authorization
- API versioning
- Rate limiting
- API audit logging

## SDK Core

The SDK Core provides tools for integrating CivicTrust into autonomous systems.

Features include:

- Agent SDKs
- Identity SDKs
- Credential SDKs
- Stewardship SDKs
- Logging SDKs
- Constitution SDKs
- Verification SDKs
- Communication SDKs
- Governance SDKs
- API clients
- Event clients
- Plugin development interfaces
- Integration helpers
- Testing utilities

SDK implementations may be provided for multiple programming languages.

## CLI Core

The CLI Core provides command-line administration and integration tools.

Features include:

- Identity management
- Steward registration
- Agent registration
- Credential management
- Constitution management
- Action verification
- Log inspection
- Trust registry inspection
- Reputation inspection
- Incident management
- Governance operations
- Federation management
- Configuration management
- Diagnostics
- Security checks

## Schema Core

The Schema Core defines interoperable data structures used throughout CivicTrust.

Features include:

- Identity schemas
- Agent schemas
- Stewardship schemas
- Credential schemas
- Action schemas
- Evidence schemas
- Constitution schemas
- Policy schemas
- Audit schemas
- Reputation schemas
- Governance schemas
- Incident schemas
- Federation schemas
- Versioned schemas
- Schema validation
- Schema compatibility

---

# Optional Plugin Modules

Optional plugins extend CivicTrust without making additional capabilities mandatory for every deployment.

## Blockchain Adapter Plugin

Provides optional integration with blockchain networks for anchoring or verification.

Features include:

- Hash anchoring
- Timestamp anchoring
- Public verification
- Smart contract adapters
- Chain-specific integrations

Blockchain is an optional verification mechanism and is not required for CivicTrust identity, stewardship, logging, governance, or accountability.

## Hardware Trust Plugin

Provides optional hardware-backed identity and key protection.

Features include:

- TPM integration
- Secure enclave integration
- Hardware-backed signatures
- Hardware identity attestation
- Secure key storage
- Hardware integrity verification

## Zero-Knowledge Plugin

Provides optional advanced zero-knowledge verification mechanisms.

Features include:

- Private compliance proofs
- Private identity claims
- Credential proofs
- Attribute proofs
- Policy compliance proofs
- Selective disclosure proofs

## DID Method Plugin

Provides support for additional decentralized identifier methods.

Features include:

- DID method adapters
- DID resolution
- DID registration
- DID verification
- DID method discovery
- Cross-method interoperability

## Credential Provider Plugin

Allows CivicTrust networks to integrate external credential issuers.

Features include:

- Credential issuer adapters
- Credential verification adapters
- Credential status adapters
- Credential transformation
- Credential interoperability

## Transparency Log Plugin

Provides integrations with external transparency log implementations.

Features include:

- Transparency log publishing
- Merkle verification
- External log synchronization
- Inclusion proofs
- Log consistency verification

## Hardware Security Module Plugin

Provides optional integration with external HSM systems.

Features include:

- HSM-backed signing
- Key generation
- Key storage
- Key rotation
- Key revocation
- Hardware-backed authorization

## Communication Protocol Plugin

Provides adapters for additional secure communication protocols.

Features include:

- Protocol adapters
- Message translation
- Identity binding
- Signature verification
- Routing integration
- Protocol-specific authorization

## Identity Provider Adapter Plugin

Provides optional interoperability with external identity systems.

Features include:

- Identity federation
- Credential translation
- External identity verification
- Enterprise integration
- Legacy identity interoperability

External identity providers must remain optional and must not become a required CivicTrust dependency.

## Agent Framework Plugin

Provides integrations with existing autonomous agent frameworks.

Features include:

- Agent registration
- Agent identity binding
- Action interception
- Action logging
- Credential verification
- Constitution enforcement
- Stewardship integration
- Framework-specific event handling

## Security Monitoring Plugin

Provides integration with external security monitoring systems.

Features include:

- Security event ingestion
- Threat detection integration
- Incident creation
- Agent quarantine
- Credential suspension
- Security audit integration

## Civic Network Plugin

Provides tools for community and civic deployments.

Features include:

- Public verification
- Community reporting
- Civic audit interfaces
- Community attestations
- Public accountability records
- Community governance integration

## Governance Plugin

Provides optional governance models for specific networks.

Features include:

- Council systems
- Voting systems
- Delegation
- Proposal management
- Constitutional amendment workflows
- Governance records
- Dispute resolution

## Reputation Provider Plugin

Allows external reputation systems to provide verifiable reputation evidence.

Features include:

- Reputation provider integration
- Reputation attestations
- Reputation verification
- Reputation history import
- Reputation portability

## Storage Plugin

Provides adapters for different storage systems.

Features include:

- Local storage
- Distributed storage
- Content-addressed storage
- Object storage
- Database storage
- Encrypted storage
- Storage replication
- Storage migration

## Analytics Plugin

Provides optional analytics without making analytics part of the accountability core.

Features include:

- Agent activity analytics
- Compliance analytics
- Network analytics
- Incident analytics
- Reputation analytics
- Governance analytics
- Privacy-preserving aggregate reporting

## Notification Plugin

Provides optional notification integrations.

Features include:

- Steward alerts
- Security alerts
- Compliance alerts
- Credential expiration alerts
- Credential revocation alerts
- Incident alerts
- Governance notifications
- Webhook notifications

---

# Interoperability Requirements

CivicTrust implementations should:

- Use documented protocols.
- Expose stable interfaces.
- Support versioned schemas.
- Avoid unnecessary vendor-specific dependencies.
- Support independent implementations.
- Permit replacement of individual modules.
- Support federation where enabled.
- Preserve cryptographic verification across implementations.
- Maintain backward compatibility where practical.

# Extensibility

CivicTrust must allow new capabilities to be introduced without modifying the fundamental accountability model.

New functionality should be implemented as:

- Core module functionality when it is fundamental to accountability.
- Optional plugin functionality when it provides specialized integration or deployment-specific capabilities.
- External services when the functionality does not need to be part of the CivicTrust trust boundary.

Plugins must use documented interfaces and must not silently bypass identity, stewardship, logging, privacy, or constitutional controls.

# Security Requirements

CivicTrust implementations should:

- Protect private keys.
- Verify signatures before accepting authenticated claims.
- Validate credentials before accepting delegated authority.
- Check revocation status where required.
- Prevent unauthorized stewardship changes.
- Protect audit records from unauthorized modification.
- Protect sensitive information from unnecessary disclosure.
- Support secure key rotation.
- Provide secure recovery mechanisms.
- Record security-sensitive administrative actions.
- Validate plugin permissions.
- Protect module boundaries.
- Maintain dependency integrity.
- Provide mechanisms for incident response.

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
  - [https://roxanneardary.com/civictrust/](https://roxanneardary.com/civictrust/)

---

## License & Notice Requirements

CivicTrust is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.  
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- CivicTrust specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.  
  Any update that adds new contributors or modifies attribution should also update `notice.md`.  
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  
