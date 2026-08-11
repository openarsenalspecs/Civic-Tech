# Umbrix

**Adaptive privacy for a connected world.**

Umbrix is a commercial-grade, open-source privacy and network security platform designed to provide adaptive network obfuscation, multi-node routing, privacy-preserving communications, and cross-platform protection.

Umbrix is built as a modular system. Core modules provide the foundational networking, cryptographic, routing, privacy, and security capabilities required for the platform to operate, while optional plugin modules extend Umbrix with specialized functionality without requiring those capabilities to be installed or enabled.

Umbrix is designed for individuals, organizations, developers, self-hosted deployments, privacy-focused infrastructure, and locally hosted AI systems that require privacy to extend beyond the application layer and into the underlying network.

---

## Table of Contents

- [Project Goals](#project-goals)
- [Design Principles](#design-principles)
- [Architecture](#architecture)
- [Core Modules](#core-modules)
- [Optional Plugin Modules](#optional-plugin-modules)
- [Client Architecture](#client-architecture)
- [Node Architecture](#node-architecture)
- [Control Plane](#control-plane)
- [Routing Architecture](#routing-architecture)
- [Protocol Architecture](#protocol-architecture)
- [Privacy Architecture](#privacy-architecture)
- [Security Architecture](#security-architecture)
- [Cross-Platform Support](#cross-platform-support)
- [AI Privacy](#ai-privacy)
- [Developer Platform](#developer-platform)
- [Configuration](#configuration)
- [Deployment](#deployment)
- [Testing and Verification](#testing-and-verification)
- [Roadmap](#roadmap)
- [License](#license)
- [Attribution](#attribution)

---

## Project Goals

Umbrix is designed around several primary objectives:

- Hide the user's public IP address from destination services.
- Separate network origin from destination traffic.
- Support configurable multi-node routing.
- Provide adaptive network obfuscation.
- Reduce traffic-analysis and fingerprinting exposure.
- Protect DNS and other metadata from unnecessary disclosure.
- Provide privacy controls across desktop and mobile platforms.
- Support self-hosted and distributed infrastructure.
- Provide a modular architecture for future privacy technologies.
- Give locally hosted AI systems a privacy layer by default.
- Minimize centralized dependencies and vendor lock-in.
- Provide transparent, auditable open-source infrastructure.

Umbrix does not treat a VPN tunnel as the entire privacy solution. Privacy is treated as a layered system encompassing routing, transport, DNS, application behavior, device identifiers, metadata, and network observability.

---

## Design Principles

### Privacy by Architecture

Privacy protections should be structural rather than dependent on users correctly configuring dozens of individual settings.

### Modular by Default

Major functionality is divided into independently maintainable modules with explicit interfaces and defined security boundaries.

### Core Stability

Security-critical functionality belongs in the core platform and should not depend on optional plugins.

### Optional Extensibility

Specialized capabilities can be added through plugins without unnecessarily increasing the attack surface of the base installation.

### Local First

Umbrix should support local and self-hosted operation wherever practical.

### Decentralized Infrastructure

The system should support distributed node discovery, routing, and reputation without requiring a single centralized control point.

### Human Control

Automatic routing and security decisions should remain configurable and understandable to users and administrators.

### Cryptographic Agility

Umbrix should be capable of adopting new cryptographic standards without requiring a complete architectural redesign.

### Cross-Platform Consistency

Privacy guarantees should remain as consistent as platform security models allow across Windows, Linux, macOS, Android, and iOS.

---

# Architecture

Umbrix is organized into four primary architectural layers:

1. **Core Platform**
2. **Network Nodes**
3. **Control Plane**
4. **Optional Plugin Ecosystem**

The core platform provides the functionality required to establish, secure, route, and terminate Umbrix connections.

Plugins provide additional functionality such as advanced traffic morphing, AI-assisted analysis, specialized transports, browser privacy controls, IoT integration, and experimental privacy technologies.

---

# Core Modules

## Core Client Module

The Client Module provides the primary user-facing networking layer.

Responsibilities include:

- Tunnel lifecycle management
- Local interface management
- Connection establishment
- Session management
- Privacy profile management
- Route selection requests
- Configuration management
- Platform integration
- Connection health monitoring
- Automatic reconnection
- Secure shutdown

The client should not expose raw private keys or sensitive routing material through ordinary user interfaces.

---

## Core Tunnel Module

The Tunnel Module manages the local encrypted network tunnel.

Responsibilities include:

- TUN/TAP integration
- Packet encapsulation
- Packet forwarding
- Tunnel state management
- MTU management
- Packet fragmentation handling
- Packet reassembly
- Connection isolation
- Leak prevention

The tunnel layer provides the foundation on which the routing and protocol modules operate.

---

## Core Protocol Module

The Protocol Module implements the Umbrix protocol architecture.

The protocol is designed to support:

- Secure session establishment
- Multiplexed traffic
- Ephemeral session keys
- Forward secrecy
- Routing envelopes
- Packet authentication
- Replay protection
- Protocol negotiation
- Version negotiation
- Cryptographic agility
- Transport abstraction

The protocol should be designed independently from any individual transport so that additional transports can be implemented without redesigning the core routing architecture.

---

## Core Cryptography Module

The Cryptography Module provides centralized cryptographic primitives and key-management interfaces.

Planned capabilities include:

- X25519 key exchange
- ChaCha20-Poly1305 authenticated encryption
- BLAKE3 hashing
- Secure random number generation
- Ephemeral session keys
- Per-hop key material
- Forward secrecy
- Key rotation
- Replay protection
- Secure key destruction
- Cryptographic algorithm negotiation
- Post-quantum hybrid key exchange support

Cryptographic implementations should rely on audited libraries whenever practical rather than implementing primitives from scratch.

---

## Core Routing Module

The Routing Module manages multi-node paths.

Capabilities include:

- Single-node routing
- Multi-node routing
- Configurable hop counts
- Entry-node selection
- Relay-node selection
- Exit-node selection
- Route health monitoring
- Route replacement
- Route failover
- Route expiration
- Route policy enforcement
- Latency-aware routing
- Reliability-aware routing
- Privacy-aware routing
- Randomized route selection

Routing decisions should minimize the information available to individual nodes about the complete path.

---

## Core Adaptive Routing Module

The Adaptive Routing Module continuously evaluates network conditions and determines whether an existing route remains appropriate.

It can consider:

- Latency
- Packet loss
- Node availability
- Congestion
- Route diversity
- Network reliability
- Privacy policy
- Transport health
- Node reputation

The module can initiate route replacement when configured thresholds are reached.

---

## Core Obfuscation Module

The Obfuscation Module provides foundational traffic transformation capabilities.

Capabilities include:

- Packet padding
- Packet-size normalization
- Timing variation
- Traffic batching
- Flow shaping
- Connection behavior normalization
- Transport camouflage
- Traffic-pattern diversification
- DPI resistance mechanisms

Obfuscation should be configurable so users can balance privacy, performance, battery consumption, and network compatibility.

---

## Core DNS Privacy Module

The DNS module protects domain-resolution traffic.

Capabilities include:

- Encrypted DNS
- DNS-over-HTTPS support
- DNS-over-QUIC support
- DNS leak prevention
- Configurable resolvers
- Per-profile resolver policies
- DNS routing through Umbrix nodes
- Resolver failover
- Local DNS interception
- DNS cache controls

---

## Core Kill Switch Module

The Kill Switch prevents traffic from bypassing the Umbrix tunnel.

Capabilities include:

- System-wide kill switch
- Application-specific kill switch
- Network-interface monitoring
- Route enforcement
- DNS leak prevention
- Connection-state enforcement
- Emergency traffic blocking

The kill switch should fail closed when enabled.

---

## Core Privacy Policy Module

The Privacy Policy Module provides centralized policy enforcement.

Policies may control:

- Required hop count
- Allowed regions
- Forbidden regions
- Node requirements
- Transport requirements
- DNS requirements
- Application routing
- Privacy level
- Obfuscation level
- Failover behavior
- Logging restrictions
- Plugin permissions

---

## Core Node Module

The Node Module allows systems to operate as Umbrix network nodes.

Node capabilities include:

- Entry relay operation
- Intermediate relay operation
- Exit relay operation
- Peer relay operation
- Node health reporting
- Capacity reporting
- Secure node identity
- Key management
- Route participation
- Node isolation

Operators should be able to configure exactly which node roles their infrastructure supports.

---

## Core Node Discovery Module

The Node Discovery Module provides decentralized discovery mechanisms.

Capabilities include:

- Distributed node discovery
- Capability advertisement
- Cryptographic node identity
- Node availability information
- Geographic metadata policies
- Transport capability discovery
- Node expiration
- Discovery cache management

Discovery data should avoid unnecessarily exposing sensitive operator information.

---

## Core Reputation Module

The Reputation Module evaluates node reliability and trust characteristics.

Metrics may include:

- Availability
- Reliability
- Latency
- Packet loss
- Protocol compliance
- Historical stability
- Abuse reports
- Cryptographic identity continuity
- Operator-defined trust policies

Reputation should influence routing without becoming an absolute centralized authority.

---

## Core Security Module

The Security Module provides system-wide defensive capabilities.

Capabilities include:

- Connection integrity monitoring
- MITM detection
- Replay detection
- Session anomaly detection
- Route integrity validation
- Node behavior validation
- Protocol downgrade protection
- Configuration integrity validation
- Secure update verification
- Security event handling

---

## Core Self-Healing Module

The Self-Healing Module provides automated recovery.

It can:

- Replace failed nodes
- Rebuild broken routes
- Re-establish tunnels
- Switch transports
- Rotate session keys
- Remove unhealthy nodes
- Recover from temporary network failures
- Restore required privacy policies

---

## Core Application Routing Module

The Application Routing Module supports application-specific network policies.

Capabilities include:

- Full-device tunneling
- Application-specific tunneling
- Split tunneling
- Application groups
- Per-application DNS policies
- Per-application routing policies
- Separate tunnels
- Application isolation

---

## Core Privacy Profile Module

Built-in profiles can include:

### Standard

Balanced privacy and performance.

### Advanced

Multi-node routing with stronger obfuscation and privacy controls.

### Maximum

Aggressive privacy controls, increased route diversity, and advanced traffic protection.

### Custom

User-defined policies controlling individual Umbrix capabilities.

Profiles should expose understandable security tradeoffs rather than presenting anonymity as an absolute guarantee.

---

## Core Telemetry Privacy Module

Umbrix should minimize unnecessary telemetry.

Capabilities include:

- Local-first diagnostics
- Opt-in metrics
- Metadata minimization
- Anonymous performance statistics
- Configurable diagnostic levels
- Local diagnostic storage
- Secure diagnostic deletion

User traffic contents should never be collected for ordinary telemetry.

---

# Optional Plugin Modules

Plugins extend Umbrix without requiring every installation to include every feature.

Plugins must operate through documented interfaces and explicit permissions.

## AI Threat Detection Plugin

Provides optional machine-learning-based detection of:

- Traffic anomalies
- Suspicious node behavior
- Connection manipulation
- Route anomalies
- Network attacks
- Potential traffic-analysis attempts

AI recommendations should remain subject to Umbrix policy controls.

---

## AI Obfuscation Plugin

Provides adaptive traffic-pattern selection based on:

- Network characteristics
- Connection performance
- Transport compatibility
- Configured privacy level

The plugin can recommend or activate approved obfuscation profiles.

---

## Traffic Morphing Plugin

Provides additional traffic-shaping strategies.

Potential capabilities include:

- Flow normalization
- Packet-size profiles
- Timing profiles
- Adaptive padding
- Cover traffic
- Protocol behavior simulation

---

## Advanced Stealth Transport Plugin

Provides additional transport implementations for networks that restrict or interfere with ordinary VPN traffic.

Transport implementations must preserve Umbrix authentication and encryption rather than bypassing them.

---

## Browser Privacy Plugin

Provides browser-level privacy controls such as:

- Fingerprint reduction
- WebRTC leak protection
- Browser DNS protection
- Geolocation permission controls
- Canvas privacy controls
- WebGL privacy controls
- User-agent policy management
- Tracking protection

Browser privacy features are inherently limited by browser security models and should not claim to eliminate fingerprinting completely.

---

## Geolocation Privacy Plugin

Provides optional application-level location privacy.

Capabilities may include:

- Location permission management
- Configurable location policies
- Privacy-preserving location responses
- Location consistency controls
- Optional location simulation

---

## Hardware Privacy Plugin

Provides supported platform-specific privacy controls for:

- Network identifiers
- Wi-Fi identifiers
- Bluetooth identifiers
- Device metadata
- Hardware telemetry

Capabilities depend on operating-system permissions and hardware support.

---

## IoT Privacy Plugin

Extends Umbrix protection to IoT environments.

Capabilities include:

- IoT subnet routing
- Device-specific tunnels
- Device isolation
- DNS protection
- Metadata minimization
- Policy-based routing
- Gateway deployment

---

## Secure AI Gateway Plugin

Provides an Umbrix privacy gateway for locally hosted AI systems.

Capabilities include:

- Model-server traffic protection
- AI API isolation
- Local inference network isolation
- Secure model-server communication
- Application-specific tunnels
- AI workload network policies
- Metadata minimization

The goal is to make network privacy a standard component of locally hosted AI infrastructure.

---

## Nested Tunnel Plugin

Provides optional layered tunnel architectures for deployments requiring additional routing separation.

---

## Peer Relay Plugin

Allows participating clients to act as temporary relay nodes.

Capabilities include:

- Ephemeral relays
- Peer discovery
- Relay authorization
- Relay expiration
- Capacity controls
- Privacy policies

---

## Decentralized Payment Plugin

Provides optional mechanisms for node operators and infrastructure providers to coordinate payments without requiring payment functionality in the Umbrix core.

---

## Network Simulation Plugin

Provides research and development capabilities for:

- Simulated network topologies
- Node behavior testing
- Routing experiments
- Traffic-pattern testing
- Performance benchmarking
- Failure simulation
- Protocol testing

---

## Geo Intelligence Plugin

Provides optional network intelligence for:

- Route recommendations
- Network availability
- Latency analysis
- Regional connectivity
- Node placement analysis
- Connectivity disruption detection

---

## Node Placement Plugin

Assists operators in determining suitable infrastructure locations based on:

- Network latency
- Regional diversity
- Reliability
- Capacity
- Route diversity
- Infrastructure availability

---

## Secure Application SDK Plugin

Provides developer-facing APIs for integrating Umbrix privacy capabilities into third-party applications.

Potential integrations include:

- Messaging
- VoIP
- AI applications
- Enterprise applications
- IoT software
- Privacy-focused browsers
- Developer tools

---

## Experimental Cryptography Plugin

Provides a controlled environment for evaluating new cryptographic algorithms and post-quantum mechanisms before potential inclusion in the core cryptographic architecture.

Experimental cryptography must never silently replace production cryptographic primitives.

---

# Client Architecture

The Umbrix client consists of:

- User interface
- Policy engine
- Tunnel manager
- Protocol engine
- Routing engine
- DNS privacy engine
- Kill switch
- Security monitor
- Plugin manager
- Platform integration layer

The platform integration layer provides operating-system-specific implementations while maintaining a common Umbrix security model.

---

# Node Architecture

An Umbrix node consists of:

- Node identity
- Protocol engine
- Cryptographic engine
- Routing engine
- Transport engine
- Relay engine
- Health monitor
- Reputation interface
- Policy engine
- Optional plugins

Node operators can deploy only the functionality required for their intended role.

---

# Control Plane

Umbrix uses a distributed control-plane architecture.

Control-plane responsibilities include:

- Node discovery
- Capability advertisement
- Route coordination
- Policy distribution
- Network health information
- Node reputation
- Version compatibility
- Key-management coordination

The control plane should be designed so that compromising a discovery service does not automatically compromise encrypted user traffic.

---

# Routing Architecture

Umbrix supports configurable multi-node routing.

A typical route can contain:

**Client → Entry Node → Relay Node → Exit Node → Destination**

Users may configure:

- Number of hops
- Geographic requirements
- Node requirements
- Performance requirements
- Route rotation
- Exit policies
- Relay diversity
- Privacy profile

Umbrix should avoid making absolute claims such as "untraceable" or "impossible to correlate." Traffic analysis remains an evolving field, and strong privacy requires continuous evaluation.

---

# Protocol Architecture

Umbrix uses a protocol architecture designed around separation of:

- Authentication
- Encryption
- Routing
- Transport
- Obfuscation
- Session management

The protocol should support multiple transports without coupling the security model to a single transport implementation.

Planned capabilities include:

- Ephemeral keys
- Forward secrecy
- Replay protection
- Session rotation
- Protocol negotiation
- Transport negotiation
- Packet authentication
- Routing envelopes
- Cryptographic agility
- Version compatibility

---

# Privacy Architecture

Umbrix treats privacy as multiple independent layers.

### Network Layer

Protects IP addresses, routing information, and network traffic.

### Transport Layer

Protects traffic characteristics and provides configurable obfuscation.

### DNS Layer

Protects domain-resolution activity.

### Application Layer

Provides application-specific routing and privacy policies.

### Browser Layer

Provides optional fingerprint and browser privacy controls.

### Device Layer

Provides supported hardware and telemetry privacy controls.

### Infrastructure Layer

Provides decentralized node discovery, routing, and operator controls.

---

# Security Architecture

Umbrix follows a defense-in-depth model.

Security mechanisms include:

- Authenticated encryption
- Forward secrecy
- Ephemeral keys
- Key rotation
- Replay protection
- Secure random generation
- Route integrity verification
- Node authentication
- Protocol downgrade protection
- Secure updates
- Kill switch enforcement
- Configuration validation
- Plugin isolation
- Security auditing

---

# Cryptography

The initial cryptographic architecture is intended to support:

- X25519
- ChaCha20-Poly1305
- BLAKE3
- Cryptographically secure randomness
- Ephemeral session keys
- Hybrid post-quantum key exchange

Cryptographic implementations should use well-maintained, independently reviewed libraries wherever possible.

Umbrix should maintain cryptographic agility so algorithms can be replaced as standards and security requirements evolve.

---

# Cross-Platform Support

Umbrix targets:

- Windows
- Linux
- macOS
- Android
- iOS

Optional integrations include:

- Browser extensions
- IoT gateways
- Self-hosted servers
- Cloud nodes
- Developer SDKs
- Locally hosted AI infrastructure

Platform-specific privacy capabilities will depend on the permissions and security architecture of each operating system.

---

# AI Privacy

Umbrix is designed to provide a privacy layer for locally hosted AI.

Locally hosted AI can reduce dependence on remote model providers, but local inference does not automatically protect:

- Network traffic
- DNS requests
- API connections
- Remote tools
- Model downloads
- Update services
- External data sources
- Application telemetry

Umbrix can provide a dedicated network privacy layer around locally hosted AI workloads through its core routing and security architecture and optional Secure AI Gateway Plugin.

The long-term objective is to make network privacy a standard architectural component of locally hosted AI rather than an afterthought.

---

# Developer Platform

Umbrix is designed for extensibility.

Developers can build plugins for:

- Routing
- Transport
- Obfuscation
- Privacy controls
- AI security
- Browser integration
- IoT networking
- Application integration
- Cryptographic experimentation
- Monitoring
- Research

Plugins should expose explicit capabilities and permissions and should not automatically receive unrestricted access to sensitive networking or cryptographic material.

---

# Plugin Security Model

Every plugin should declare:

- Plugin name
- Version
- Required Umbrix version
- Permissions
- Network access requirements
- Data access requirements
- Configuration requirements
- Security dependencies

Plugin permissions should be minimized according to the principle of least privilege.

Security-critical core functions must not be replaceable by untrusted plugins without explicit administrator approval.

---

# Configuration

Umbrix configuration should support:

- Privacy profiles
- Routing policies
- Node preferences
- Hop counts
- DNS policies
- Kill switch settings
- Application routing
- Transport preferences
- Obfuscation profiles
- Plugin configuration
- Update channels
- Diagnostic preferences

Configuration should be validated before activation and rejected when security requirements conflict.

---

# Deployment

Umbrix should support:

- Individual clients
- Self-hosted nodes
- Private organizational networks
- Distributed node networks
- Cloud deployments
- Hybrid deployments
- IoT gateways
- Locally hosted AI environments

Node operators should be able to independently configure infrastructure without requiring access to client traffic or private user credentials.

---

# Commercial-Grade Operations

Umbrix is designed to support production environments through:

- Stable and beta release channels
- Signed releases
- Automatic updates
- Health monitoring
- Node failover
- Route recovery
- Configuration validation
- Security advisories
- Audit-friendly architecture
- Deployment automation
- Optional metrics
- Version compatibility checks

---

# Testing and Verification

Umbrix development should include:

- Unit testing
- Integration testing
- Protocol testing
- Cross-platform testing
- Multi-node testing
- Failure testing
- Performance testing
- Privacy leak testing
- DNS leak testing
- Route integrity testing
- Cryptographic testing
- Fuzz testing
- Plugin isolation testing
- Security auditing

Privacy claims should be validated through measurable testing rather than assumed from architectural intent.

---

# Performance

Umbrix should provide configurable tradeoffs between:

- Privacy
- Latency
- Throughput
- Battery consumption
- CPU usage
- Route complexity
- Obfuscation strength

Users should be able to select appropriate profiles rather than forcing maximum overhead on every connection.

---

# Observability

Umbrix should provide privacy-preserving operational visibility.

Supported information may include:

- Connection status
- Tunnel health
- Node availability
- Latency
- Packet loss
- Route state
- Protocol state
- Resource usage

Sensitive user traffic contents should not be included in ordinary diagnostics.

---

# Emergency Controls

Umbrix should provide emergency controls capable of:

- Blocking network traffic
- Terminating active tunnels
- Removing ephemeral routing information
- Rotating session keys
- Disconnecting compromised nodes
- Disabling plugins
- Restoring safe configuration defaults

Emergency controls should prioritize preventing accidental traffic leakage.

---

# Roadmap

## Phase 1 — Foundation

- Core client
- Core node
- Tunnel implementation
- Cryptographic module
- Initial protocol
- Basic routing
- DNS protection
- Kill switch
- Configuration system

## Phase 2 — Multi-Node Network

- Multi-hop routing
- Node discovery
- Node reputation
- Route failover
- Adaptive routing
- Distributed control plane

## Phase 3 — Advanced Privacy

- Traffic obfuscation
- Flow shaping
- Fingerprint protection
- Application routing
- Privacy profiles
- Advanced security monitoring

## Phase 4 — Plugin Ecosystem

- Plugin API
- Plugin permissions
- AI threat detection
- Traffic morphing
- Browser privacy
- IoT support
- Secure AI Gateway
- Developer SDK

## Phase 5 — Research and Future Security

- Post-quantum cryptography
- Advanced network simulation
- Experimental transports
- Advanced privacy research
- Additional decentralized infrastructure

---

# Security Disclosure

Security vulnerabilities should be reported responsibly through the project's designated security-reporting process.

Do not publicly disclose an exploitable vulnerability before maintainers have had an opportunity to evaluate and address it.

---

# Contributions

Contributions are welcome across:

- Network engineering
- Systems programming
- Cryptography
- Security research
- Routing
- Obfuscation
- Cross-platform development
- AI security
- Browser privacy
- IoT networking
- Documentation
- Testing
- Infrastructure

See `CONTRIBUTING.md` for contribution requirements.

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
  - [https://roxanneardary.com/umbrix/](https://roxanneardary.com/umbrix/)

---

## License & Notice Requirements

Umbrix is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- Umbrix specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
