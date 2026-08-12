# World Expedition

## Journey Through History. Experience Today. Discover Tomorrow.

## Overview

World Expedition is an open source specification for designing a real-world higher education program in which artificial intelligence assists students, educators, and institutions in discovering, planning, coordinating, and documenting experiential learning journeys.

The specification treats the real world as an extension of the classroom. Instead of limiting education to lectures, textbooks, simulations, and conventional campus experiences, World Expedition connects academic learning with places, communities, organizations, professionals, historical sites, infrastructure, technologies, industries, research institutions, cultural institutions, and emerging developments.

The system uses AI to help assemble educational routes based on a student's academic program, career interests, learning objectives, available resources, geographic constraints, and desired experiences. Students then travel to relevant destinations, observe real-world conditions, ask questions, interact with people and organizations, participate in appropriate activities, document their experiences, and connect those experiences back to their education and future careers.

World Expedition is designed as a modular architecture. Core modules provide the fundamental capabilities required to operate the experiential education system, while optional plugin modules extend the system for specialized academic disciplines, institutional requirements, travel environments, funding models, accessibility requirements, assessment systems, and emerging technologies.

## Design Principles

World Expedition implementations should follow these principles:

- **Real-world learning:** Academic knowledge should connect to observable and experienceable real-world environments.
- **Student-centered exploration:** Students should have meaningful agency in selecting interests, experiences, questions, and learning paths.
- **AI-assisted discovery:** AI should assist with research, planning, synthesis, and route construction without becoming the final authority.
- **Human oversight:** Educators, qualified professionals, institutions, and students should remain involved in important decisions.
- **Historical continuity:** Experiences should connect the present to relevant historical developments.
- **Present-day observation:** Students should have opportunities to verify knowledge through firsthand observation.
- **Future exploration:** Students should investigate emerging technologies, industries, careers, research, and possible futures.
- **Career relevance:** Experiences should connect academic learning with practical skills and potential career pathways.
- **Evidence-based learning:** Students should distinguish between documented evidence, personal observation, interpretation, and speculation.
- **Source transparency:** AI-generated recommendations and claims should be traceable to their underlying sources whenever practical.
- **Modularity:** Institutions should be able to adopt individual capabilities without implementing the entire system.
- **Interoperability:** Components should use documented interfaces and portable data formats whenever practical.
- **Vendor independence:** Implementations should avoid unnecessary dependence on a single AI provider, mapping service, educational platform, or travel provider.
- **Accessibility:** The system should support students with different physical, financial, geographic, technological, and educational circumstances.
- **Privacy:** Student data should be minimized, protected, and controlled according to applicable institutional and legal requirements.
- **Safety:** Travel and experiential activities must incorporate appropriate risk assessment, institutional policies, and human oversight.
- **Open source implementation:** Implementations should remain compatible with the principles of the AGPL-3.0+ license.

## Core Modules

### Student Profile Module

The Student Profile Module maintains the information required to personalize experiential learning.

Capabilities should include:

- Academic program and area of study
- Courses and learning objectives
- Career interests
- Skills and competencies
- Areas of curiosity
- Preferred learning environments
- Geographic preferences
- Travel limitations
- Time availability
- Budget constraints
- Accessibility requirements
- Prior experiences
- Desired professional exposure
- Student-defined learning goals

Students should be able to review, correct, and control information used to generate recommendations.

### Curriculum Mapping Module

The Curriculum Mapping Module connects academic requirements with potential real-world experiences.

Capabilities should include:

- Course-to-experience mapping
- Learning objective identification
- Competency mapping
- Subject-area relationships
- Academic credit considerations
- Field study opportunities
- Research opportunities
- Internship relationships
- Experiential learning requirements
- Interdisciplinary connections
- Career competency mapping

The module should allow educators to define which experiences satisfy specific educational objectives.

### AI Journey Architect Module

The AI Journey Architect Module transforms educational goals into potential experiential learning journeys.

The AI should be capable of:

- Discovering relevant destinations
- Connecting destinations to academic objectives
- Creating multi-stop routes
- Comparing alternative routes
- Identifying educational opportunities along a route
- Considering transportation and travel constraints
- Considering time and budget constraints
- Prioritizing educational value
- Identifying gaps in a proposed journey
- Suggesting alternate experiences
- Rebuilding routes when circumstances change

