# GameCommons

**The universe of community-owned games.**

GameCommons is an open-source, federated multiplayer gaming platform specification that enables anyone to create, host, and connect community-owned game servers. Inspired by the decentralized architecture of federated platforms, GameCommons allows independent server operators to build thriving gaming communities while remaining discoverable and interoperable through an open federation protocol.

Designed as a modular platform rather than a single game server, GameCommons separates the core infrastructure from game-specific implementations. Every game is packaged as a module, allowing administrators to host one or many games on a single server while sharing common services such as authentication, federation, matchmaking, analytics, funding, and administration.

Released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**, GameCommons ensures that improvements made to network-deployed instances remain available to the community while enabling organizations to build sustainable multiplayer ecosystems without vendor lock-in.

---

# Vision

Create an open ecosystem where communities—not centralized corporations—own and operate the online worlds they play in.

GameCommons provides the infrastructure for:

- Community-owned game servers
- Federated multiplayer networks
- Self-hosted gaming communities
- Open game discovery
- Sustainable community funding
- Cross-server collaboration
- Open game development
- Long-term preservation of online games

---

# Design Goals

- Modular architecture
- Federation-first
- Local-first administration
- Privacy-first
- Community ownership
- Open standards
- Vendor neutrality
- Horizontal scalability
- High availability
- Security by design
- Accessibility
- Internationalization
- Sustainable funding
- Extensible plugin ecosystem

---

# Core Architecture

```
                    Federation Network

            GameCommons Instance
                    │
        ┌───────────┼────────────┐
        │           │            │
    Game Modules  Core Modules  Plugin Modules
```

Every server operates independently while participating in an optional federation of public or private GameCommons instances.

---

# Core Modules

## Federation Core

Provides the networking foundation for GameCommons.

### Features

- Instance federation
- Server discovery
- Federation synchronization
- Trust relationships
- Capability negotiation
- Cross-server communication
- Federation APIs
- Instance health monitoring

---

## Identity & Authentication

Unified authentication across hosted games.

### Features

- Local accounts
- Federated identities
- OAuth
- OpenID Connect
- LDAP
- Passkeys
- Multi-factor authentication
- Guest accounts
- Session management

---

## Server Registry

Maintains information about participating servers.

### Features

- Public server listings
- Private federation support
- Instance metadata
- Server capabilities
- Health status
- Discovery indexing

---

## Game Module Manager

Installs and manages individual game implementations.

### Features

- Module installation
- Dependency management
- Automatic updates
- Version compatibility
- Lifecycle management
- Capability registration

---

## Plugin Manager

Manages optional platform extensions.

### Features

- Plugin installation
- Plugin updates
- Digital signature verification
- Dependency resolution
- Version management

---

## Capability Engine

Allows modules to advertise supported functionality.

### Features

- Capability declarations
- Service discovery
- Compatibility validation
- Dynamic feature negotiation

---

## Event Bus & Service Mesh

The communication backbone of the platform.

### Features

- Publish/Subscribe messaging
- Event routing
- Service discovery
- Internal RPC
- Distributed workflows
- Message queues
- Event replay
- Federation event propagation
- Dead-letter queues
- Webhook integration
- Workflow orchestration
- Event auditing

---

## Matchmaking Core

Coordinates multiplayer sessions.

### Features

- Matchmaking
- Lobbies
- Queue management
- Session orchestration
- Cross-server matchmaking
- Invitations

---

## Networking Layer

Abstract networking infrastructure.

### Features

- TCP
- UDP
- QUIC
- WebSockets
- HTTP/HTTPS
- Custom transport providers

---

## Storage Layer

Unified storage abstraction.

### Features

- SQLite
- PostgreSQL
- MariaDB
- Object storage
- Flat files
- Database migrations

---

## API Gateway

Unified API access.

### Features

- REST
- GraphQL
- WebSockets
- gRPC
- API versioning
- Authentication

---

## Permissions & RBAC

Platform-wide authorization.

### Features

- Role management
- Permission policies
- Delegated administration
- Custom roles
- Access auditing

---

## Administration Dashboard

Centralized server management.

### Features

- Server management
- Module management
- User administration
- Logs
- Configuration
- Updates
- Diagnostics

---

## Monitoring & Telemetry

Operational monitoring.

### Features

- Metrics
- Health monitoring
- Logging
- Performance monitoring
- Alerts
- Audit logs

---

## Security Framework

Security services shared by every module.

### Features

- Secure communications
- Rate limiting
- Secrets management
- Certificate management
- Abuse prevention
- Audit logging

---

## Notification Framework

Platform-wide notification system.

### Features

- Email
- Push notifications
- In-app notifications
- Webhooks
- Event subscriptions

---

## Funding & Grants

Supports long-term community sustainability.

### Features

- Grant management
- Funding applications
- Milestone tracking
- Review workflows
- Community funding
- Bounties
- Treasury integration
- Financial reporting

---

## Treasury Management

Financial infrastructure.

### Features

- Budget management
- Revenue allocation
- Community funds
- Reserve funds
- Financial reporting
- Distribution APIs

---

## Rewards & Dividends

Community reward infrastructure.

### Features

- Reward pools
- Revenue sharing
- Player rewards
- Contributor incentives
- Reputation rewards
- Automated distributions
- Reward policies

---

## Federated Chat

Cross-server communication.

### Features

- Global chat
- Community channels
- Private messaging
- Presence
- Rich media
- Moderation
- Federation support

