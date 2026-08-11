# TransitMemory

**The Open Source Core for Custom Transportation Systems.**

TransitMemory is an open source specification for building modular transportation management systems for schools, transportation companies, childcare organizations, universities, businesses, nonprofits, camps, senior transportation, community transportation, and other organizations.

TransitMemory provides a standardized Core for transportation routing, rider scheduling, stop management, driver operations, route intelligence, ETA calculation, traffic awareness, route optimization, institutional transportation memory, and organization-built extensions.

Organizations can build their own modules on top of the Core without modifying the Core specification. Optional plugins provide integrations and capabilities such as real-time vehicle tracking, GPS hardware, traffic data providers, mapping services, communications, weather data, telematics, and AI services.

TransitMemory is designed to support local-first operation, modular deployment, interoperability, vendor independence, and organization-controlled transportation systems.

## Core Principles

### Modular Architecture

TransitMemory separates the transportation Core from organization-specific modules and optional plugins.

The Core defines standardized:

- Data models
- APIs
- Events
- Permissions
- Transportation workflows
- Extension points
- Safety constraints
- Interoperability requirements

Organizations can build their own modules using these interfaces without modifying the Core.

### Organization Independence

Organizations control their own transportation workflows, policies, branding, customer communication, and operational modules.

An organization can build modules for:

- Schools
- School districts
- Private schools
- Daycare providers
- Universities
- Corporate transportation
- Employee shuttles
- Camps
- Senior transportation
- Community transportation
- Nonprofits
- Healthcare transportation
- Residential transportation
- Charter transportation
- Specialized transportation

### Plugin Independence

External services are not required to be part of the Core.

Plugins can connect TransitMemory to:

- GPS systems
- Fleet tracking systems
- Mapping providers
- Traffic providers
- Weather services
- SMS providers
- Email providers
- Push notification services
- Telematics systems
- Student information systems
- Artificial intelligence services
- Other external systems

The Core remains independent of any specific vendor or service provider.

### Safety First

Transportation safety requirements take precedence over optimization and efficiency.

The system must not recommend a route that violates known:

- Safety restrictions
- Legal restrictions
- Vehicle restrictions
- Road restrictions
- Accessibility requirements
- Organization-defined transportation requirements

## Core Modules

### Route Management Module

The Route Management Module defines the fundamental route structure.

Features include:

- Create and manage routes
- Create recurring routes
- Create one-time routes
- Define route sequences
- Define stop order
- Assign drivers
- Assign vehicles
- Create route variants
- Create temporary route modifications
- Activate or deactivate stops for individual trips
- Duplicate routes
- Version routes
- Maintain historical route configurations
- Compare planned and completed routes
- Support morning routes
- Support afternoon routes
- Support evening routes
- Support special-purpose routes

### Stop Management Module

The Stop Management Module manages transportation stops and their operational requirements.

Features include:

- Permanent stops
- Temporary stops
- Rider assignments
- Arrival windows
- Departure windows
- Stop-specific instructions
- Accessibility requirements
- Loading information
- Unloading information
- Safe stopping locations
- Stop hazards
- Stop performance history
- Stop delay analysis
- Stop operational notes

### Rider Management Module

The Rider Management Module manages people assigned to transportation services.

Features include:

- Rider records
- Transportation assignments
- Authorized stops
- Recurring transportation schedules
- Temporary transportation changes
- Daily rider status
- Organization-defined rider fields
- Rider transportation requirements
- Role-based access to rider information

The Core should support organization-specific extensions without requiring organizations to modify the Core rider data model.

### Daily Stop Skip Module

The Daily Stop Skip Module allows authorized parents, guardians, customers, or riders to notify the organization that transportation is not required for a particular trip.

Features include:

- Skip a stop for a specific day
- Skip morning transportation
- Skip afternoon transportation
- Skip both directions
- Cancel a previous request
- Define request deadlines
- Confirm requests
- Track request status
- Notify drivers
- Notify dispatchers
- Update the active daily route
- Preserve the permanent rider assignment

A daily stop skip changes the active trip without permanently modifying the rider's transportation assignment.

### Driver Operations Module

The Driver Operations Module provides the operational interface for drivers.

Features include:

- Driver route assignments
- Current route information
- Active stops
- Authorized rider information
- Stop instructions
- Route status
- Driver notes
- Road observations
- Road problem reporting
- Unsafe turn reporting
- Difficult loading location reporting
- Temporary condition reporting
- Route recommendations
- Driver route overrides
- Driver decision records

### Driver Road Knowledge Module

The Driver Road Knowledge Module allows drivers to contribute transportation knowledge that can be reused by the organization.

Drivers can report:

- Tight turns
- Unsafe turns
- Directional restrictions
- Difficult intersections
- Low-clearance locations
- Weight restrictions
- Narrow roads
- Difficult turnaround locations
- Construction
- Recurring congestion
- Flooding
- Poor visibility
- Unsafe stopping locations
- Vehicle-specific road problems

Each road observation can include:

- Location
- Direction
- Reason
- Vehicle type
- Severity
- Date reported
- Source
- Verification status
- Expiration date
- Temporary or permanent status

Driver observations become reusable transportation knowledge rather than isolated notes.

### Vehicle Management Module

The Vehicle Management Module maintains vehicle information used by routing and operations.

Features include:

- Vehicle records
- Vehicle assignments
- Vehicle dimensions
- Vehicle height
- Vehicle width
- Vehicle length
- Vehicle weight
- Passenger capacity
- Accessibility capabilities
- Turning characteristics
- Vehicle restrictions
- Replacement vehicle assignments
- Vehicle classes

### Vehicle-Aware Routing Module

The Vehicle-Aware Routing Module ensures routes account for the physical characteristics of assigned vehicles.

Features include:

- Vehicle dimensions
- Turning radius
- Road width
- Clearance restrictions
- Weight restrictions
- Height restrictions
- Vehicle capacity
- Accessibility requirements
- Vehicle-specific road restrictions
- Organization-defined vehicle constraints

Routing recommendations must not violate known vehicle restrictions.

### ETA and Traffic Intelligence Module

The ETA and Traffic Intelligence Module is a Core module.

It provides standardized ETA calculations while remaining independent of any particular traffic or mapping provider.

Features include:

- Route-level ETA
- Stop-level ETA
- Destination ETA
- Continuous ETA recalculation
- Historical travel times
- Current traffic conditions
- Recurring traffic patterns
- Time-of-day traffic patterns
- Day-of-week traffic patterns
- School-zone congestion
- Construction impacts
- Road closure impacts
- Traffic incident impacts
- Route changes
- Stop completion
- Stop dwell time
- Delay prediction
- ETA confidence
- ETA accuracy measurement

Traffic data can be supplied by optional traffic plugins.

The Core defines the interface for receiving traffic information without requiring a specific provider.

### Time Optimization Module

The Time Optimization Module analyzes transportation history and recommends improvements.

Features include:

- Historical route duration analysis
- Historical stop duration analysis
- Travel time analysis
- Stop sequence analysis
- Schedule analysis
- Delay analysis
- Route efficiency analysis
- Alternative stop ordering
- Schedule recommendations
- Recurring delay identification
- Route segment analysis
- Projected time savings
- Planned-versus-actual comparison

Optimization recommendations must explain the reasoning behind the recommendation.

### Route Optimization Module

The Route Optimization Module evaluates possible route configurations while respecting Core safety and operational constraints.

Features include:

- Stop ordering
- Route sequencing
- Vehicle assignment considerations
- Travel-time optimization
- Route distance optimization
- Capacity considerations
- Rider requirements
- Vehicle restrictions
- Road restrictions
- Time windows
- Organization-defined constraints
- Alternative route analysis
- Optimization recommendations

Optimization must prioritize:

1. Safety
2. Legal and regulatory constraints
3. Vehicle constraints
4. Rider requirements
5. Organization requirements
6. Schedule requirements
7. Efficiency

### Route Recommendation Module

The Route Recommendation Module provides human-reviewable recommendations rather than silently changing established routes.

Features include:

- Recommendation generation
- Reasoning
- Estimated time savings
- Affected stops
- Affected riders
- Affected vehicles
- Constraints considered
- Accept recommendation
- Reject recommendation
- Modify recommendation
- Record decision
- Record reason for rejection
- Learn from repeated overrides

### Route Records Module

The Route Records Module maintains the operational history of transportation trips.

Features include:

- Daily trip records
- Planned route
- Actual route
- Driver
- Vehicle
- Scheduled stops
- Completed stops
- Skipped stops
- Route deviations
- Delays
- Distance
- Duration
- Stop dwell times
- Driver observations
- Operational events
- Route changes
- Optimization decisions

### Institutional Transportation Memory Module

TransitMemory uses historical transportation information as organizational knowledge.

The Institutional Transportation Memory Module preserves:

- Driver observations
- Route history
- Stop history
- Road restrictions
- Historical travel times
- Historical delays
- ETA accuracy
- Route deviations
- Optimization decisions
- Driver overrides
- Planned-versus-actual performance

The purpose is to prevent organizations from repeatedly rediscovering the same transportation problems.

### Safety and Constraints Module

The Safety and Constraints Module defines the rules that routing and optimization systems must respect.

It supports:

- Permanent restrictions
- Temporary restrictions
- Vehicle-specific restrictions
- Directional restrictions
- Time-specific restrictions
- Organization restrictions
- School-specific restrictions
- Stop-specific restrictions
- Rider-specific transportation requirements
- Accessibility requirements
- Constraint priorities
- Constraint history
- Constraint expiration

### Notification Events Module

The Core defines standardized transportation events that can be consumed by communication modules and plugins.

Events may include:

- Route created
- Route updated
- Route started
- Route completed
- Stop approaching
- Stop arrived
- Stop departed
- Rider cancellation requested
- Rider cancellation approved
- Rider cancellation cancelled
- Delay detected
- ETA updated
- Route deviation detected
- Driver observation created
- Road restriction created
- Vehicle assigned
- Vehicle changed
- Transportation alert created

### Module Framework

The Module Framework provides the interfaces organizations and developers use to extend TransitMemory.

Features include:

- Core APIs
- Data models
- Events
- Permissions
- Extension points
- Module manifests
- Module versioning
- Module compatibility
- Module dependencies
- Module installation
- Module updates
- Module removal
- Organization-specific data extensions
- Organization-specific workflows
- Organization-specific business rules

Organization modules must not require modification of TransitMemory Core source code.

### Organization Module Framework

Organizations can build custom modules on top of the Core.

Organization modules can provide:

- Organization-specific workflows
- Custom transportation policies
- Custom rider workflows
- Custom scheduling
- Custom reporting
- Custom analytics
- Custom administration
- Custom communication
- Custom customer experiences
- Custom transportation rules
- Custom data fields

Organizations maintain control over their own modules while using standardized Core interfaces.

### Organization Communication Module

Organizations can create customized communication modules for parents, guardians, customers, riders, employees, or other authorized users.

Features include:

- Organization branding
- Organization name
- Organization logo
- Organization colors
- Organization terminology
- Custom workflows
- Custom notifications
- Transportation information
- Route information
- Stop information
- ETA information
- Daily transportation cancellation
- Transportation status
- Service announcements
- Emergency notifications
- Organization contact information

Communication modules may be distributed as:

- Mobile applications
- Web applications
- Progressive Web Apps
- Embedded web modules
- Other organization-defined interfaces

### Permission Module

The Permission Module defines access to Core capabilities.

Permissions can include:

- Routes
- Stops
- Riders
- Drivers
- Vehicles
- GPS
- ETA
- Historical records
- Notifications
- Analytics
- Administration
- Organization modules
- Plugins

Organizations can define additional permissions through modules.

### Audit Module

The Audit Module records important system activity.

Features include:

- Route changes
- Stop changes
- Rider status changes
- Driver overrides
- Optimization decisions
- Road restriction changes
- Notification activity
- Module activity
- Permission changes
- Administrative actions
- System events

## Optional Plugin Modules

Optional plugins extend TransitMemory without modifying the Core.

### Real-Time Bus Tracking Plugin

Provides real-time vehicle location capabilities.

Features may include:

- Live GPS location
- Vehicle position
- Vehicle heading
- Vehicle speed
- Current route position
- Current stop
- Next stop
- Route progress
- Route deviation detection
- Stop arrival detection
- Stop departure detection
- GPS history
- Trip replay
- Geofencing
- GPS accuracy
- Tracking connection status

Real-time tracking is intentionally optional.

TransitMemory Core can operate without a real-time tracking provider.

### GPS Hardware Plugin

Connects TransitMemory to dedicated GPS hardware installed on vehicles.

### Driver Device Tracking Plugin

Uses an authorized driver's phone, tablet, or other device as a location source.

### Fleet Tracking Plugin

Connects TransitMemory to external fleet tracking systems.

### Telematics Plugin

Connects vehicle telematics data to TransitMemory.

### Mapping Plugin

Provides optional integration with external mapping and geocoding services.

Potential capabilities include:

- Maps
- Geocoding
- Reverse geocoding
- Routing
- Map visualization
- Address validation

### Traffic Data Plugin

Provides external traffic information to the Core ETA and Traffic Intelligence Module.

Potential data sources include:

- Commercial traffic services
- Government transportation feeds
- Municipal traffic feeds
- Construction feeds
- Road closure feeds
- Traffic incident feeds
- Organization-generated traffic data

### Weather Plugin

Provides optional weather information.

Features may include:

- Current weather
- Forecasts
- Severe weather alerts
- Flooding information
- Weather-related route warnings
- Weather-based ETA adjustments

### SMS Plugin

Provides SMS communication for organizations that choose to use text messaging.

### Email Plugin

Provides email communication.

### Push Notification Plugin

Provides mobile and web push notifications.