The AI should explain why each destination was selected.

### Destination Discovery Module

The Destination Discovery Module identifies places that may provide educational value.

Potential destinations include:

- Historic sites
- Museums
- Universities
- Research facilities
- Businesses
- Manufacturing facilities
- Government institutions
- Cultural institutions
- Natural environments
- Infrastructure projects
- Engineering projects
- Hospitals and healthcare institutions
- Farms and agricultural operations
- Energy facilities
- Technology organizations
- Startups
- Nonprofit organizations
- Creative organizations
- Professional associations
- Laboratories
- Libraries
- Archives
- Archaeological sites
- Public spaces
- Planned developments
- Emerging technology demonstrations

Destinations should be evaluated according to educational relevance rather than tourism popularity alone.

### Historical Context Module

The Historical Context Module provides the historical foundation for each learning destination.

Capabilities should include:

- Historical timelines
- Major events
- Important individuals
- Cultural developments
- Technological developments
- Economic developments
- Political and institutional developments
- Scientific developments
- Previous uses of a location
- Historical conflicts and competing interpretations
- Primary and secondary sources
- Connections between historical events and present conditions

Historical information should identify sources and distinguish established evidence from interpretation.

### Present Experience Module

The Present Experience Module identifies what students can observe and learn at a destination today.

Capabilities should include:

- Current organizations
- Current industries
- Active projects
- Current technologies
- Current infrastructure
- Current research
- Professional environments
- Public programs
- Demonstrations
- Exhibitions
- Workshops
- Community activities
- Current challenges
- Current opportunities

The objective is to help students understand how academic concepts operate in real environments.

### Future Outlook Module

The Future Outlook Module connects present-day observations with emerging possibilities.

Capabilities should include:

- Emerging technologies
- Research developments
- Planned infrastructure
- New industries
- Emerging occupations
- Startup ecosystems
- Scientific developments
- Policy changes
- Forecasts
- Competing future scenarios
- Potential risks
- Potential opportunities

The system must distinguish between established information, credible projections, speculative scenarios, and AI-generated possibilities.

### Professional Connection Module

The Professional Connection Module connects students with people working in relevant fields.

Potential connections include:

- Professionals
- Researchers
- Entrepreneurs
- Engineers
- Scientists
- Artists
- Craftspeople
- Government officials
- Educators
- Business owners
- Community leaders
- Technicians
- Industry specialists
- Nonprofit professionals

The system should identify appropriate opportunities for observation, interviews, mentorship, demonstrations, job shadowing, internships, and other approved interactions.

### Question Generation Module

The Question Generation Module helps students prepare for firsthand experiences.

The AI should generate questions based on:

- Academic subjects
- Student interests
- Destination history
- Current conditions
- Professional roles
- Technologies
- Career pathways
- Future developments
- Contradictory evidence
- Student learning objectives

Students should be encouraged to modify, reject, and create their own questions.

### Experiential Learning Module

The Experiential Learning Module converts destinations into structured learning experiences.

Experiences may include:

- Field observations
- Interviews
- Guided tours
- Site studies
- Research activities
- Workshops
- Demonstrations
- Job shadowing
- Apprenticeship activities
- Community engagement
- Field experiments
- Documentation projects
- Comparative studies
- Problem-solving exercises
- Student-designed investigations

Activities must be appropriate to the student's educational level, institutional policies, and safety requirements.

### Observation and Verification Module

The Observation and Verification Module allows students to compare prior information with firsthand experience.

Students should be able to document:

- What they expected to find
- What they actually observed
- What differed from the AI's recommendations
- What information was confirmed
- What information was incorrect
- What information remained uncertain
- New questions that emerged
- Evidence collected
- Conversations held
- Personal observations
- Photographs and permitted media
- Supporting documentation

This module establishes firsthand observation as an important source of learning rather than treating AI output as unquestionable truth.

### Reflection Module

The Reflection Module transforms experiences into academic learning.

Students should be able to record:

- What they learned
- What surprised them
- What contradicted previous assumptions
- How the experience relates to coursework
- How the experience relates to potential careers
- What questions remain unanswered
- What they would investigate next
- How their perspective changed
- What skills they developed