---

## Analytics Framework

Privacy-respecting analytics.

### Features

- Server analytics
- Community analytics
- Module analytics
- Financial analytics
- Dashboards
- Reporting
- Privacy-first metrics

---

## Translation & Localization

Internationalization platform.

### Features

- Multi-language support
- Runtime localization
- Community translations
- Translation management
- Internationalization APIs

---

## Web Portal

Public-facing platform.

### Features

- Community websites
- Server browser
- Public APIs
- Documentation
- Landing pages
- SEO support

---

## Configuration Management

Centralized configuration.

### Features

- Environment profiles
- Secret references
- Versioned configuration
- Configuration validation

---

## Scheduler & Automation

Background processing.

### Features

- Scheduled jobs
- Maintenance
- Event automation
- Workflow execution
- Background workers

---

## Asset Management

Shared asset infrastructure.

### Features

- Asset versioning
- CDN integration
- Game assets
- Static resources
- Content delivery

---

## Search & Indexing

Federated discovery services.

### Features

- Game search
- Server search
- Player search
- Federation indexing
- Full-text search

---

# Optional Plugin Modules

## Advertising & Sponsorship

- Community sponsorships
- Banner advertising
- Featured servers
- Campaign management
- Sponsor analytics

---

## Community Treasury Governance

- Budget proposals
- Voting
- Treasury transparency
- Community governance

---

## Donations

- One-time donations
- Memberships
- Fundraising campaigns
- Donation goals

---

## Marketplace

- Digital storefronts
- Cosmetic items
- Digital goods
- Marketplace commissions

---

## Tournament Manager

- Tournament brackets
- Registration
- Scheduling
- Prize management
- Federation tournaments

---

## Leaderboards & Rankings

- Elo ratings
- Seasonal rankings
- Cross-server leaderboards

---

## Friends & Social

- Friends
- Parties
- Activity feeds
- Social profiles

---

## Guilds & Communities

- Guilds
- Organizations
- Community management
- Shared resources

---

## Voice Communication

- Voice chat
- Positional audio
- Moderation
- Recording support

---

## Replay & Spectator

- Replay recording
- Spectator mode
- Broadcasting

---

## Streaming Integration

- Live streaming
- Broadcast overlays
- Streaming APIs

---

## Event Scheduler

- Community events
- Calendars
- Registration
- Automated announcements

---

## News & Announcements

- Community news
- Patch notes
- Featured content

---

## Mod Repository

- Mod publishing
- Version management
- Dependency resolution

---

## Asset Repository

- Shared assets
- Maps
- Texture packs
- Media libraries

---

## AI Moderation

- Spam detection
- Abuse detection
- Content moderation

---

## AI NPC Framework

- Intelligent NPCs
- Dialogue systems
- AI behaviors

---

## Anti-Cheat

- Cheat detection
- Behavioral analysis
- Appeals workflow

---

## Reputation System

- Trust scores
- Contributor reputation
- Moderation history

---

## Achievement System

- Achievements
- Badges
- Progress tracking

---

## Economy Framework

- Virtual currencies
- Trading
- Banking
- Crafting

---

## Inventory Framework

- Shared inventories
- Item storage
- Trading APIs

---

## Billing & Commerce

- Subscriptions
- Premium services
- Invoicing

---

## Backup & Disaster Recovery

- Automated backups
- Replication
- Restore management

---

## Federation Directory

- Regional directories
- Community directories
- Discovery hubs

---

## Developer SDK

- SDK generation
- Development tools
- Module templates

---

## Mobile Companion API

- Mobile synchronization
- Remote administration
- Push services

---

## Integration Bridges

- Discord
- Matrix
- IRC
- Slack
- Webhooks

---

## Federation Governance

- Federation councils
- Shared policies
- Inter-server voting

---

## Educational Tools

- Classrooms
- Training servers
- Learning environments

---

## Research Framework

- Research datasets
- Academic collaboration
- Experiment management

---

## Cross-Game Services

- Shared player profiles
- Universal achievements
- Cross-game identities
- Universal statistics

---

# Game Modules

Every supported game is implemented as an independent module.

Examples include:

- Chess
- Trading Card Games
- First-Person Shooters
- MMORPGs
- Survival Games
- Sandbox Games
- Strategy Games
- Racing Games
- Educational Games
- Board Games

Each module defines:

- Federation capabilities
- Networking requirements
- Matchmaking behavior
- Storage requirements
- Asset management
- Plugin compatibility
- World synchronization
- Mod support

---

# Federation

GameCommons allows independent communities to discover and connect with one another without requiring centralized ownership.

Federation supports:

- Public instances
- Private federations
- Community discovery
- Cross-server matchmaking
- Cross-server messaging
- Shared tournaments
- Shared funding initiatives
- Shared grant opportunities
- Shared player identities (optional)

---

# Sustainability

GameCommons is designed to support long-term community operation through optional funding mechanisms.

Communities may choose to enable:

- Sponsorships
- Advertising
- Donations
- Grant funding
- Revenue sharing
- Marketplace commissions
- Community rewards

Every funding model remains under the control of each individual server operator.

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
  - [https://roxanneardary.com/gamecommons/](https://roxanneardary.com/gamecommons/)  

---

## License & Notice Requirements

GameCommons is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:
  **Roxanne Ardary** and **https://www.roxanneardary.com/**.
- GameCommons specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