### Voice Notification Plugin

Provides automated voice notifications where supported by the organization.

### Student Information System Plugin

Connects school transportation information with student information systems.

### School Management Plugin

Connects TransitMemory to school administration systems.

### Attendance Plugin

Connects transportation records with attendance systems.

### Human Resources Plugin

Connects employee transportation systems with organizational personnel systems.

### Customer Management Plugin

Connects transportation operations with customer management systems.

### Identity Provider Plugin

Connects TransitMemory authentication and authorization to external identity providers.

### Fleet Management Plugin

Connects vehicles, maintenance, assignments, and fleet information to external fleet management systems.

### AI Route Advisor Plugin

Provides optional AI-assisted transportation analysis.

Potential capabilities include:

- Route analysis
- Delay analysis
- Schedule recommendations
- Stop optimization
- Route optimization recommendations
- Anomaly detection
- Transportation forecasting
- Natural-language route analysis
- Operational recommendations

AI modules must operate within Core safety, legal, vehicle, rider, and organization-defined constraints.

AI recommendations should be reviewable by authorized human operators before significant route changes are applied.

## API and Interoperability

TransitMemory implementations should provide standardized interfaces for:

- Routes
- Stops
- Riders
- Drivers
- Vehicles
- Schedules
- ETA
- Traffic conditions
- Route history
- Road constraints
- Notifications
- Organization modules
- Plugins
- Events
- Permissions

The specification should support interoperable implementations without requiring a specific programming language, database, mapping provider, GPS provider, cloud platform, or communication provider.

## Data Portability

TransitMemory should support importing and exporting transportation information.

Data portability may include:

- Routes
- Stops
- Riders
- Vehicles
- Drivers
- Schedules
- Route history
- GPS history
- Road restrictions
- Optimization records
- Organizational configuration

Organizations should be able to migrate between compatible TransitMemory implementations without unnecessary vendor lock-in.

## Privacy and Security

TransitMemory is designed for transportation environments that may involve sensitive rider, location, and organizational information.

Implementations should support:

- Authentication
- Authorization
- Role-based access control
- Permission-based data access
- Organization isolation
- Data minimization
- Rider privacy
- Parent and guardian access controls
- Driver access controls
- Dispatcher access controls
- Administrator access controls
- Location access controls
- Historical GPS access controls
- Audit logging
- Configurable retention policies
- Secure module permissions
- Secure API access

## Local-First Operation

TransitMemory should support local-first implementations where practical.

Organizations should be able to maintain operational functionality without requiring continuous dependence on a centralized third-party service.

Local-first implementations may provide:

- Local route data
- Local stop data
- Local rider assignments
- Local route history
- Local driver notes
- Local road knowledge
- Local optimization
- Local module execution
- Synchronization when connectivity becomes available

## Configuration

Organizations can configure:

- Route policies
- Stop policies
- Rider policies
- Driver permissions
- Vehicle restrictions
- ETA rules
- Traffic sources
- Notification rules
- Daily cancellation deadlines
- Safety constraints
- Optimization priorities
- Data retention
- Privacy settings
- Module permissions
- Plugin permissions
- Organization-specific workflows

## Extensibility Requirements

A conforming TransitMemory implementation should allow organizations and developers to extend the system without modifying the Core.

Extensions may add:

- Transportation workflows
- Rider workflows
- Communication interfaces
- Optimization models
- Analytics
- Integrations
- User interfaces
- Organizational policies
- Data sources
- Transportation services
- AI capabilities

The Core establishes the common transportation infrastructure while organizations control their own modules and implementations.

## Suggested Implementation Layers

A TransitMemory implementation may be organized into the following layers:

### Core

Contains the standardized transportation infrastructure and Core Modules.

### Organization Modules

Contains functionality developed by individual organizations to meet their specific operational requirements.

### Communication Modules

Contains customized parent, guardian, customer, rider, or employee interfaces.

### Optional Plugins

Contains integrations and capabilities that are not required by the Core.

### External Services

Contains third-party services such as:

- GPS providers
- Traffic providers
- Mapping services
- Weather providers
- Messaging providers
- Identity providers
- Fleet systems
- AI services

## Conformance

A TransitMemory implementation should document:

- Supported Core Modules
- Supported APIs
- Supported events
- Supported permissions
- Supported organization modules
- Supported plugins
- Supported data formats
- Supported authentication methods
- Supported interoperability features

Implementations may provide additional capabilities as long as those capabilities do not violate the Core specification.

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
  - [https://roxanneardary.com/transitmemory/](https://roxanneardary.com/transitmemory/)  

---

## License & Notice Requirements

TransitMemory is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- TransitMemory specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