### Portfolio Module

The Portfolio Module creates a durable record of experiential learning.

Portfolio materials may include:

- Field reports
- Research
- Interviews
- Observations
- Projects
- Photographs
- Presentations
- Maps
- Data
- Reflections
- Competency evidence
- Professional contacts
- Student-created work
- Faculty evaluations

Students should retain control over which portfolio materials are public, private, institutional, or shared with prospective employers.

### Career Alignment Module

The Career Alignment Module connects educational experiences with potential career pathways.

Capabilities should include:

- Career exploration
- Occupation mapping
- Skill identification
- Competency development
- Professional exposure tracking
- Employer discovery
- Internship discovery
- Apprenticeship discovery
- Research opportunity discovery
- Portfolio alignment
- Emerging career identification

The system should expose students to careers they may not have previously considered while allowing students to reject recommendations.

### Route Optimization Module

The Route Optimization Module continuously evaluates and improves experiential journeys.

Optimization criteria may include:

- Educational value
- Distance
- Travel time
- Transportation
- Cost
- Schedule
- Availability
- Weather
- Accessibility
- Safety
- Student preferences
- Institutional requirements
- Destination operating conditions
- Required appointments
- Academic deadlines

The system should support alternative routes and graceful degradation when a destination becomes unavailable.

### Faculty Module

The Faculty Module provides educators with tools for integrating experiential learning into academic programs.

Capabilities should include:

- Defining learning objectives
- Approving destinations
- Creating assignments
- Reviewing student experiences
- Evaluating reflections
- Mapping experiences to coursework
- Providing feedback
- Establishing required experiences
- Creating optional experiences
- Monitoring learning progress
- Identifying gaps in experiential exposure

Faculty should retain authority over academic requirements.

### Institutional Module

The Institutional Module allows colleges, universities, and other educational organizations to define program-wide policies.

Capabilities should include:

- Academic requirements
- Travel policies
- Safety policies
- Approved destinations
- Insurance requirements
- Accessibility standards
- Student privacy requirements
- Faculty responsibilities
- Credit policies
- Funding policies
- Partner requirements
- Data governance
- Institutional approval workflows

### Safety and Governance Module

The Safety and Governance Module establishes safeguards for real-world educational activity.

Capabilities should include:

- Risk assessment
- Destination screening
- Travel advisories
- Emergency procedures
- Contact requirements
- Institutional approvals
- Supervision requirements
- Activity restrictions
- Student consent
- Accessibility considerations
- Incident documentation
- Human escalation

AI recommendations must never override institutional safety requirements or qualified human judgment.

### Accessibility Module

The Accessibility Module ensures that experiential learning objectives can be pursued by students with different needs.

Capabilities should include:

- Accessible destination discovery
- Mobility considerations
- Transportation accessibility
- Sensory considerations
- Alternative experiences
- Remote participation
- Financial accessibility
- Technology accessibility
- Communication accessibility

Alternative experiences should preserve the underlying learning objective whenever possible rather than simply replacing the experience with unrelated online material.

### Funding and Scholarship Module

The Funding and Scholarship Module identifies resources that can make experiential education financially accessible.

Potential resources include:

- Scholarships
- Grants
- Institutional funding
- Research funding
- Travel awards
- Employer sponsorships
- Community partnerships
- Fellowships
- Paid experiential opportunities
- Work-study opportunities

The system should clearly distinguish verified funding opportunities from AI-generated suggestions.

### Community Knowledge Module

The Community Knowledge Module recognizes local communities as sources of knowledge.

Capabilities should include:

- Local experts
- Community organizations
- Oral histories
- Local businesses
- Cultural institutions
- Community projects
- Local research
- Indigenous and traditional knowledge where appropriately shared
- Community-defined educational opportunities

Community participation should be respectful, consensual, and appropriately compensated when applicable.

### Knowledge Provenance Module

The Knowledge Provenance Module records the origin of information used by the system.

Sources may include:

- Academic publications
- Government sources
- Institutional websites
- Historical archives
- Museums
- Research organizations
- Professional organizations
- Community sources
- Firsthand student observations
- Verified datasets
- Other documented sources

The system should preserve provenance wherever practical and identify information that cannot be independently verified.

