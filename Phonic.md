# Phonic

## AI for Every Call.

Phonic is an open-source AI-powered call interception, screening, and intelligence system designed to protect users from robocalls, enhance voicemail handling, and provide full visibility into all phone communications.

It acts as an intelligent communication layer between the phone network and the user.

---

## 🚀 Core Features

### 📞 Call Interception
- Intercepts all incoming calls before they reach the user
- Routes calls through AI-based decision engine
- Supports SIP/VoIP providers and telephony systems

### 🚫 Robocall Detection & Blocking
- Machine learning-based spam detection
- Audio pattern recognition for prerecorded messages
- Behavioral analysis (response timing, silence detection)
- Dynamic reputation scoring system for phone numbers
- Global + local blocklists

### 🗣️ Voicemail Recording & Transcription
- Automatic voicemail capture
- High-accuracy speech-to-text (Whisper, Vosk, or cloud STT)
- Searchable transcript history
- Audio + text storage pairing

### 📊 Call Logging System
- Full inbound and outbound call history
- Caller ID tracking
- Call classification results (safe, spam, unknown)
- Timestamped records with duration and metadata
- Export support (JSON, CSV)

### 🔔 Notifications & Alerts
- Real-time SMS/email/push notifications
- Alerts for:
  - blocked calls
  - missed calls
  - voicemail received
  - high-risk spam detection

### 🚨 Automated Reporting Engine
- Sends robocall reports to regulatory bodies (where supported)
- Spam number intelligence aggregation
- Optional community-based reporting network

---

## 🧠 AI Intelligence Layer

### Conversational Call Screening
- AI answers unknown callers
- Collects intent before forwarding
- Example:
  - “Who are you trying to reach?”
  - “What is the purpose of your call?”

### Intent & Sentiment Analysis
- Detects urgency of calls and messages
- Identifies phishing/spam intent patterns
- Classifies caller behavior

### Call Summarization
- Automatic summaries of voicemails
- Key points extraction
- Urgency scoring system

### Adaptive Learning System
- Learns from user feedback:
  - mark as spam → improves detection model
  - mark as safe → strengthens whitelist
- Personalized AI filtering per user

---

## 🧱 Full Feature List

### Core System
- Call interception engine
- SIP/VoIP integration layer
- AI routing decision engine
- Real-time audio processing pipeline

### AI / ML Features
- Robocall classification model
- Voice fingerprint detection
- Speech-to-text transcription engine
- Sentiment + urgency scoring
- Adaptive learning feedback loop

### Communication Features
- Voicemail system
- AI call screening assistant
- Call forwarding rules
- Notification system (SMS/email/push)

### Data & Logging
- Call history database
- Voicemail storage system
- Audit logs for AI decisions
- Exportable datasets

### Security & Privacy
- End-to-end encryption for stored audio
- TLS for all communication
- Local-first deployment option
- No external dependency mode

### Platform Features
- Web dashboard (React + Tailwind)
- REST API backend (FastAPI/Node.js)
- Docker deployment support
- Kubernetes-ready architecture

### Reporting & Intelligence
- Spam number tracking
- Automated robocall reporting system
- Community intelligence sharing (optional)
- Reputation scoring network

---

## 🧰 Tech Stack

### Telephony Layer
- Asterisk
- FreeSWITCH
- Twilio Programmable Voice

### AI / Machine Learning
- PyTorch
- TensorFlow
- Hugging Face Transformers

### Speech Processing
- OpenAI Whisper
- Vosk
- Google Cloud Speech-to-Text

### Backend
- Python (FastAPI)
- Node.js (API gateway/services)

### Database
- PostgreSQL (structured logs)
- MongoDB (flexible call/AI metadata)

### Frontend
- React
- TailwindCSS

### Infrastructure
- Docker
- Kubernetes (scaling)
- Event-driven messaging (Kafka / RabbitMQ optional)

---

## 🌍 Future Vision

Phonic is designed to evolve into:

- A global AI call firewall network
- A decentralized spam intelligence graph
- A fully autonomous AI call assistant
- A privacy-first communications operating layer

---

## 📦 Installation (MVP Concept)

(Implementation will vary by deployment model)

- Clone repository
- Install backend dependencies (Python/Node)
- Configure telephony provider (Asterisk/Twilio)
- Deploy AI services (Docker recommended)
- Launch web dashboard

---

## 🤝 Contributing

We welcome contributions across AI, telephony systems, backend infrastructure, and UI/UX.

Please see `CONTRIBUTING.md` for guidelines.

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
  - [https://roxanneardary.com/phonic/](https://roxanneardary.com/phonic/)

---

## License & Notice Requirements

Phonic is released under the **GNU Affero General Public License v3.0 or later (AGPL-3.0+)**.   
By contributing to this project, you agree that your contributions will also be released under this license.

Please note the following:

- All contributions must comply with the **AGPL-3.0+** terms.  
- Under **Section 7** of the license, all redistributions, forks, and derivative works must preserve attribution to:  
  **Roxanne Ardary** and **[roxanneardary.com](https://www.roxanneardary.com/)**.  
- Phonic specificiations are free to use with attribution. A Specification Branding License can be negotiated upon request.
- The project's **notice.md** file tracks attribution requirements and contributor acknowledgments.   
  Any update that adds new contributors or modifies attribution should also update `notice.md`. 
- When submitting a pull request, ensure that any new files maintain the attribution headers where applicable.
- Network-deployed versions of this software must also remain fully AGPL-3.0+ compliant, including exposure of source code modifications when applicable under the license.

For full legal details, please refer to the AGPL-3.0+ license and the project's `notice.md` file.  
