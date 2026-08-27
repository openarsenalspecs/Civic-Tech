# PassTheMic Specification
**Better Words. Better Manners. Better Conversations.**
- HTML Mirror: [https://roxanneardary.com/passthemic-specification/](https://roxanneardary.com/passthemic-specification/)  

---

## Overview

PassTheMic is a voice-first AI language tutor and conversation coach designed to teach language fluency alongside the skills required to participate effectively in real conversations. The system combines language instruction, voice interaction, dialect awareness, speech-speed control, conversational intelligence, active listening, manners, gratitude, cultural awareness, and social communication into a modular architecture.

PassTheMic is designed to help students learn not only what to say, but how to listen, respond, ask meaningful questions, share conversational space, communicate respectfully, express appreciation, understand cultural context, and adapt their communication to different people and situations.

The system must support multiple AI instructor and coach characters that students can select according to their preferred personality, teaching style, voice, dialect, accent, communication style, and coaching approach.

## Design Principles

- Voice-first interaction
- Modular architecture
- Open source implementation
- Local-first operation where technically feasible
- Model independence
- Vendor neutrality
- User control
- Privacy by design
- Configurable AI characters
- Adaptive learning
- Human-centered communication
- Cultural awareness
- Conversational reciprocity
- Accessibility
- Explainable coaching
- Non-diagnostic behavioral analysis
- Interoperability
- Extensible plugin architecture

---

## Core System Module

The Core System Module provides the shared infrastructure required by all PassTheMic modules.

The module must provide:

- Module lifecycle management
- Configuration management
- Shared user profiles
- Shared learning profiles
- Session management
- Event management
- Inter-module communication
- Permission management
- Feature configuration
- Model abstraction
- Voice-service abstraction
- Language-service abstraction
- Character-service abstraction
- Data-management interfaces
- Privacy controls
- Security controls
- Logging controls
- Local and remote service configuration
- Plugin management interfaces
- Accessibility interfaces

All modules should communicate through defined interfaces rather than creating unnecessary dependencies between individual modules.

## Voice Interaction Module

The Voice Interaction Module provides the primary spoken interface between the student and PassTheMic.

The module must support:

- Voice activation
- Hands-free interaction
- Wake-word activation where supported
- Push-to-talk interaction
- Continuous conversation mode
- Voice activity detection
- Speaker turn detection
- Natural pause recognition
- Speech overlap detection
- Real-time speech recognition
- Speech-to-text transcription
- Text-to-speech responses
- Voice activity indicators
- Microphone permissions
- Recording controls
- Conversation mute controls
- Adjustable response timing
- Configurable listening duration
- Background-noise handling
- Voice input calibration
- Voice output calibration
- Audio device selection

The system should support local speech processing where technically feasible and allow external speech services through modular interfaces.

## Speech Speed Module

The Speech Speed Module allows students to control the speed of AI speech and develop awareness of their own conversational pace.

The module must support:

- Slow speech
- Normal speech
- Fast speech
- Fine-grained speed adjustment
- Custom speed settings
- Character-specific speech speed
- Lesson-specific speech speed
- Conversation-specific speech speed
- Temporary speed adjustments
- Persistent speed preferences
- Speech-speed presets
- Real-time speed controls
- Student speech-speed analysis
- Words-per-minute analysis
- Speaking-duration analysis
- Pause-frequency analysis
- Pause-duration analysis
- Response-latency analysis
- Speech-burst analysis
- Speech-speed consistency analysis
- Individual speech-speed baselines
- Adaptive speech-speed coaching
- Progressive speed training
- Slow-to-natural speech progression
- Natural-to-native-speed training
- Speed and pronunciation analysis
- Speed and comprehension analysis
- Speed and conversational pacing analysis

The system must not treat faster speech as inherently superior.

Speech speed should be evaluated according to clarity, comprehension, context, language, dialect, conversational partner, and communication goals.

## Speech Analysis Module

The Speech Analysis Module analyzes characteristics of spoken communication.

The module may analyze:

- Pronunciation
- Articulation
- Speech rate
- Pauses
- Rhythm
- Cadence
- Intonation
- Stress
- Volume
- Speech clarity
- Filler words
- Repetition
- Hesitation
- Turn timing
- Interruptions
- Overlapping speech
- Changes in speaking speed
- Changes in vocal characteristics

The module should distinguish between language-learning errors and legitimate speech variation.

## Dialect and Accent Module

The Dialect and Accent Module provides dialect-aware language learning and conversational interaction.

The module must support:

- Dialect recognition
- Accent recognition
- Accent adaptation
- Regional vocabulary
- Regional grammar
- Slang
- Idioms
- Pronunciation variation
- Speech-pattern variation
- Cadence
- Intonation
- Code-switching
- Dialect-aware speech recognition
- User-selected target dialects
- User-selected target accents
- Standard-language instruction
- Regional-language instruction
- Dialect comparison
- Dialect-specific vocabulary lessons
- Dialect-specific pronunciation lessons
- Dialect-aware correction
- Dialect-aware speech-speed analysis
- Recognition of legitimate dialect variations

The system must avoid treating legitimate dialect differences as errors solely because they differ from a standardized language model.

## Language Learning Module

The Language Learning Module provides general language-learning functionality shared by language-specific modules.

The module must support:

- Vocabulary instruction
- Grammar instruction
- Sentence construction
- Pronunciation training
- Listening comprehension
- Reading comprehension
- Writing practice
- Speaking practice
- Translation exercises
- Idiom instruction
- Slang instruction
- Colloquial language
- Formal language
- Informal language
- Professional language
- Academic language
- Travel language
- Everyday language
- Language immersion
- Vocabulary retention
- Spaced repetition
- Adaptive difficulty
- Personalized lessons
- Language assessment
- Error correction
- Natural-expression coaching
- Language proficiency tracking

## English Language Module

The English Language Module provides dedicated English-language instruction.

It must support:

- English vocabulary
- English grammar
- English pronunciation
- English phonetics
- English listening comprehension
- English speaking practice
- English writing practice
- English idioms
- English slang
- English regional variations
- English dialect instruction
- English accent training
- English conversation
- English cultural communication
- English-specific speech-speed training

The architecture must allow English to operate independently as a language module without requiring language-specific logic to be embedded in the core system.

## Spanish Language Module

The Spanish Language Module provides dedicated Spanish-language instruction.

It must support:

- Spanish vocabulary
- Spanish grammar
- Spanish pronunciation
- Spanish phonetics
- Spanish listening comprehension
- Spanish speaking practice
- Spanish writing practice
- Spanish idioms
- Spanish slang
- Spanish regional variations
- Spanish dialect instruction
- Spanish accent training
- Spanish conversation
- Spanish cultural communication
- Spanish-specific speech-speed training

## Additional Language Modules

Every supported language must have its own dedicated language module.

Each language module should provide:

- Language-specific vocabulary
- Language-specific grammar
- Language-specific pronunciation
- Language-specific phonetics
- Language-specific listening comprehension
- Language-specific speaking practice
- Language-specific writing practice
- Language-specific idioms
- Language-specific slang
- Language-specific dialects
- Language-specific accents
- Language-specific cultural context
- Language-specific conversation patterns
- Language-specific speech-speed considerations
- Language-specific learning progression
- Language-specific assessment
- Language-specific language resources

Additional languages should be added as independent modules without requiring changes to unrelated language modules.

## Pronunciation Module

The Pronunciation Module provides detailed pronunciation training.

The module must support:

- Phoneme identification
- Phoneme production practice
- Word pronunciation
- Sentence pronunciation
- Connected speech
- Stress patterns
- Intonation
- Rhythm
- Articulation
- Pronunciation comparison
- Pronunciation scoring
- Target-language pronunciation
- Dialect-specific pronunciation
- Accent-specific pronunciation
- Slow pronunciation practice
- Natural-speed pronunciation practice
- Fast-speech pronunciation practice

## Lip Syncing Module

The Lip Syncing Module synchronizes AI character facial and mouth movements with generated speech.

The module must support:

- Real-time lip synchronization
- Audio-to-mouth synchronization
- Phoneme-to-viseme mapping
- Viseme timing
- Character facial animation
- Mouth-shape transitions
- Natural speech timing
- Adjustable synchronization latency
- Character-specific facial rigs
- Language-aware lip movement
- Dialect-aware timing
- Speech-speed-aware animation
- Emotional facial expression synchronization
- Pauses and silence synchronization
- Interruption-aware animation
- Streaming lip synchronization
- Offline lip synchronization where supported

Lip synchronization should remain synchronized when speech speed, language, dialect, or AI character changes.

The system should separate lip-sync interfaces from the underlying language and speech systems so different animation engines can be supported.

## AI Character Module

The AI Character Module provides selectable AI instructors and conversation coaches.

The system must support multiple characters with configurable:

- Names
- Voices
- Personalities
- Teaching styles
- Coaching styles
- Conversation styles
- Dialects
- Accents
- Formality
- Vocabulary
- Emotional expression
- Speaking speed
- Response timing
- Questioning style
- Correction style
- Encouragement style
- Roleplay behavior

Students must be able to select and switch characters.

Characters may specialize in:

- Grammar
- Vocabulary
- Pronunciation
- Conversation
- Listening
- Manners
- Gratitude
- Cultural communication
- Professional communication
- Casual communication
- Difficult conversations
- Speech-speed training

## Conversation Coach Module

The Conversation Coach Module provides real-time and post-conversation coaching.

It must support:

- Conversation practice
- Natural conversation simulation
- Small-talk practice
- Storytelling practice
- Question-and-answer practice
- Spontaneous speaking
- Topic transitions
- Topic maintenance
- Conversation openings
- Conversation closings
- Conversation recovery
- Clarification practice
- Active listening practice
- Reflective response practice
- Follow-up question practice
- Conversational confidence building
- Conversational pacing
- Response timing
- Silence tolerance
- Professional conversation
- Casual conversation
- Group conversation simulation

## Conversation Reciprocity Module

The Conversation Reciprocity Module teaches students to participate in balanced conversations.

It must analyze:

- Speaking time
- Turn-taking
- Conversation balance
- Topic ownership
- Topic redirection
- Topic return
- Follow-up questions
- Other-focused responses
- Self-focused responses
- Conversational openings
- Unanswered openings
- Conversational opportunities
- Airtime distribution
- Conversation dominance
- Reciprocity

The system should provide feedback designed to help students recognize when they are speaking too much, redirecting conversation toward themselves, failing to ask questions, or failing to return attention to another person.

## Pass the Mic Module

The Pass the Mic Module is the central conversational-awareness system.

It teaches students:

- To listen before responding
- To ask follow-up questions
- To avoid immediately matching every story with their own
- To recognize when they are redirecting attention toward themselves
- To return the conversation to another speaker
- To share conversational airtime
- To avoid conversational competition
- To recognize story one-upmanship
- To notice repeated self-reference
- To make room for another person
- To reclaim their own conversational space
- To recognize when another person is taking over the conversation
- To respectfully redirect a conversation
- To set conversational boundaries
- To recognize when a conversation has become one-sided

The system should teach the principle:

**Being interesting is not the same as being interested.**

The system should reinforce the principle:

**Great conversations are not competitions for airtime.**

## Follow-Up Question Module

The Follow-Up Question Module teaches students to demonstrate curiosity and maintain conversational continuity.

It must support:

- Context-aware questions
- Open-ended questions
- Clarifying questions
- Reflective questions
- Emotional questions
- Interest-based questions
- Story-continuation questions
- Professional questions
- Social questions
- Cultural questions
- Follow-up question suggestions
- Question-quality analysis
- Relevance analysis
- Repetition detection
- Topic-change detection

The system should teach students to consider asking a follow-up question before immediately sharing their own related experience.

## Active Listening Module

The Active Listening Module teaches students to listen for understanding.

It must support:

- Listening comprehension
- Topic continuity
- Response relevance
- Key-detail recognition
- Emotional-context recognition
- Clarification
- Paraphrasing
- Reflective responses
- Verbal acknowledgments
- Listening exercises
- Listening quizzes
- Listening roleplay
- Listening-speed adaptation
- Premature-response detection
- Unrelated-response detection

## Interruption Module

The Interruption Module analyzes conversational interruptions and teaches appropriate turn-taking.

It must support:

- Interruption detection
- Overlapping speech detection
- Accidental interruption recognition
- Enthusiastic overlap recognition
- Clarification interruption recognition
- Supportive interruption recognition
- Repeated interruption detection
- Topic-stealing interruption detection
- Competitive interruption detection
- Interruption-frequency tracking
- Waiting-for-turn exercises
- Pause practice
- Conversational timing practice
- Appropriate interruption training

## Conversational Self-Awareness Module

The Conversational Self-Awareness Module helps students recognize their own communication patterns.

It may analyze:

- Frequency of self-reference
- Frequency of "I"
- Frequency of "me"
- Frequency of "my"
- Frequency of "mine"
- Self-disclosure
- Self-focused responses
- Other-focused responses
- Story length
- Question frequency
- Follow-up frequency
- Interruption frequency
- Speaking time
- Topic redirection
- Topic return
- Conversation balance

The system must distinguish normal self-reference from excessive self-focused conversation.

## Story Matching Module

The Story Matching Module teaches students how to relate personal experiences without taking over the conversation.

It must support:

- Related-story detection
- Personal-experience matching
- Empathetic story matching
- Competitive story matching
- Excessive story matching
- Story relevance
- Story length
- Conversational redirection detection
- Topic-return coaching
- "Tell me more" prompts
- Story-to-question transitions
- Personal-story balance

## Topic Return Module

The Topic Return Module teaches students how to return attention to the original speaker or topic.

It must support:

- Topic-return detection
- Topic-return reminders
- Personal-story return prompts
- Follow-up prompts
- Conversation recovery
- Unfinished-topic detection
- Topic-continuity coaching
- Topic-return phrases
- Conversational reciprocity exercises

Example coaching phrases may include:

- "Tell me more about that."
- "What happened next?"
- "How are you handling that?"
- "I want to go back to what you were saying."
- "But tell me more about your experience."

## Manners Module

The Manners Module teaches students how to communicate politely and respectfully.

It must support:

- Greetings
- Introductions
- Requests
- Thank-you expressions
- Apologies
- Turn-taking
- Appropriate interruptions
- Respectful disagreement
- Appropriate forms of address
- Professional etiquette
- Social etiquette
- Dining etiquette
- Digital etiquette
- Conversation etiquette
- Boundary-respecting communication
- Polite refusal
- Polite correction
- Polite disagreement
- Polite requests
- Polite conversation endings
- Context-sensitive manners

## Politeness Detection Module

The Politeness Detection Module evaluates whether language is appropriate for the conversational context.

It may identify:

- Abrupt language
- Demanding language
- Dismissive language
- Rude language
- Excessively formal language
- Inappropriate informality
- Contextual politeness
- Tone
- Formality
- Social appropriateness

The system should explain why an expression may be inappropriate and offer alternative phrasing.

## Gratitude Module

The Gratitude Module teaches students how to recognize and communicate appreciation.

It must support:

- Saying thank you
- Expressing appreciation
- Thanking someone for their time
- Thanking someone for their help
- Acknowledging effort
- Appreciating generosity
- Appreciating attention
- Appreciating emotional support
- Thanking someone for a gift
- Thanking someone for an invitation
- Professional gratitude
- Personal gratitude
- Social gratitude
- Written gratitude
- Spoken gratitude
- Receiving gratitude
- Receiving compliments
- Giving compliments
- Gratitude roleplay
- Culturally appropriate gratitude

The system should distinguish gratitude from unnecessary apologizing.

## Polite Assertiveness Module

The Polite Assertiveness Module teaches students how to maintain boundaries while remaining respectful.

It must support:

- Saying no politely
- Setting boundaries
- Correcting someone respectfully
- Disagreeing respectfully
- Asking someone to stop
- Reclaiming a conversation
- Asking someone to let them finish
- Declining invitations
- Declining requests
- Expressing discomfort
- Ending uncomfortable conversations
- Responding to rude behavior
- Distinguishing politeness from submission
- Maintaining dignity while being courteous

## Emotional Conversation Module

The Emotional Conversation Module teaches students how to respond appropriately when conversations involve vulnerability or emotional subjects.

It must support:

- Responding to vulnerable disclosures
- Emotional listening
- Empathetic responses
- Validation
- Supportive questions
- Avoiding immediate self-redirection
- Avoiding story competition
- Emotional cue recognition
- Appropriate self-disclosure
- Emotional boundaries
- Sensitive-topic roleplay
- Difficult-conversation practice
- Appropriate conversational pacing
- Appropriate response timing

The system should not present itself as a replacement for professional mental health care.

## Cultural Communication Module

The Cultural Communication Module teaches students how communication varies across cultures and regions.

It must support:

- Country-specific communication guidance
- Regional communication guidance
- Dialect-specific etiquette
- Cultural greetings
- Cultural politeness
- Cultural gratitude
- Cultural conversation norms
- Formality differences
- Silence norms
- Interruption norms
- Storytelling norms
- Gift etiquette
- Hospitality
- Workplace etiquette
- Cross-cultural conversation
- Cultural speech-speed differences

Cultural guidance must be presented as contextual information rather than universal rules.

## Roleplay Module

The Roleplay Module provides realistic conversational scenarios.

It must support:

- First meetings
- Friendships
- Dating conversations
- Workplace conversations
- Networking
- Interviews
- Customer service
- Travel
- Restaurants
- Shopping
- Family conversations
- Neighbor interactions
- Classroom conversations
- Professional meetings
- Difficult conversations
- Conflict
- Emotional conversations
- Cross-cultural conversations
- Group conversations
- Public speaking
- Dialect-specific scenarios
- Speech-speed scenarios

## Lip Sync Character Module

The Lip Sync Character Module connects the AI character system to visual speech animation.

It must support:

- Character mouth animation
- Phoneme-driven mouth movement
- Viseme-driven mouth movement
- Language-specific phoneme timing
- Speech-speed synchronization
- Natural facial movement
- Facial expressions
- Eye movement
- Head movement
- Conversational gestures
- Pause synchronization
- Emotional expression
- Character-specific animation profiles

## Conversation Analysis Module

The Conversation Analysis Module performs detailed analysis after or during conversations.

It must support:

- Transcript analysis
- Grammar analysis
- Vocabulary analysis
- Pronunciation analysis
- Dialect analysis
- Speaking-time analysis
- Speech-speed analysis
- Turn-taking analysis
- Interruption analysis
- Question analysis
- Follow-up analysis
- Topic analysis
- Self-reference analysis
- Reciprocity analysis
- Manners analysis
- Gratitude analysis
- Emotional-response analysis
- Conversational-pacing analysis

## Adaptive Learning Module

The Adaptive Learning Module personalizes instruction according to student performance.

It must support:

- Student skill profiles
- Adaptive lesson difficulty
- Adaptive vocabulary
- Adaptive conversation complexity
- Adaptive coaching
- Adaptive pronunciation training
- Adaptive dialect recognition
- Adaptive character behavior
- Adaptive speech speed
- Personalized objectives
- Weakness identification
- Strength identification
- Progress milestones
- Skill progression
- Review scheduling

## Student Progress Module

The Student Progress Module tracks development across language and communication skills.

It must track:

- Language proficiency
- Conversation proficiency
- Listening
- Speaking
- Vocabulary
- Grammar
- Pronunciation
- Dialect comprehension
- Question-asking
- Active listening
- Manners
- Gratitude
- Social awareness
- Conversational pacing
- Speech-speed development
- Confidence
- Reciprocity
- Interruption frequency
- Follow-up-question frequency

## Coaching Mode Module

The Coaching Mode Module allows students to control how much feedback they receive.

Modes should include:

- No coaching
- Post-conversation coaching
- Gentle coaching
- Standard coaching
- Active coaching
- Language-only coaching
- Conversation-only coaching
- Manners-only coaching
- Gratitude-only coaching
- Speech-speed coaching
- Dialect coaching
- Combined coaching
- Custom coaching

## Instructor Mode Module

The Instructor Mode Module provides structured educational experiences.

Modes should include:

- Structured lesson
- Free conversation
- Vocabulary lesson
- Grammar lesson
- Pronunciation lesson
- Listening lesson
- Speech-speed lesson
- Dialect lesson
- Roleplay
- Conversation practice
- Cultural lesson
- Manners lesson
- Gratitude lesson
- Review session
- Assessment session

## Voice Personalization Module

The Voice Personalization Module allows students to customize the AI's spoken presentation.

It should support:

- Voice selection
- Character voice selection
- Accent selection
- Dialect selection
- Speaking speed
- Response timing
- Pitch preferences
- Voice energy
- Formality
- Emotional expressiveness
- Character-specific voice profiles

## Conversation Intelligence Module

The Conversation Intelligence Module maintains contextual understanding during conversations.

It must support:

- Semantic context tracking
- Topic tracking
- Speaker tracking
- Conversation-state tracking
- Intent recognition
- Question recognition
- Answer recognition
- Topic-shift recognition
- Emotional-context recognition
- Social-context recognition
- Conversational-opportunity detection
- Conversational-repair detection
- Speech-speed awareness
- Turn-taking awareness
- Interruption awareness

## Conversation Repair Module

The Conversation Repair Module helps students recover from misunderstandings and awkward moments.

It must support:

- Misunderstanding detection
- Clarification requests
- Miscommunication repair
- Accidental-offense repair
- Apology coaching
- Topic recovery
- Forgotten-thought recovery
- Conversation restart
- Polite correction
- Intent clarification
- Awkward-moment repair
- Pacing adjustment after misunderstanding

## Confidence Module

The Confidence Module provides progressively challenging communication practice.

It should support:

- Low-pressure practice
- Gradual difficulty
- Positive reinforcement
- Mistake normalization
- Repetition
- Guided conversation
- Spontaneous conversation
- Confidence tracking
- Personalized encouragement
- Private practice
- Adjustable speech speed
- Adjustable response timing

## Accessibility Module

The Accessibility Module provides alternative interaction and learning methods.

It should support:

- Voice interaction
- Text interaction
- Captions
- Transcripts
- Adjustable speech rate
- Adjustable response timing
- Keyboard interaction
- Visual feedback
- Audio feedback
- Customizable interface
- Adjustable coaching frequency
- Alternative communication exercises
- Accessible character interfaces
- Visual lip-sync controls

## Privacy Module

The Privacy Module gives students control over voice, conversation, learning, and profile data.

It should support:

- Explicit microphone permissions
- Recording controls
- Recording indicators
- Conversation deletion
- Transcript deletion
- Profile deletion
- Character-memory controls
- Data-retention controls
- Voice-profile deletion
- Student-controlled history
- Data export
- Privacy configuration
- Optional telemetry
- Local-first processing where feasible
- Encryption where supported

## Local-First Module

The Local-First Module enables functionality to operate locally whenever technically feasible.

It should support:

- Local AI models
- Local speech recognition
- Local text-to-speech
- Local conversation analysis
- Local user profiles
- Local conversation history
- Offline language practice
- Offline conversation practice where model capabilities permit
- Optional remote inference
- Local voice processing
- Local lip-sync processing
- Local language resources

## Model Independence Module

The Model Independence Module prevents the system from requiring a single AI provider.

It should support:

- Multiple AI models
- Local models
- Self-hosted models
- Remote models
- Specialized language models
- Specialized speech models
- Model switching
- Model selection
- Model fallback
- Provider abstraction
- Vendor-neutral APIs

## Explainable Coaching Module

The Explainable Coaching Module makes feedback understandable and actionable.

It should provide:

- Specific behavioral examples
- Language explanations
- Manners explanations
- Gratitude explanations
- Cultural explanations
- Conversation explanations
- Speech-speed explanations
- Suggested alternatives
- Before-and-after comparisons
- Feedback confidence indicators
- Student feedback controls

The system should explain what occurred rather than merely assigning a score.

## Non-Diagnostic Behavioral Analysis Module

The system may identify observable communication patterns but must not diagnose personality disorders or other psychological conditions.

Feedback should describe behavior.

Preferred:

"You redirected the conversation toward your own experience several times without asking a follow-up question."

Avoid:

"You are a conversational narcissist."

The module should focus on communication behaviors that the student can understand and practice changing.

## Conversational Ethics Module

The Conversational Ethics Module should reinforce:

- Respect for conversational partners
- Respect for privacy
- Respect for boundaries
- Respect for cultural differences
- Avoidance of manipulation
- Avoidance of deceptive coaching
- Avoidance of personality labeling
- Mutuality
- Curiosity
- Empathy
- Gratitude
- Respectful disagreement
- Appropriate speech pacing
- Appropriate disclosure
- Consent-aware interaction

## Conversation Goals Module

Students should be able to establish communication goals such as:

- Speak more confidently
- Improve pronunciation
- Expand vocabulary
- Improve grammar
- Understand a dialect
- Learn a dialect
- Adjust speaking speed
- Improve speech clarity
- Ask better questions
- Become a better listener
- Interrupt less
- Share more appropriately
- Stop redirecting conversations
- Improve manners
- Become more gracious
- Express gratitude naturally
- Handle difficult conversations
- Become more culturally aware
- Improve professional communication
- Become more socially fluent
- Improve conversational pacing

## Assessment Module

The Assessment Module evaluates language and communication skills.

Assessments may include:

- Vocabulary assessments
- Grammar assessments
- Pronunciation assessments
- Listening assessments
- Speaking assessments
- Dialect comprehension assessments
- Conversation assessments
- Speech-speed assessments
- Active-listening assessments
- Manners assessments
- Gratitude assessments
- Reciprocity assessments
- Cultural communication assessments

Assessments should be configurable and should not reduce communication ability to a single universal score.

---

## Optional Plugin Modules

PassTheMic should support optional plugins that extend functionality without modifying the core architecture.

Optional plugins may include:

- Additional language modules
- Additional dialect modules
- Additional accent modules
- Speech-recognition engines
- Text-to-speech engines
- Translation engines
- Grammar engines
- Pronunciation engines
- Vocabulary databases
- Language databases
- Cultural databases
- Transcription engines
- Voice-analysis engines
- Lip-sync engines
- Avatar engines
- Facial-animation engines
- AI model providers
- Local AI models
- Cloud AI providers
- Learning-management systems
- Teacher-review systems
- Human conversation partners
- Progress dashboards
- Character libraries
- Scenario libraries
- Educational content providers
- Accessibility tools
- External authentication systems
- Optional analytics systems

Plugins must use defined interfaces and must not compromise core privacy, security, interoperability, or user-control requirements.

## Character Plugin Module

Optional character plugins may introduce additional AI instructors and coaches.

Character plugins may define:

- Character identity
- Personality
- Voice
- Accent
- Dialect
- Teaching methodology
- Coaching methodology
- Speaking speed
- Formality
- Emotional style
- Questioning style
- Correction style
- Roleplay capabilities
- Cultural specialization

Characters should remain replaceable without changing core learning data.

## Human Teacher Plugin Module

An optional Human Teacher Plugin may allow students to connect with human instructors.

It may support:

- Teacher review
- Assignment review
- Conversation review
- Progress review
- Feedback
- Lesson creation
- Custom exercises
- Teacher-selected characters
- Teacher-selected coaching goals

AI coaching and human instruction should remain separable.

## Human Conversation Partner Plugin

An optional Human Conversation Partner Plugin may allow students to practice with other people.

It may support:

- Language exchange
- Conversation matching
- Scheduled conversations
- Conversation preferences
- Language-level matching
- Dialect preferences
- Conversation goals
- Safety controls
- Reporting
- Blocking
- Privacy controls

## Optional Translation Plugin

The Translation Plugin may provide:

- Text translation
- Speech translation
- Real-time translation
- Phrase translation
- Context-aware translation
- Dialect-aware translation
- Idiom explanation
- Translation alternatives
- Formality-aware translation

## Optional Avatar Plugin

The Avatar Plugin may provide visual AI characters.

It may support:

- Animated characters
- Facial expressions
- Lip synchronization
- Eye movement
- Head movement
- Gesture animation
- Emotion visualization
- Character-specific animation
- Real-time animation
- Offline animation

## Optional Analytics Plugin

The Analytics Plugin may provide additional learning analytics.

It may support:

- Advanced progress analytics
- Skill trends
- Conversation trends
- Speech-speed trends
- Vocabulary trends
- Pronunciation trends
- Listening trends
- Reciprocity trends
- Manners trends
- Gratitude trends

Analytics must remain optional and subject to user privacy controls.

## Security Module

The Security Module should protect the system and user data.

It should support:

- Authentication
- Authorization
- Permission controls
- Secure storage
- Secure communication
- Plugin permissions
- Model permissions
- Microphone permissions
- Data-access controls
- Session security
- Audit logging where appropriate
- Secure deletion
- Privacy-preserving defaults

## Configuration Module

Students should be able to configure:

- Preferred language
- Target dialect
- Target accent
- AI character
- AI voice
- Speech speed
- Response timing
- Coaching intensity
- Learning difficulty
- Conversation difficulty
- Correction style
- Lesson style
- Privacy settings
- Recording settings
- Data retention
- Accessibility settings
- Character preferences
- Progress tracking

## Core Conversational Philosophy

PassTheMic must reinforce the principle:

**Better Words. Better Manners. Better Conversations.**

The system should teach that effective communication is more than grammatical correctness.

Effective communication includes:

- Curiosity
- Attention
- Listening
- Reciprocity
- Respect
- Courtesy
- Gratitude
- Timing
- Context
- Cultural awareness
- Emotional awareness
- Appropriate self-disclosure
- Appropriate speech speed
- Knowing when to speak
- Knowing when to listen
- Knowing when to slow down
- Knowing when to ask a question
- Knowing when to pass the mic

## Core Outcome

PassTheMic should help students become:

- More fluent speakers
- Better listeners
- More thoughtful conversationalists
- More culturally aware communicators
- More polite participants
- More gracious communicators
- More adaptable speakers
- More confident conversationalists

The system's ultimate objective is not simply to teach students what words to use.

It is to teach students how to use language to **communicate, connect, listen, respect, appreciate, adapt, and participate in meaningful conversations.**

## Open Source and Modular Extensibility

PassTheMic is designed as an open source specification under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.

The architecture must allow additional modules, characters, languages, dialects, voices, learning systems, coaching methodologies, animation systems, and integrations to be added without requiring changes to the fundamental core.

The system should prioritize:

- Modularity
- Interoperability
- Local-first operation
- User control
- Model independence
- Vendor neutrality
- Configurability
- Accessibility
- Privacy
- Explainability
- Human-in-the-loop control

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
  - [https://roxanneardary.com/passthemic/](https://roxanneardary.com/passthemic/)  

---

## License & Notice Requirements

PassTheMic is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to any Open Arsenal project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.
- PassTheMic specifications are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.