### AI Transparency Module

The AI Transparency Module makes the distinction between information types visible to students and educators.

The system should distinguish:

- Verified facts
- Source-derived information
- Institutional information
- Historical interpretation
- Professional opinion
- Student observation
- Forecast
- Scenario
- AI-generated inference
- AI-generated recommendation

AI-generated content should never be presented as firsthand observation or verified fact.

### Privacy and Data Governance Module

The Privacy and Data Governance Module governs student and institutional data.

Implementations should provide:

- Data minimization
- User consent
- Access controls
- Data retention policies
- Data export
- Data deletion
- Privacy controls
- Audit records
- Secure storage
- Provider transparency
- Protection against unnecessary data collection

Students should have meaningful control over personal information associated with their educational journeys.

### Assessment Module

The Assessment Module evaluates experiential learning.

Assessment may consider:

- Knowledge acquisition
- Critical thinking
- Observation
- Research ability
- Communication
- Problem solving
- Professional interaction
- Reflection
- Application of academic concepts
- Demonstrated competencies
- Ability to distinguish evidence from assumption
- Ability to evaluate conflicting information

Assessment should prioritize demonstrated learning rather than the number of destinations visited.

### Interoperability Module

The Interoperability Module defines mechanisms for connecting World Expedition implementations with external educational and technical systems.

Potential integrations include:

- Learning management systems
- Student information systems
- Academic catalogs
- Mapping systems
- Transportation systems
- Calendar systems
- Travel services
- Research databases
- Library systems
- Career platforms
- Portfolio systems
- AI providers
- Institutional identity systems

Implementations should avoid unnecessary proprietary dependencies.

## Optional Plugin Modules

World Expedition should support optional plugins that extend the core system without requiring every implementation to adopt every capability.

### Academic Discipline Plugins

Plugins may specialize the system for:

- Architecture
- Engineering
- Medicine
- Nursing
- Agriculture
- Environmental science
- Computer science
- Artificial intelligence
- Business
- Economics
- History
- Anthropology
- Archaeology
- Sociology
- Political science
- Law
- Education
- Art
- Music
- Journalism
- Film
- Hospitality
- Skilled trades
- Manufacturing
- Construction

### Research Expedition Plugin

Provides advanced support for field research, data collection, research documentation, scientific observation, and faculty-led expeditions.

### Internship and Apprenticeship Plugin

Connects educational journeys with internships, apprenticeships, job shadowing, cooperative education, and employment opportunities.

### International Education Plugin

Provides support for international travel, cross-cultural education, international institutions, language learning, and global academic experiences.

### Road Trip Education Plugin

Optimizes educational journeys conducted primarily by automobile, RV, bus, or other overland transportation.

### Public Transportation Plugin

Optimizes journeys around rail, bus, subway, ferry, and other public transportation networks.

### Virtual Expedition Plugin

Provides alternative or complementary experiences when physical travel is unavailable.

### Museum and Cultural Institution Plugin

Connects students with museums, archives, libraries, galleries, historic sites, cultural organizations, and exhibitions.

### Industry Immersion Plugin

Connects students with businesses, manufacturing facilities, technology companies, laboratories, professional organizations, and industry environments.

### Future Studies Plugin

Provides structured exploration of emerging technologies, economic changes, scientific developments, demographic changes, new occupations, and alternative future scenarios.

### AI Provider Plugin

Allows an implementation to connect with different AI models or providers without making the core architecture dependent on one provider.

### Mapping Provider Plugin

Allows implementations to use different geographic and mapping services.

### Funding Discovery Plugin

Provides specialized scholarship, grant, fellowship, sponsorship, and institutional funding discovery.

### Alumni Network Plugin

Connects students with alumni who can provide professional perspectives, mentorship, interviews, and career guidance.

### Employer Network Plugin

Allows participating employers to provide educational experiences, site visits, demonstrations, projects, internships, and career opportunities.

### Community Partnership Plugin

Provides tools for community organizations to participate in experiential education programs.

### Accessibility Services Plugin

Provides specialized accessibility assessment and alternative experience planning.

### Language Learning Plugin

Connects destinations and experiences with language acquisition and cultural immersion.

### Credentialing Plugin

