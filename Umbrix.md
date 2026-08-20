# Umbrix
**Adaptive privacy for a connected world.**
- HTML Mirror:  [https://roxanneardary.com/umbrix-specification/](https://roxanneardary.com/umbrix-specification/)  
---

Umbrix is a commercial-grade, open-source privacy and network security platform designed to provide adaptive network obfuscation, multi-node routing, encrypted communications, application isolation, and per-agent network privacy across desktop, mobile, server, IoT, and locally hosted AI environments.

Umbrix is designed as a modular system. Core modules provide the foundational networking, cryptographic, routing, privacy, security, and multi-channel capabilities required by the platform. Optional plugin modules extend Umbrix with specialized functionality without requiring those capabilities to be installed or enabled.

A central design goal of Umbrix is to make network privacy available at the individual application and AI-agent level. Multiple AI agents can operate simultaneously while receiving independently managed Umbrix channels, routing policies, encryption sessions, DNS policies, privacy profiles, and network identities.

---

## Project Goals

Umbrix is designed to:

- Protect network traffic through authenticated encryption.
- Mask public IP addresses from destination services.
- Separate network origin from destination traffic.
- Support configurable multi-node routing.
- Provide adaptive network obfuscation.
- Reduce exposure to traffic analysis.
- Protect DNS and network metadata.
- Provide application-specific network isolation.
- Provide dedicated VPN channels for individual AI agents.
- Support independently managed privacy policies for every channel.
- Support locally hosted AI systems with network privacy by default.
- Support self-hosted and distributed infrastructure.
- Minimize unnecessary centralized dependencies.
- Provide cryptographic agility.
- Support desktop, mobile, server, IoT, and AI infrastructure.
- Provide a modular plugin ecosystem.
- Maintain transparent, auditable open-source architecture.

Umbrix treats privacy as a layered system rather than simply an encrypted tunnel. Network routing, transport behavior, DNS, applications, AI agents, device interfaces, metadata, and infrastructure are treated as separate privacy boundaries.

---

## Design Principles

### Privacy by Architecture

Privacy protections should be structural rather than dependent on users correctly configuring numerous individual settings.

### Modular Design

Core capabilities should be separated into independently maintainable modules with explicit interfaces and security boundaries.

### Core Security

Security-critical functionality belongs in the core platform and should not depend on optional plugins.

### Optional Extensibility

Specialized capabilities should be implemented as optional plugins when they are not required for the fundamental operation of Umbrix.

### Local First

Umbrix should support local and self-hosted operation wherever practical.

### Distributed Infrastructure

Umbrix should support distributed nodes, decentralized discovery, and distributed routing without requiring a single centralized authority.

### Agent Isolation

Every AI agent should be capable of receiving an independently managed network channel.

### Application Isolation

Applications should be able to receive independent routing, DNS, encryption, and privacy policies.

### Human Control

Automatic routing and security decisions should remain configurable and understandable.

### Cryptographic Agility

Umbrix should support replacement and addition of cryptographic mechanisms as standards evolve.

### Cross Platform

The architecture should maintain consistent privacy behavior across supported operating systems while respecting platform-specific security boundaries.

### Measurable Privacy

Privacy claims should be evaluated through testing and measurable security properties rather than assumed from architectural intent.

---

# Architecture

Umbrix consists of a modular privacy platform containing:

- Client services
- Tunnel management
- Protocol services
- Cryptographic services
- Routing services
- Node services
- Control-plane services
- Privacy policy services
- Multi-channel services
- Application isolation
- AI-agent isolation
- Security monitoring
- Optional plugins
- Developer APIs

Core modules provide foundational functionality.

Optional plugins extend the platform through defined interfaces and permission boundaries.

---

# Core Modules

## Core Client Module

The Client Module provides the primary local Umbrix service.

Capabilities include:

- Connection management
- Tunnel lifecycle management
- Privacy profile management
- Channel management
- Route selection
- Configuration management
- Platform integration
- Connection health monitoring
- Automatic reconnection
- Secure shutdown
- Policy enforcement
- Security state reporting

The client should not expose private cryptographic material through ordinary user interfaces.

---

## Core Tunnel Module

The Tunnel Module provides the local encrypted network interface.

Capabilities include:

- TUN/TAP integration
- Platform-specific virtual interfaces
- Packet encapsulation
- Packet forwarding
- Packet authentication
- Packet reassembly
- MTU management
- Connection isolation
- Traffic leak prevention
- Tunnel lifecycle management

The Tunnel Module provides the foundation for device-wide and channel-specific routing.

---

## Core Protocol Module

The Protocol Module provides the Umbrix protocol architecture.

Capabilities include:

- Secure session establishment
- Mutual authentication
- Session negotiation
- Multiplexed traffic
- Ephemeral session keys
- Forward secrecy
- Routing envelopes
- Packet authentication
- Replay protection
- Protocol version negotiation
- Transport negotiation
- Cryptographic negotiation
- Session expiration
- Session rotation

The protocol architecture should remain independent from individual network transports.

---

## Core Cryptography Module

The Cryptography Module provides cryptographic primitives and key-management services.

Capabilities include:

- X25519 key exchange
- ChaCha20-Poly1305 authenticated encryption
- BLAKE3 hashing
- Cryptographically secure random generation
- Ephemeral session keys
- Per-channel keys
- Per-hop keys
- Forward secrecy
- Key rotation
- Replay protection
- Secure key destruction
- Cryptographic agility
- Hybrid post-quantum key exchange support

Umbrix should use independently reviewed cryptographic libraries wherever practical.

---

## Core Routing Module

The Routing Module manages traffic paths through Umbrix infrastructure.

Capabilities include:

- Single-node routing
- Multi-node routing
- Configurable hop counts
- Entry-node selection
- Relay-node selection
- Exit-node selection
- Route health monitoring
- Route expiration
- Route rotation
- Route replacement
- Route failover
- Privacy-aware routing
- Performance-aware routing
- Reliability-aware routing
- Route diversity
- Policy-based routing

Routing should minimize unnecessary knowledge of the complete path at individual nodes.

---

## Core Adaptive Routing Module

The Adaptive Routing Module evaluates network conditions and determines whether routes remain appropriate.

It may consider:

- Latency
- Packet loss
- Node availability
- Congestion
- Reliability
- Route diversity
- Transport health
- Privacy requirements
- Node reputation
- Configured user policies

The module can replace routes when configured thresholds or privacy requirements are no longer satisfied.

---

## Core Obfuscation Module

The Obfuscation Module provides foundational traffic transformation.

Capabilities include:

- Packet padding
- Packet-size normalization
- Timing variation
- Traffic batching
- Flow shaping
- Connection behavior normalization
- Traffic-pattern diversification
- Transport camouflage
- DPI resistance mechanisms
- Configurable obfuscation levels

Obfuscation profiles should provide configurable tradeoffs between privacy, performance, latency, and resource consumption.

---

## Core DNS Privacy Module

The DNS Privacy Module protects domain resolution.

Capabilities include:

- Encrypted DNS
- DNS over HTTPS
- DNS over QUIC
- DNS leak prevention
- Configurable resolvers
- Per-profile DNS policies
- Per-channel DNS policies
- DNS routing through Umbrix nodes
- Resolver failover
- Local DNS interception
- DNS cache controls

---

## Core Kill Switch Module

The Kill Switch Module prevents traffic from bypassing Umbrix.

Capabilities include:

- Device-wide kill switch
- Application-specific kill switch
- AI-agent-specific kill switch
- Channel-specific kill switch
- Interface monitoring
- Route enforcement
- DNS leak prevention
- Emergency traffic blocking
- Fail-closed behavior

When enabled, the kill switch should prevent traffic from escaping outside the configured Umbrix privacy boundary.

---

## Core Privacy Policy Module

The Privacy Policy Module provides centralized policy enforcement.

Policies may control:

- Required hop count
- Allowed regions
- Restricted regions
- Node requirements
- Transport requirements
- DNS requirements
- Application routing
- AI-agent routing
- Privacy level
- Obfuscation level
- Failover behavior
- Logging restrictions
- Plugin permissions
- Channel permissions
- Bandwidth limits
- Connection destinations

---

## Core Privacy Profile Module

Umbrix should provide configurable privacy profiles.

### Standard

Balanced privacy, performance, and resource consumption.

### Advanced

Multi-node routing with increased obfuscation and stronger privacy controls.

### Maximum

Aggressive privacy controls, increased route diversity, and stronger traffic protection.

### AI Agent

Dedicated privacy settings optimized for individual AI-agent channels.

### Custom

Fully user-defined privacy policies.

Profiles should communicate their security and performance tradeoffs clearly.

---

## Core MultiChannel Module

The MultiChannel Module provides independent Umbrix network channels for applications, services, and AI agents.

Each channel represents an independent logical privacy boundary.

Capabilities include:

- Per-application VPN channels
- Per-agent VPN channels
- Independent encryption sessions
- Independent routing policies
- Independent DNS policies
- Independent privacy profiles
- Independent obfuscation profiles
- Independent kill switches
- Independent exit-node policies
- Independent bandwidth policies
- Independent security policies
- Independent channel lifecycle
- Channel health monitoring
- Channel failover
- Channel suspension
- Channel revocation
- Channel destruction
- Channel quotas
- Channel priority
- Channel authorization
- Dynamic channel creation
- Dynamic channel termination

A channel should be capable of operating independently from other channels on the same device.

---

## Core AI Agent Channel Module

The AI Agent Channel Module extends MultiChannel functionality specifically for AI agents.

Each AI agent can receive a dedicated Umbrix channel.

An AI agent channel can include:

- Dedicated network identity
- Dedicated session keys
- Dedicated route
- Dedicated entry node
- Dedicated relay nodes
- Dedicated exit node
- Dedicated DNS policy
- Dedicated privacy profile
- Dedicated obfuscation policy
- Dedicated kill switch
- Dedicated bandwidth limit
- Dedicated destination policy
- Dedicated security policy
- Dedicated plugin permissions
- Dedicated channel lifecycle
- Dedicated health state

Multiple AI agents can operate simultaneously without requiring them to share the same routing or privacy configuration.

---

## Core Agent Lifecycle Module

The Agent Lifecycle Module manages network privacy throughout the life of an AI agent.

Supported lifecycle states include:

- Agent registration
- Channel creation
- Policy assignment
- Route establishment
- Agent startup
- Active monitoring
- Route rotation
- Policy updates
- Channel suspension
- Agent termination
- Channel destruction
- Ephemeral key destruction

When an agent terminates, its channel and ephemeral session material should be securely disposed of according to configured policy.

---

## Core Agent Authorization Module

The Agent Authorization Module controls which applications and AI agents may access specific Umbrix channels.

Capabilities include:

- Agent identity registration
- Application identity registration
- Channel ownership
- Channel access control
- Permission management
- Token-based authorization
- Local authorization
- Channel revocation
- Permission expiration
- Policy inheritance controls

An AI agent should not automatically gain access to another agent's channel.

---

## Core Agent API Module

The Agent API provides local interfaces for AI orchestration systems and application frameworks.

Capabilities include:

- Create channel
- Assign channel
- Query channel
- Update channel policy
- Request route
- Rotate route
- Suspend channel
- Resume channel
- Revoke channel
- Destroy channel
- Query health
- Query connection state
- Apply privacy profile
- Apply DNS policy
- Apply destination policy

The API should authenticate requests and enforce channel-specific authorization.

---

## Core Agent SDK Module

The Agent SDK provides developers with interfaces for integrating Umbrix into AI applications.

Potential integrations include:

- Locally hosted AI
- AI agent frameworks
- Agent orchestration systems
- Autonomous applications
- AI development environments
- Model servers
- Tool-using agents
- Workflow engines

The SDK should abstract channel lifecycle operations without exposing unnecessary cryptographic material.

---

## Core Application Routing Module

The Application Routing Module provides network policies for individual applications.

Capabilities include:

- Full-device routing
- Application-specific routing
- Split tunneling
- Application groups
- Per-application DNS
- Per-application exit policies
- Per-application privacy profiles
- Application-specific kill switches
- Application-specific channel assignment

---

## Core Node Module

The Node Module allows infrastructure to participate in the Umbrix network.

Supported node roles include:

- Entry node
- Relay node
- Exit node
- Peer relay
- Private relay
- Organization-controlled node

Node capabilities include:

- Secure node identity
- Key management
- Route participation
- Health reporting
- Capacity reporting
- Policy enforcement
- Node isolation
- Secure configuration

---

## Core Node Discovery Module

The Node Discovery Module provides decentralized infrastructure discovery.

Capabilities include:

- Distributed node discovery
- Node capability advertisement
- Cryptographic node identity
- Transport capability discovery
- Node availability
- Node expiration
- Discovery caching
- Privacy-preserving node metadata
- Regional diversity information

---

## Core Reputation Module

The Reputation Module evaluates node reliability and trust characteristics.

Potential inputs include:

- Availability
- Reliability
- Latency
- Packet loss
- Protocol compliance
- Historical stability
- Security reports
- Identity continuity
- Operator policies

Reputation should inform routing without becoming an absolute centralized authority.

---

## Core Security Module

The Security Module provides system-wide defensive capabilities.

Capabilities include:

- Session integrity monitoring
- MITM detection
- Replay detection
- Route integrity validation
- Node behavior validation
- Protocol downgrade protection
- Configuration validation
- Security event detection
- Secure update verification
- Plugin security enforcement
- Channel security monitoring
- Agent security monitoring

---

## Core Self-Healing Module

The Self-Healing Module provides automatic network recovery.

Capabilities include:

- Failed-node replacement
- Broken-route recovery
- Tunnel reconnection
- Transport switching
- Session key rotation
- Unhealthy-node removal
- Channel recovery
- Agent-channel recovery
- Network failure recovery
- Policy restoration

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

User traffic contents should not be collected as ordinary telemetry.

---

## Core Configuration Module

The Configuration Module manages system, channel, agent, node, routing, security, and plugin configuration.

Capabilities include:

- Configuration validation
- Policy validation
- Profile management
- Configuration versioning
- Secure configuration storage
- Configuration import
- Configuration export
- Configuration rollback
- Conflict detection

---

# Optional Plugin Modules

Optional plugins extend Umbrix without requiring specialized functionality in the core installation.

Plugins must use documented interfaces and explicit permission models.

---

## AI Threat Detection Plugin

Provides optional AI-assisted detection of:

- Traffic anomalies
- Suspicious node behavior
- Route anomalies
- Connection manipulation
- Network attacks
- Potential traffic-analysis patterns
- Unexpected agent behavior

AI recommendations should remain subject to Umbrix security policies.

---

## AI Obfuscation Plugin

Provides adaptive selection of approved traffic-obfuscation strategies based on:

- Network characteristics
- Transport compatibility
- Connection performance
- Privacy requirements
- Configured policy

---

## Traffic Morphing Plugin

Provides additional traffic transformation capabilities.

Potential capabilities include:

- Flow normalization
- Packet-size profiles
- Timing profiles
- Adaptive padding
- Cover traffic
- Traffic-pattern variation
- Transport behavior simulation

---

## Advanced Stealth Transport Plugin

Provides additional transport implementations for environments where conventional VPN traffic experiences interference.

All transports must preserve Umbrix authentication and encryption.

---

## Browser Privacy Plugin

Provides browser-level privacy controls.

Capabilities may include:

- Fingerprint reduction
- WebRTC leak protection
- Browser DNS protection
- Geolocation permission controls
- Canvas privacy controls
- WebGL privacy controls
- User-agent policies
- Tracking protection

Browser-level protections should clearly communicate platform limitations.

---

## Geolocation Privacy Plugin

Provides optional application-level location privacy controls.

Capabilities may include:

- Location permission policies
- Configurable location behavior
- Location consistency controls
- Privacy-preserving location responses
- Optional location simulation

---

## Hardware Privacy Plugin

Provides supported platform-specific privacy controls for:

- Network identifiers
- Wi-Fi identifiers
- Bluetooth identifiers
- Device metadata
- Hardware telemetry

Capabilities depend on operating-system permissions.

---

## IoT Privacy Plugin

Extends Umbrix to IoT environments.

Capabilities include:

- IoT subnet routing
- Device-specific tunnels
- Device isolation
- DNS protection
- Metadata minimization
- Device policies
- Gateway deployment

---

## Secure AI Gateway Plugin

Provides a dedicated Umbrix privacy gateway for locally hosted AI infrastructure.

Capabilities include:

- Model-server traffic protection
- AI API isolation
- Local inference isolation
- Model-server communication protection
- AI application-specific tunnels
- AI workload network policies
- Metadata minimization
- Agent channel provisioning

---

## Agent Orchestration Plugin

Integrates Umbrix with external AI orchestration systems.

Capabilities may include:

- Automatic agent registration
- Automatic channel creation
- Agent-to-channel assignment
- Dynamic policy assignment
- Agent shutdown detection
- Channel cleanup
- Channel health integration
- Agent fleet management

---

## Container Network Plugin

Provides network isolation for containerized AI agents and applications.

Capabilities include:

- Container-specific channels
- Namespace-aware routing
- Per-container DNS
- Container kill switches
- Container-specific exit policies
- Container channel lifecycle
- Container network isolation

---

## Virtual Machine Network Plugin

Provides independent Umbrix channels for virtual machines.

Capabilities include:

- VM-specific channels
- VM routing policies
- VM DNS policies
- VM kill switches
- VM-specific privacy profiles
- VM channel lifecycle management

---

## Nested Tunnel Plugin

Provides optional layered tunnel architectures for deployments requiring additional routing separation.

---

## Peer Relay Plugin

Allows authorized clients to operate as temporary relay nodes.

Capabilities include:

- Ephemeral relays
- Peer discovery
- Relay authorization
- Relay expiration
- Capacity controls
- Relay privacy policies

---

## Decentralized Payment Plugin

Provides optional infrastructure for node operators and service providers to coordinate payments without placing payment functionality in the Umbrix core.

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
- Latency analysis
- Regional connectivity
- Node availability
- Connectivity disruption detection
- Infrastructure analysis

---

## Node Placement Plugin

Assists infrastructure operators with node placement analysis based on:

- Network latency
- Regional diversity
- Reliability
- Capacity
- Route diversity
- Infrastructure availability

---

## Secure Application SDK Plugin

Provides APIs for integrating Umbrix privacy capabilities into third-party applications.

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

Provides a controlled environment for evaluating emerging cryptographic algorithms and post-quantum mechanisms.

Experimental algorithms must not silently replace production cryptographic mechanisms.

---

# Multi-Agent Privacy Architecture

Umbrix should support an environment where multiple AI agents operate simultaneously while maintaining independent network privacy boundaries.

A deployment may contain:

- Agent A with a two-hop route
- Agent B with a three-hop route
- Agent C with a dedicated exit policy
- Agent D with restricted destination access
- Agent E with maximum obfuscation

Each agent can maintain independent:

- Channels
- Keys
- Routes
- DNS policies
- Privacy profiles
- Kill switches
- Security policies
- Bandwidth limits
- Plugin permissions
- Destination policies

The system should prevent accidental channel sharing unless explicitly authorized.

---

# AI Agent Channel Isolation

Each AI agent should be treated as an independently addressable network workload.

A channel should provide:

- Network isolation
- Cryptographic isolation
- Routing isolation
- DNS isolation
- Policy isolation
- Security isolation
- Lifecycle isolation

The channel architecture should support local AI systems running multiple simultaneous agents without requiring all agents to share one VPN identity or route.

---

# AI Agent Network Lifecycle

A typical AI agent lifecycle should support:

**Register → Authenticate → Create Channel → Assign Policy → Establish Route → Start Agent → Monitor → Rotate Route → Update Policy → Terminate Agent → Destroy Channel**

Channel destruction should invalidate the associated session and dispose of ephemeral cryptographic material according to configured security policy.

---

# Control Plane

The Umbrix control plane manages distributed network coordination.

Capabilities include:

- Node discovery
- Node capability advertisement
- Route coordination
- Policy distribution
- Network health information
- Node reputation
- Version compatibility
- Channel coordination
- Agent channel management
- Key-management coordination

Compromise of a discovery or coordination component should not automatically expose encrypted user traffic.

---

# Routing Architecture

Umbrix supports configurable multi-node paths.

A typical route may consist of:

**Client or Agent → Entry Node → Relay Node → Exit Node → Destination**

Routing can be independently configured for each device, application, container, virtual machine, or AI agent.

Users may configure:

- Hop count
- Geographic requirements
- Node requirements
- Performance requirements
- Route rotation
- Exit policies
- Relay diversity
- Privacy profiles
- Agent-specific policies

Umbrix should not claim absolute anonymity or guarantee that traffic analysis is impossible.

---

# Protocol Architecture

Umbrix uses a protocol architecture that separates:

- Authentication
- Encryption
- Routing
- Transport
- Obfuscation
- Session management
- Channel management

The protocol should support multiple transports without coupling the security model to one transport.

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
- Channel-specific sessions
- Agent-specific sessions
- Version compatibility

---

# Privacy Architecture

Umbrix treats privacy as multiple independent layers.

### Network Layer

Protects IP addresses, routing information, and network traffic.

### Transport Layer

Provides encrypted communication and configurable traffic obfuscation.

### DNS Layer

Protects domain-resolution activity.

### Application Layer

Provides application-specific routing and privacy policies.

### AI Agent Layer

Provides dedicated network channels and privacy boundaries for individual AI agents.

### Browser Layer

Provides optional browser fingerprint and privacy controls.

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
- Channel isolation
- Agent isolation
- Security auditing

---

# Cryptography

The initial cryptographic architecture should support:

- X25519
- ChaCha20-Poly1305
- BLAKE3
- Cryptographically secure randomness
- Ephemeral session keys
- Per-channel keys
- Per-hop keys
- Forward secrecy
- Hybrid post-quantum key exchange

Umbrix should maintain cryptographic agility so algorithms can evolve without requiring a complete architectural redesign.

---

# Cross Platform Support

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
- Container environments
- Virtual machines
- Locally hosted AI systems
- AI orchestration systems

Platform-specific capabilities depend on operating-system permissions and security models.

---

# AI Privacy

Umbrix is designed to provide a privacy layer for locally hosted AI.

Running an AI model locally does not automatically protect:

- Network traffic
- DNS requests
- API connections
- Remote tools
- Model downloads
- Update services
- External data sources
- Application telemetry
- Agent-to-agent communications

Umbrix should allow each AI agent to receive its own network channel so that local AI deployments can establish independent privacy boundaries for every running agent.

The long-term objective is to make network privacy a standard component of locally hosted AI infrastructure.

---

# Developer Platform

Umbrix is designed for extensibility.

Developers can build integrations for:

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
- Agent orchestration
- AI development frameworks

Plugins should expose explicit capabilities and permissions.

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

Plugin permissions should follow least-privilege principles.

Security-critical core functionality must not be replaceable by untrusted plugins without explicit administrator approval.

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
- AI-agent routing
- Transport preferences
- Obfuscation profiles
- Channel policies
- Agent policies
- Plugin configuration
- Update channels
- Diagnostic preferences

Configuration should be validated before activation.

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
- Containerized deployments
- Virtual machines
- Locally hosted AI environments
- AI agent environments

Node operators should be able to configure infrastructure independently without requiring access to user traffic or private client credentials.

---

# Commercial Grade Operations

Umbrix should support production deployments through:

- Stable releases
- Beta releases
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
- Channel health monitoring
- Agent fleet management

---

# Testing and Verification

Umbrix development should include:

- Unit testing
- Integration testing
- Protocol testing
- Cross-platform testing
- Multi-node testing
- Multi-channel testing
- Multi-agent testing
- Failure testing
- Performance testing
- Privacy leak testing
- DNS leak testing
- Route integrity testing
- Cryptographic testing
- Fuzz testing
- Plugin isolation testing
- Channel isolation testing
- Agent isolation testing
- Security auditing

Privacy claims should be validated through measurable testing.

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
- Number of channels
- Number of active AI agents

Users should be able to select appropriate profiles rather than forcing maximum overhead on every connection.

---

# Observability

Umbrix should provide privacy-preserving operational visibility.

Supported information may include:

- Connection status
- Tunnel health
- Channel health
- Agent channel status
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
- Terminating individual channels
- Terminating individual agent channels
- Removing ephemeral routing information
- Rotating session keys
- Disconnecting compromised nodes
- Disabling plugins
- Revoking agent permissions
- Restoring safe configuration defaults

Emergency controls should prioritize preventing accidental traffic leakage.

---

# Security Disclosure

Security vulnerabilities should be reported responsibly through the project's designated security-reporting process.

Security researchers should avoid publicly disclosing exploitable vulnerabilities before maintainers have had an opportunity to evaluate and address them.

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
- Umbrix specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