Allows institutions to issue certificates, microcredentials, competency records, or other recognized documentation for completed experiential learning.

### Gamification Plugin

Adds optional achievement systems, challenges, badges, milestones, exploration goals, and collaborative learning activities without making gamification a requirement of the educational model.

## Operational Workflow

A World Expedition implementation should support a continuous experiential learning cycle:

**Discover → Plan → Prepare → Travel → Observe → Question → Experience → Document → Reflect → Assess → Connect → Discover Again**

### Discover

The student identifies academic interests, career goals, questions, and areas they want to explore.

### Plan

The AI Journey Architect constructs potential routes and identifies relevant destinations and experiences.

### Prepare

The system provides historical context, current information, questions, learning objectives, safety information, and preparation materials.

### Travel

The student travels to approved destinations using appropriate transportation and institutional procedures.

### Observe

The student examines the real environment and compares firsthand observations with previously provided information.

### Question

The student asks prepared questions and develops new questions based on what they encounter.

### Experience

The student participates in appropriate educational, professional, research, cultural, or community activities.

### Document

The student records observations, evidence, interviews, research, and other permitted materials.

### Reflect

The student connects the experience to academic learning, career development, and personal understanding.

### Assess

Faculty, institutions, or approved evaluators assess the student's demonstrated learning and competencies.

### Connect

The system connects the experience to future coursework, careers, research, internships, apprenticeships, and additional destinations.

### Discover Again

New knowledge and questions become inputs for the next experiential learning journey.

## AI Decision Framework

AI systems operating within World Expedition should function as assistants, navigators, researchers, and synthesis tools rather than autonomous academic authorities.

AI recommendations should:

- Explain their reasoning where practical.
- Identify supporting sources.
- Identify uncertainty.
- Identify assumptions.
- Distinguish facts from predictions.
- Present alternatives.
- Allow human review.
- Allow student modification.
- Avoid fabricating destinations, organizations, events, or opportunities.
- Avoid representing unavailable experiences as available.
- Reevaluate recommendations when source information changes.

Important decisions involving academic credit, safety, student welfare, institutional policy, or significant financial commitments should include appropriate human oversight.

## Destination Evaluation

Each destination should be evaluated according to multiple dimensions rather than popularity alone.

Evaluation criteria may include:

- Educational relevance
- Historical significance
- Current relevance
- Future relevance
- Career relevance
- Experiential opportunities
- Professional access
- Research value
- Community value
- Accessibility
- Cost
- Travel requirements
- Safety
- Source quality
- Availability
- Student interest

The system should explain the factors contributing to a recommendation.

## Experiential Learning Records

Each completed experience should produce a structured learning record.

A record may contain:

- Destination
- Date
- Academic objective
- Career objective
- Preparation materials
- Questions
- Activities
- Observations
- Evidence
- People encountered
- Sources consulted
- Student reflections
- Faculty feedback
- Competencies demonstrated
- Follow-up opportunities
- Future research questions

Students should be able to export their records in portable formats.

## Academic Integration

World Expedition should support integration with conventional higher education rather than requiring institutions to abandon existing educational structures.

Possible models include:

- Field assignments within existing courses
- Required experiential learning credits
- Elective expedition programs
- Semester-long travel programs
- Faculty-led expeditions
- Research expeditions
- Cooperative education
- Internships
- Apprenticeships
- Capstone projects
- Career exploration programs
- Independent study
- Interdisciplinary programs
- Degree pathways incorporating continuous field experience

## Program Models

Implementations may support different scales of participation.

### Local Expedition

A short experience within the student's local region.

### Regional Expedition

A multi-destination journey covering a larger geographic area.

### National Expedition

A journey across multiple states or regions connected to a student's educational objectives.

### International Expedition

A cross-border educational journey incorporating international experiences.

### Longitudinal Expedition

A series of experiences conducted throughout a student's academic program.

### Degree Expedition

A complete educational pathway in which experiential journeys form a major component of the student's academic progression.

## Student Agency

Students should be active participants in constructing their education.

The system should allow students to:

- Reject recommendations
- Request alternatives
- Change priorities
- Add destinations
- Remove destinations
- Create questions
- Challenge AI conclusions
- Document contradictions
- Propose experiences
- Develop independent research
- Create their own learning routes

The AI should expand the student's possibilities rather than narrow them unnecessarily.

## Human-in-the-Loop Governance

World Expedition implementations should establish clear responsibilities among:

- Students
- Faculty
- Advisors
- Institutions
- Destination organizations
- Community partners
- Employers
- Researchers
- AI systems
- Service providers

The system should make clear which decisions can be automated and which require human authorization.

## Quality Assurance

Implementations should continuously evaluate:

- Recommendation accuracy
- Source quality
- Destination availability
- Student outcomes
- Learning outcomes
- Safety performance
- Accessibility
- Cost effectiveness
- AI error rates
- Student satisfaction
- Faculty satisfaction
- Partner satisfaction
- Career outcomes

Student and faculty feedback should be incorporated into future recommendations.

## Failure Handling

The system should anticipate that real-world conditions change.

It should support:

- Destination closures
- Canceled events
- Weather disruptions
- Transportation disruptions
- Schedule changes
- Incorrect information
- Unavailable professionals
- Funding changes
- Safety concerns
- Student schedule changes
- Changes in academic requirements

When a planned experience becomes unavailable, the system should identify alternatives that preserve the original learning objective whenever possible.

## Security

Implementations should protect:

- Student accounts
- Educational records
- Travel information
- Personal information
- Institutional data
- Partner information
- Authentication credentials
- API credentials
- AI provider credentials
- Private research
- Portfolio materials

Security controls should follow applicable institutional and legal requirements.

## Privacy

World Expedition should not require unnecessary personal information to provide educational recommendations.

Implementations should provide transparent policies covering:

- What information is collected
- Why information is collected
- How information is processed
- Which organizations receive information
- How long information is retained
- How students can access their information
- How students can export their information
- How students can request deletion where applicable

## Extensibility

The core architecture should allow additional modules and plugins to be introduced without requiring fundamental redesign.

Extensions should have:

- Clear interfaces
- Documented capabilities
- Defined permissions
- Version compatibility
- Failure isolation
- Configuration controls
- Data handling requirements
- Security requirements

Optional plugins should not silently alter core educational, safety, privacy, or governance behavior.

## Implementation Requirements

A conforming implementation should:

- Support student-centered experiential learning.
- Provide a mechanism for mapping educational objectives to real-world experiences.
- Provide AI-assisted discovery or route construction.
- Distinguish AI recommendations from verified information.
- Provide source provenance where practical.
- Support firsthand observation and documentation.
- Provide mechanisms for human oversight.
- Protect student and institutional data.
- Support accessibility considerations.
- Provide mechanisms for handling unavailable or changed destinations.
- Support modular extension through optional capabilities.
- Remain compatible with the AGPL-3.0+ licensing requirements of the project.

## Recommended Experience Model

A World Expedition experience should connect three perspectives:

**Past:** What happened here, how did it develop, and what can be learned from it?

**Present:** What is happening here now, who is involved, and what can the student experience firsthand?

**Future:** What could happen next, what technologies or careers are emerging, and what possibilities should the student investigate?

This three-perspective model forms the conceptual foundation of World Expedition.

## Long-Term Vision

World Expedition envisions a higher education model in which students do not wait until graduation to encounter the professional and social environments they are preparing to enter.

A student studying engineering should be able to see infrastructure, manufacturing, laboratories, construction, research, and emerging technologies.

A student studying history should be able to stand where history occurred, examine primary sources, speak with historians, and compare competing interpretations.

A student studying business should be able to observe companies, markets, supply chains, entrepreneurship, manufacturing, finance, and emerging industries.

A student studying environmental science should be able to observe ecosystems, conservation projects, agriculture, energy systems, water infrastructure, and environmental management firsthand.

A student studying artificial intelligence should be able to encounter research institutions, data centers, robotics systems, AI companies, public applications, and communities affected by the technology.

The destination changes according to the student, but the underlying principle remains the same:

**Education should prepare students for the world by allowing them to experience the world while they learn.**

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
  - [https://roxanneardary.com/world-expedition/](https://roxanneardary.com/world-expedition/)  

---

## License & Notice Requirements

World Expedition is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- World Expedition specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.
  Any update that adds new contributors or modifies attribution should also update `notice.md`.
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
