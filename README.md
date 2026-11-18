best models for TTA ATT and understadning..

If you mean TTA (Text-to-Audio), ATT (Audio-to-Text), and Audio Understanding, here are my recommendations for November 2026.
1. Best models by task
Task	Best models	Recommendation
Text-to-Audio (TTA)	Eleven v4, Qwen Audio TTS, Cartesia Sonic	Eleven v4
Audio-to-Text (ATT/ASR)	Qwen3-ASR, NVIDIA Nemotron, Whisper	Qwen3-ASR
Audio Understanding	Gemini, Step-Audio-R1, Voxtral	Gemini / Step-Audio
Real-time Audio	NVIDIA Nemotron, Gemini	Depends on latency
Multilingual Audio	Qwen3-ASR, Whisper	Qwen3-ASR

TrustTheBench+3
2. My top recommendations
Text-to-Audio

    Eleven v4: Natural, expressive speech.
    Qwen Audio TTS: Strong speech generation.
    Cartesia Sonic: Excellent for real-time voice applications.

Audio-to-Text

    Qwen3-ASR: Excellent multilingual transcription.
    NVIDIA Nemotron: Fast transcription.
    Whisper Large-v3: Strong multilingual baseline.

Audio Understanding

    Gemini: General audio comprehension and reasoning.
    Step-Audio-R1: Advanced audio reasoning.
    Voxtral: Transcription, summarization, and audio-based question answering.

DataCamp+2
3. One clarification

When you say TTA and ATT, do you mean:

    TTA: Text-to-Audio generation.
    ATT: Audio-to-Text transcription.
    Audio Understanding: Understanding conversations, speakers, emotions, sounds, context, and meaning.

Or are you referring to Text-to-Audio, Audio-to-Text, and Text Understanding (LLMs)?

I can then give you a proper top-10 ranking, including open-source models, commercial APIs, accuracy, latency, and cost.
Sources

Text-to-Audio (TTA)	Eleven v4, Qwen Audio TTS, Cartesia Sonic	Eleven v4 what about whisp[er from openai?

Good question! OpenAI Whisper is excellent, but it is NOT a Text-to-Audio (TTA) model. It is primarily an Audio-to-Text (ATT/ASR) model.

OpenAI has separate models for speech generation.
OpenAI audio models: What's the difference?
Model	Function	Best use
Whisper	Audio → Text	Speech transcription
GPT-4o mini TTS	Text → Audio	Speech generation
TTS-1-HD	Text → Audio	High-quality speech
TTS-1	Text → Audio	Low-latency speech
GPT Realtime	Audio ↔ Audio	Real-time voice interaction

OpenAI Developers+2
My recommendations
For Text-to-Audio

    ElevenLabs
    Cartesia Sonic
    OpenAI GPT-4o mini TTS
    Qwen Audio TTS

For Audio-to-Text

    OpenAI GPT Transcribe
    Whisper
    Qwen3-ASR
    NVIDIA Nemotron

One important update: OpenAI's current documentation recommends migrating existing TTS integrations toward its Realtime API model, gpt-realtime-2.1-mini. The older TTS models are scheduled for shutdown on January 6, 2027. OpenAI Developers+1

Official resources:

    OpenAI Whisper on GitHub
    OpenAI Text-to-Speech documentation

My advice: Don't compare Whisper against ElevenLabs for TTA. Compare Whisper against other transcription models, and ElevenLabs against other speech-generation models. They solve different problems.
Sources
This might also interest you.
Learn more
LangChain
LLM Eval Platform for AI Agents
Offline + online evals. LLM-as-judge + human feedback. Catch regressions before users do.
Ad

Task	Best models	Recommendation
Text-to-Audio (TTA)	Eleven v4, Qwen Audio TTS, Cartesia Sonic	Eleven v4
Audio-to-Text (ATT/ASR)	Qwen3-ASR, NVIDIA Nemotron, Whisper	Qwen3-ASR
Audio Understanding	Gemini, Step-Audio-R1, Voxtral	Gemini / Step-Audio
Real-time Audio	NVIDIA Nemotron, Gemini	Depends on latency
Multilingual Audio	Qwen3-ASR, Whisper	Qwen3-ASR are these recommendation free?

Not all of them! Some are completely free and open-source, while others offer free credits or limited free tiers.

Here is a breakdown.
1. Free vs Paid AI Audio Models
Model	Free?	How to use
Eleven v4	✅ Limited free	Free monthly credits
Qwen Audio TTS	⚠️ Depends	API credits or self-hosting alternatives
Cartesia Sonic	✅ Limited free	20K monthly credits
Qwen3-ASR	⚠️ Limited free	API quota; self-hosting options
NVIDIA Nemotron	✅ Open models available	Local deployment
Whisper	✅ Completely free	Run locally
Gemini Audio	⚠️ Limited free	Gemini API free tier, model-dependent
Step-Audio-R1	✅ Open-source availability	Local deployment
Voxtral	✅ Open-weight models available	Local deployment
2. Best Completely Free Options

If you don't want to spend money, I'd prioritize these:
Task	Recommended free model
Text-to-Audio	Qwen3-TTS
Audio-to-Text	Whisper
Audio Understanding	Step-Audio
Real-time Audio	Qwen Audio
Multilingual Audio	Whisper / Qwen3-ASR
3. Official Downloads and Platforms

    Whisper: OpenAI Whisper GitHub
    Qwen: Qwen GitHub
    NVIDIA: NVIDIA NeMo
    Step-Audio: StepFun GitHub
    Voxtral: Mistral AI
    ElevenLabs: Pricing
    Cartesia: Pricing

4. My Recommendation

If your goal is to build an AI audio system without paying for API calls, I'd choose:

    TTA: Qwen3-TTS
    ATT: Whisper Large-v3
    Audio Understanding: Step-Audio
    Multilingual transcription: Qwen3-ASR
    Real-time processing: A locally deployed streaming model.

Important: Open-source doesn't always mean free to operate. Running models locally requires hardware, and API providers may charge even when the underlying model weights are freely available.

I can also put together a list of the **10 best completely free, open-source audio AI models that you can run locally without API costs**.
For production voice agents in latency-sensitive calls, here’s one voice API option.
Learn more
Vapi
The Voice API Built for Production, Not Demos
<500ms latency. 200+ model integrations. Bring your own stack. 750K+ developers already building.
Ad

Yeha i need the entie stack for free and it must be commercial-use open

Absolutely. In that case, I'd build your stack around self-hosted, open-source AI models with commercial-use permissions.

Your requirements should be:

    100% free model weights.
    Commercial use permitted.
    Open-source code and preferably permissively licensed weights.
    No paid API dependencies.
    Run locally or on your own server.
    No usage limits or monthly credit restrictions.
    Ability to modify and redistribute where the license permits.

One important distinction: free to use commercially is not necessarily the same as open-source. I'll prioritize Apache 2.0 and MIT licenses rather than models with restrictive research-only or custom licenses.
Recommended free commercial AI audio stack
Task	My recommended model	License	Commercial use
Text-to-Audio (TTS)	Qwen3-TTS 1.7B	Apache 2.0	✅
Audio-to-Text (ASR)	Qwen3-ASR	Apache 2.0	✅
Alternative ASR	Whisper Large-v3	MIT	✅
Audio Understanding	Qwen2.5-Omni	Apache 2.0	✅
Real-time Audio	Qwen2.5-Omni	Apache 2.0	✅
Multilingual Audio	Qwen3-ASR	Apache 2.0	✅
General LLM / Reasoning	Qwen3	Apache 2.0	✅

The official repositories provide the relevant licenses: Qwen3-TTS, Qwen3-ASR, Whisper, Qwen2.5-Omni and Qwen3.

These are permissive model licenses, not guarantees that every associated dependency, dataset or voice recording has identical licensing.
2. Additional components for a complete stack

You will also need supporting technologies.
Component	Recommended software	Purpose
Model serving	vLLM	Serve models
Model framework	Hugging Face Transformers	Load models
Audio processing	FFmpeg	Convert audio
API backend	FastAPI	Build endpoints
Voice activity detection	Silero VAD	Detect speech
Speaker diarization	Research pyannote alternatives individually for commercial licensing	Identify speakers
Interface	Gradio	Web interface
Containerization	Docker	Deployment

Check individual dependency licenses before commercial distribution.
3. Download the models

Here are the official repositories:

Text-to-Audio

    Qwen3-TTS GitHub

Audio-to-Text

    Qwen3-ASR GitHub
    Whisper GitHub

Audio Understanding

    Qwen2.5-Omni GitHub

Reasoning

    Qwen3 GitHub

4. Important: What does completely free actually mean?

You can have:

    No API subscriptions.
    No per-request charges.
    No monthly usage limits.
    No model licensing fees.
    Commercial deployment rights under the applicable licenses.
    Complete control over your data.

However, you still need computing hardware, electricity and storage.
5. Let's build the right stack

I need one important detail before recommending model sizes and deployment architecture.

Where do you intend to run these models?

    Local PC: Windows/Linux, NVIDIA GPU.
    Mac: Apple Silicon (M1/M2/M3/M4).
    Own cloud server: Self-hosted GPU server.
    CPU only: No dedicated GPU.
    Not decided: Recommend the most economical setup.

I can then put together a complete architecture with commercially usable open models, installation commands, model sizes, hardware requirements and a unified API—without depending on paid AI services.
This might also interest you.
Learn more
Go.AI, On-Premises AI for Regulated Industries
Private AI On-Prem
Deploy secure AI in your own environment.
Ad

would this work as a lets say rbuisness recepcionist ?

Yes! Absolutely. You could build a fully functional AI business receptionist using this stack, without paying per-minute AI or API fees.

In fact, this is a very realistic application for these models.

I'd design it as an AI receptionist that answers phone calls, talks naturally, understands customers, books appointments, answers business questions, and transfers calls to humans.
1. What your AI receptionist could do

Imagine someone calls a dental clinic:

Customer: Hi, I'd like to schedule an appointment.

AI Receptionist: Of course! Are you looking for a new patient appointment or a routine checkup?

Customer: A routine checkup.

AI Receptionist: Absolutely. What day works best for you?

Customer: Thursday afternoon.

AI Receptionist: Let me check availability. I have 2:30 PM and 4:00 PM available. Which works better?

Customer: 2:30.

AI Receptionist: Perfect. Can I get your name and phone number?

The AI then:

    Checks the appointment calendar.
    Books the appointment.
    Saves customer information.
    Sends a confirmation.
    Updates the business CRM.

All automatically.
2. The complete AI receptionist architecture

Here is the stack I'd build.
Component	Technology	Purpose
Speech-to-Text	Qwen3-ASR	Understand callers
Text-to-Speech	Qwen3-TTS	Speak naturally
AI Brain	Qwen3	Understand and respond
Audio Understanding	Qwen2.5-Omni	Understand complex audio
Voice Detection	Silero VAD	Detect when someone speaks
Backend	Python + FastAPI	Manage conversations
Database	PostgreSQL	Store customer information
Memory	Redis	Maintain conversation state
Calendar	CalDAV / custom integration	Schedule appointments
Dashboard	React	Business management
Deployment	Docker	Run everything

The core models have permissive licenses, including Apache 2.0 for the cited Qwen3-TTS and Qwen3-ASR releases. GitHub+1
3. How the system works
text

          CUSTOMER CALLS
                 |
                 v
          PHONE SYSTEM
                 |
                 v
          AUDIO PROCESSING
                 |
                 v
             QWEN3-ASR
          (Speech to Text)
                 |
                 v
             AI BRAIN
              QWEN3
                 |
          +------+------+
          |      |      |
          v      v      v
        CRM   Calendar  Business
              Booking   Knowledge
          |      |      |
          +------+------+
                 |
                 v
             QWEN3-TTS
          (Text to Speech)
                 |
                 v
          CUSTOMER HEARS AI

The system can also transfer calls to a real employee when necessary.
4. Features you could sell to businesses

I'd build these features into the product:
Feature	Description
24/7 Receptionist	Answers calls anytime
Appointment Booking	Books appointments automatically
FAQ Assistant	Answers business questions
Lead Capture	Collects potential customer details
Call Transfer	Transfers to employees
Missed Call Recovery	Follows up with missed callers
Multilingual Support	Handles multiple languages
Call Summaries	Summarizes every conversation
CRM Integration	Stores customer interactions
Business Dashboard	Shows calls, bookings and leads
5. One important issue: Phone calls

Your AI models can be completely free, but connecting them to the traditional telephone network is different.

You generally need:

    A phone number.
    SIP connectivity or a telephone provider.
    A server with sufficient processing power.
    Internet connectivity.

Telephone providers generally charge for numbers and calls.

You can eliminate AI API fees, but you cannot realistically guarantee zero operating costs for conventional telephone calls.

For a completely self-hosted approach, investigate:

    Asterisk — Open-source telephone system.
    FreeSWITCH — Open-source communications platform.
    LiveKit — Real-time audio infrastructure.

6. Hardware recommendations

For a production receptionist, I'd recommend:
Hardware	Suitability
CPU only	Testing, not ideal for multiple calls
NVIDIA GPU 12GB	Small-scale experimentation
NVIDIA GPU 24GB	More practical for a small deployment
NVIDIA GPU 48GB+	More room for concurrent calls and larger models

Actual capacity depends heavily on model sizes, quantization, streaming implementation and simultaneous callers.
7. My recommendation: Build it as a SaaS

Rather than building a receptionist for just one business, build a platform where businesses can subscribe.

For example:

AI Receptionist Dashboard

    Business name and profile.
    Business opening hours.
    Services and pricing.
    Appointment availability.
    AI receptionist personality.
    Call history.
    Customer information.
    Appointment management.
    Human call-transfer settings.

Each business gets its own AI receptionist and isolated customer data.

You could eventually sell this to:

    Dental clinics.
    Medical offices.
    Restaurants.
    Hair salons.
    Auto repair shops.
    Real estate agencies.
    Hotels.
    Law firms.

For healthcare and legal customers, you'd need additional privacy, security and regulatory safeguards before deployment.
8. Three things I'd like to establish before designing it

    Phone calls: Do you want customers to call a real telephone number and speak with the AI, just like a human receptionist?
    Business model: Do you want to build one receptionist for your own business, or a SaaS platform where hundreds of businesses can create their own AI receptionists?
    Infrastructure: Do you want everything running on your own server, with no external AI APIs whatsoever?

My recommendation: Build a multi-business SaaS platform with a completely self-hosted AI engine. That gives you control over the models, customer data, operating costs and product.
Sources

Asterisk — Open-source telephone system.
FreeSWITCH — Open-source communications platform.
LiveKit — Real-time audio infrastructure. what are these for

These three technologies handle the telephone and real-time communication side of your AI receptionist. They aren't AI models themselves. They make it possible for your AI to communicate with customers over phone calls.

Think of them as the connection between a customer's telephone and your AI brain.
1. What each one does
1. Asterisk

Official Asterisk website

Think of Asterisk as your virtual telephone receptionist infrastructure.

It handles:

    Incoming and outgoing telephone calls.
    Phone extensions.
    Call routing.
    Call transfers to human employees.
    Interactive voice response (IVR).
    SIP telephone connections.
    Voicemail.

Example:

A customer calls your business number. Asterisk receives the call and routes its audio to your AI receptionist.

If the customer asks to speak to an employee, Asterisk can transfer the call.
2. FreeSWITCH

Official FreeSWITCH website

Think of FreeSWITCH as a powerful telephone and media-processing engine.

It handles:

    SIP calls.
    Audio streams.
    Call routing.
    Conference calls.
    Call recording.
    Audio transcoding.
    Multiple simultaneous calls.

It is particularly useful for building larger communication platforms.
3. LiveKit

Official LiveKit website

Think of LiveKit as the real-time audio connection between people and AI.

It handles:

    Real-time audio streaming.
    Two-way audio communication.
    Low-latency voice transmission.
    Interruptions and turn-taking.
    Multiple participants.
    AI voice agents.

For example, when a customer interrupts your AI receptionist mid-sentence, a properly implemented voice pipeline can stop the AI's speech and listen to the customer.
2. What's the difference?
Capability	Asterisk	FreeSWITCH	LiveKit
Traditional phone calls	✅	✅	Via SIP
SIP support	✅	✅	✅
Audio streaming	✅	✅	✅
Call transfers	✅	✅	Via integration
AI voice agents	Via integration	Via integration	✅
Real-time conversations	✅	✅	✅
WebRTC	Via integration	Via integration	✅
3. Which ones should you use?

For your AI receptionist project, I would start with:

Asterisk + LiveKit + your self-hosted AI models.

The architecture would look like this:
text

       CUSTOMER PHONE
              |
              v
         ASTERISK
       (Phone System)
              |
              v
          LIVEKIT
      (Audio Streaming)
              |
              v
       AI RECEPTIONIST
              |
       +------+------+
       |      |      |
       v      v      v
      ASR     LLM    TTS
       |      |      |
       +------+------+
              |
              v
       CUSTOMER PHONE

You don't necessarily need FreeSWITCH as well. Asterisk and FreeSWITCH overlap considerably.
4. What about costs?
Technology	Self-hosted software cost
Asterisk	Free
FreeSWITCH	Free
LiveKit open-source server	Free
Qwen models	Free under applicable licenses
PostgreSQL	Free
Redis	Free
Docker	Free

You still pay for infrastructure, electricity and potentially telephone connectivity.
5. My recommendation

For your project, I'd use:

    Asterisk: Telephone infrastructure.
    LiveKit: Real-time audio communication.
    Qwen3-ASR: Speech recognition.
    Qwen3: AI reasoning and conversation.
    Qwen3-TTS: Voice generation.
    FastAPI: Backend orchestration.
    PostgreSQL: Business and customer data.

This gives you the foundation for a self-hosted AI receptionist SaaS.

One particularly important design decision: Make sure the AI can listen while speaking, detect interruptions, respond quickly and transfer calls to humans. Those capabilities will make the difference between a frustrating voice bot and a convincing virtual receptionist.
For receptionist and call-handling, here's an AI phone system option.
Learn more
RingCentral
RingEX
AI-powered voice. Outpace the pack, every call.
Ad

cool, lets build the entire workgflow and logic infractureswithouth phone plans at fierst themn later on we can add phones.. since this will add cost and im broke

Absolutely. And I actually think that's the smartest way to approach this.

We will build the entire AI receptionist platform first, without purchasing phone numbers, telephone subscriptions, paid APIs, or cloud AI services.

We'll develop it so that when you're ready to spend money on telephone connectivity, we can plug it in without rebuilding the application.

For now, we'll use your computer's microphone and speakers to simulate a real customer phone call.

The goal is to build something that could eventually become a commercial SaaS product.
1. Our project: Self-hosted AI Receptionist

Let's call it OpenReceptionist for now.

The system will have four major parts:

    AI engine — understands and responds to customers.
    Voice engine — listens and speaks.
    Business engine — handles bookings, FAQs, customers and business rules.
    Management dashboard — lets businesses configure their receptionist.

Everything will communicate through our own backend.
2. Complete architecture

Here is the architecture I recommend:
text

                 OPENRECEPTIONIST
                  SYSTEM PLATFORM
                         |
          +--------------+--------------+
          |              |              |
          v              v              v
      AI ENGINE      BUSINESS ENGINE   DASHBOARD
          |              |              |
     +----+----+     +---+------+    +---+------+
     |    |    |     |          |    |          |
     ASR  LLM  TTS  Booking    CRM  Settings  Analytics
     |    |    |     |          |    |          |
     +----+----+     +----------+    +----------+
          |
          v
     VOICE ENGINE
          |
     Browser Microphone
     Browser Speakers
          |
          v
       CUSTOMER

Eventually, we'll add:
text

CUSTOMER PHONE
      |
      v
ASTERISK / SIP
      |
      v
LIVEKIT
      |
      v
OPENRECEPTIONIST

The important thing is that the AI receptionist itself won't depend on Asterisk or LiveKit. We'll create an interchangeable communication layer.

That means we can add telephone support later.
3. Technology stack

These are my proposed choices.
Layer	Technology	Why
Frontend	React	Receptionist dashboard
Backend	Python + FastAPI	Application logic
Database	PostgreSQL	Persistent business data
Cache	Redis	Sessions and temporary state
Speech recognition	Whisper	Reliable local transcription
Alternative ASR	Qwen3-ASR	Multilingual transcription
AI brain	Qwen3	Conversation and reasoning
Voice generation	Qwen3-TTS	Natural speech
Voice activity detection	Silero VAD	Detect speech and silence
Audio processing	FFmpeg	Audio conversion
Real-time connection	WebSockets	Stream audio
Deployment	Docker Compose	Run everything locally

We'll keep the AI models replaceable.

For example, if we discover a better TTS model, we should be able to replace Qwen3-TTS without rewriting the booking system.
4. The most important part: The receptionist's brain

We shouldn't simply send every customer message to an LLM and hope it behaves correctly.

We need a structured conversation engine.

I'd divide it into six components.
A. Conversation Manager

Maintains:

    Current conversation.
    Customer identity.
    Conversation history.
    Current task.
    Conversation stage.
    Language.
    Whether the customer wants a human.

Example:
json

{
  "session_id": "session_001",
  "customer_name": null,
  "intent": "book_appointment",
  "conversation_stage": "collecting_information",
  "language": "en",
  "human_requested": false
}

B. Intent Recognition

The AI must understand what customers want.

Initial intents:
Intent	Example
Greeting	Hello, good morning
Business hours	When do you close?
Services	What services do you offer?
Pricing	How much does it cost?
Appointment	I'd like to book
Rescheduling	Change my appointment
Cancellation	Cancel my booking
Location	Where are you located?
Human transfer	Can I speak to someone?
Complaint	I have a problem
C. Business Knowledge

Each business gets its own knowledge base.

For example:
json

{
  "business_name": "Example Dental Clinic",
  "opening_hours": {
    "monday": "08:00-17:00",
    "tuesday": "08:00-17:00",
    "wednesday": "08:00-17:00",
    "thursday": "08:00-17:00",
    "friday": "08:00-15:00"
  },
  "services": [
    {
      "name": "Dental Cleaning",
      "duration_minutes": 45,
      "price": 100
    }
  ],
  "timezone": "America/Denver"
}

The AI should only answer business-specific questions using verified business information.

If it doesn't know something, it should admit that rather than invent an answer.
D. Booking Engine

This is particularly important.

The AI should never independently invent available appointments.

Instead:

    Customer requests an appointment.
    AI identifies the requested service.
    Backend checks availability.
    AI presents available times.
    Customer chooses.
    Backend validates availability again.
    Backend creates the booking.
    Customer receives confirmation.

The database, not the LLM, controls appointments.
E. Customer Management

We need to save:

    Customer name.
    Phone number (when available).
    Email.
    Previous appointments.
    Conversation history.
    Customer preferences.
    Notes.

F. Escalation Engine

The AI should recognize when it needs human assistance.

Examples:

    Customer explicitly requests an employee.
    AI cannot confidently answer.
    Customer reports an emergency.
    Customer makes a serious complaint.
    A booking operation fails.

During our initial development, escalation can simulate a transfer by displaying a notification in the dashboard.
5. Project folder structure

I want us to organize this properly from the beginning, so we don't end up with a massive, difficult-to-maintain application.

Our initial repository will look like this:
text

open-receptionist/
│
├── frontend/
│   ├── src/
│   │   ├── pages/
│   │   │   ├── Dashboard.jsx
│   │   │   ├── Receptionist.jsx
│   │   │   ├── Customers.jsx
│   │   │   ├── Appointments.jsx
│   │   │   ├── CallHistory.jsx
│   │   │   └── Settings.jsx
│   │   │
│   │   ├── components/
│   │   └── services/
│   │
│   └── package.json
│
├── backend/
│   ├── app/
│   │   ├── main.py
│   │   │
│   │   ├── api/
│   │   │   ├── conversations.py
│   │   │   ├── customers.py
│   │   │   ├── appointments.py
│   │   │   └── businesses.py
│   │   │
│   │   ├── ai/
│   │   │   ├── orchestrator.py
│   │   │   ├── conversation.py
│   │   │   ├── intent.py
│   │   │   ├── prompts.py
│   │   │   └── memory.py
│   │   │
│   │   ├── audio/
│   │   │   ├── asr.py
│   │   │   ├── tts.py
│   │   │   ├── vad.py
│   │   │   └── audio_processor.py
│   │   │
│   │   ├── business/
│   │   │   ├── booking.py
│   │   │   ├── knowledge.py
│   │   │   ├── customer_manager.py
│   │   │   └── escalation.py
│   │   │
│   │   ├── communication/
│   │   │   ├── base.py
│   │   │   ├── browser.py
│   │   │   └── telephony.py
│   │   │
│   │   ├── database/
│   │   └── config/
│   │
│   └── requirements.txt
│
├── models/
│   ├── asr/
│   ├── llm/
│   └── tts/
│
├── infrastructure/
│   ├── docker-compose.yml
│   └── Dockerfiles/
│
├── tests/
│
├── documentation/
│
└── README.md

This separation is important because the AI, business logic, audio processing and telephone infrastructure will all be independent.
6. How an actual conversation will work

Let's design the internal logic.

Suppose a customer says:

"I want to book an appointment for tomorrow."

The workflow:
text

1. Browser captures microphone audio
              |
2. Voice Activity Detection
              |
3. Speech-to-Text (ASR)
              |
4. Conversation Manager
              |
5. Intent Recognition
              |
6. Business Rules Engine
              |
7. AI generates response
              |
8. Text-to-Speech
              |
9. Browser plays generated audio
              |
10. Wait for next customer response

There are some important rules:

    The AI cannot make up appointment availability.
    The AI cannot invent prices.
    The AI cannot claim a booking succeeded until the database confirms it.
    The AI must remember the context of the current conversation.
    The customer must be able to interrupt the AI.
    The AI must recognize when it needs human assistance.

We'll implement these as backend-enforced rules rather than relying exclusively on prompts.
7. Development roadmap

I suggest building this in stages.
Phase	What we build	Result
1	Backend and database	Application foundation
2	Local AI models	Working AI brain
3	Speech recognition	AI understands speech
4	Speech generation	AI speaks
5	Voice conversation	Two-way conversation
6	Business knowledge	Understands individual businesses
7	Booking engine	Books appointments
8	Customer management	CRM functionality
9	Dashboard	Business administration
10	Multi-tenant architecture	Multiple businesses
11	Call simulation and testing	Production preparation
12	Asterisk integration	Real telephone calls later

I would not start with the dashboard. I'd first make sure we can have a natural conversation with the AI. That's the foundation of the entire product.
8. What will cost us money?

For the initial development:
Item	Cost
Python	$0
React	$0
FastAPI	$0
PostgreSQL	$0
Redis	$0
Whisper	$0
Qwen3-ASR	$0
Qwen3-TTS	$0
Qwen3	$0 under applicable model license
Docker	$0
Local browser microphone	$0
API subscriptions	$0

We can download and run the models locally. Their actual performance will depend on your hardware.

For licensing, we'll maintain a dependency and model license register. The official Qwen3-TTS Apache 2.0 license, Qwen3-ASR Apache 2.0 license and Whisper MIT license are good starting points. GitHub+2

We also need to check the individual LLM weight licenses, dependencies, voice assets and datasets before commercial distribution.
9. Let's start building: I need your hardware information

Before installing anything, I need to know what we're working with.

What computer will we use to develop and run OpenReceptionist?

Please tell me:

    Operating system (Windows 10/11, Linux, macOS).
    RAM (8GB, 16GB, 32GB, etc.).
    GPU (NVIDIA, AMD, Apple Silicon, or integrated graphics).
    GPU model and VRAM, if applicable.

You can also send a screenshot of your system specifications.

Our first milestone: Get a locally running AI receptionist that can listen through your microphone, understand what you say, respond intelligently, and speak back to you.

No subscriptions. No API keys. No telephone plans.

We'll build it one component at a time, with the eventual commercial SaaS architecture in mind.
Worked for 17s
Sources
This might also interest you.
Learn more
RingCentral
AI Receptionist (Alt)
AI voice answers 24/7. Turn calls into cash.
Ad

letsw keep it simple... lets build the ai first.. the tta .. att .. brain... first... and also  when you say dashboard what does that m,ean?

Perfect. Let's simplify everything. We won't build the telephone system, CRM, booking engine, or dashboard yet.

First, we'll build the AI itself. Three core components:
1. Our AI system

We need three models working together.
A. TTA — Text-to-Audio (AI speaks)

This converts the AI's written response into a human-sounding voice.

Recommended: Qwen3-TTS

    Open-weight.
    Apache 2.0 licensed.
    Commercial use permitted.
    Multiple voice capabilities.
    Supports multilingual speech generation.

Repository: Qwen3-TTS
B. ATT — Audio-to-Text (AI listens)

This converts your spoken words into text.

Recommended: Whisper Large-v3

    Open source.
    MIT licensed.
    Commercial use permitted.
    Multilingual transcription.
    Can run locally.

Repository: OpenAI Whisper

We can also test Qwen3-ASR as an alternative.

Repository: Qwen3-ASR
C. AI Brain — Understanding and responding

This is the intelligence behind the receptionist.

Recommended: Qwen3

It will:

    Understand customer questions.
    Maintain conversation context.
    Generate intelligent responses.
    Follow receptionist instructions.
    Decide what information it needs.
    Determine when it should ask follow-up questions.

Repository: Qwen3
2. How the three models work together

This is the first thing we're going to build:
text

         YOUR MICROPHONE
                |
                v
         +-------------+
         |   WHISPER   |
         |  AUDIO TEXT |
         +-------------+
                |
                v
         +-------------+
         |   QWEN 3    |
         |  AI BRAIN   |
         +-------------+
                |
                v
          TEXT RESPONSE
                |
                v
         +-------------+
         |  QWEN3-TTS  |
         | TEXT AUDIO  |
         +-------------+
                |
                v
          YOUR SPEAKERS

You'll be able to talk to your computer, and the AI will answer you out loud.

Initially, we'll use a simple listen → understand → respond → speak workflow. Later, we'll add streaming and interruptions to make conversations feel natural.
3. What does Dashboard mean?

A dashboard is simply a graphical interface where you control and monitor your AI system.

Imagine opening a website on your computer.

You see something like:
OpenReceptionist
Section	What it does
AI Settings	Configure the AI brain
Voice Settings	Choose the AI's voice
Speech Recognition	Configure transcription
Conversations	View conversations
Knowledge Base	Give AI business information
Testing	Talk to your AI
System Status	See which models are running

For example, under Voice Settings, you could select different voices.

Under AI Settings, you could change the model or receptionist personality.

But we don't need this yet!

We'll initially interact with the AI through a simple testing interface. Once everything works, we can build the dashboard.
4. Our actual development order

Let's keep the project focused.
Stage	What we build
1	Install and run AI Brain (Qwen3)
2	Install and run Whisper
3	Install and run Qwen3-TTS
4	Connect all three
5	Create microphone input
6	Create speaker output
7	Test complete conversations
8	Improve conversational speed and naturalness

No paid APIs. No subscriptions. No phone plans.
5. Before we install anything

I need just one piece of information:

What computer are you using?

    Windows 11
    Windows 10
    Linux
    macOS

And, if you know them, tell me your:

    RAM (16GB, 32GB, etc.).
    Graphics card (NVIDIA RTX 3060, 4060, 4070, etc.).

This matters because Qwen3, Whisper and Qwen3-TTS can require substantial memory.

Our first goal is simple: build an AI that listens to you, understands you, and talks back to you. Once that works, we have the foundation of our receptionist.

id liek to see the concept of the dashbaord

I can create a visual mockup of the OpenReceptionist dashboard, but image generation requires you to log in first.

Once you're logged in, I can generate a professional SaaS dashboard concept showing the AI receptionist, voice settings, AI models, conversation testing, and system monitoring.
This might also interest you.
Learn more
RingCentral
AI Receptionist (Alt)
AI voice answers 24/7. Turn calls into cash.
Ad

sen dme a link then to see what you are thinking

Here are some dashboard designs you can explore for inspiration:

    Dribbble – AI Dashboard Designs
    Behance – SaaS Dashboard Designs
    Tailwind UI – Dashboard Components
    shadcn/ui – Dashboard Examples

My vision for OpenReceptionist:

A clean, modern dark-themed dashboard with:

    Left sidebar for navigation.
    Large central AI conversation testing area.
    Live microphone status.
    AI brain, TTA and ATT model status.
    Voice selection and configuration.
    Conversation history.
    Performance metrics.

Think of a combination of Linear + modern AI control panel, rather than an old-fashioned business CRM.

half of that is useless lol

😂 Fair enough. Let's cut the fluff.

For now, our dashboard only needs to do four things:

    Chat – Talk to the AI and test its intelligence.
    Voice – Test microphone, speech recognition (ATT), and speech generation (TTA).
    Models – See which models are loaded and switch between them.
    Settings – Configure the AI's personality, instructions, and behavior.

That's it.

No CRM, analytics, customer management, appointment bookings, or unnecessary business features yet.

The goal is an AI development console, not a business management dashboard.

We can build the receptionist features after the AI itself works properly.
This might also interest you.
Learn more
RingCentral
AI Receptionist (Alt)
AI voice answers 24/7. Turn calls into cash.
Ad

lets do that

Let's build it. 🚀

We'll start with OpenReceptionist AI Console, a simple local application with four sections:

    Chat — test the AI brain.
    Voice — test microphone, ATT and TTA.
    Models — manage and switch AI models.
    Settings — configure personality and instructions.

Step 1: Check your computer

Before installing anything, tell me:

    Are you using Windows 10, Windows 11, Linux, or macOS?
    How much RAM do you have?
    Do you have an NVIDIA graphics card? If so, which one?

Step 2: What we'll build

Our first version will look something like this:
text

┌──────────────────────────────────────────────┐
│ OPENRECEPTIONIST                    ● LOCAL  │
├──────────────┬───────────────────────────────┤
│              │                               │
│  CHAT        │       AI CONVERSATION         │
│              │                               │
│  VOICE       │  You: Hello!                  │
│              │                               │
│  MODELS      │  AI: Hello! How can I help?   │
│              │                               │
│  SETTINGS    │                               │
│              │                               │
│              │  [ Type a message... ] [Send] │
│              │                               │
└──────────────┴───────────────────────────────┘

We'll use React for the interface and Python/FastAPI for the backend.

First milestone: Get the AI brain running locally and responding to messages through this interface. Then we'll add listening and speaking.

No subscriptions, no paid APIs, no phone plans. Just local AI.
This might also interest you.
Learn more
JumpCube
AI for Customer Service
Handle recurring questions on web and WhatsApp.
Ad

Ubuntu 24.04.5 LTSNVIDIA NVIDIA_DGX_SparkCortex-X925 × 10 Cortex-A725 × 10128.0 GiB4.1 TB 

# System Details Report
---

## Report details
- **Date generated:**                              2026-11-17 18:22:21

## Hardware Information:
- **Hardware Model:**                              NVIDIA NVIDIA_DGX_Spark
- **Memory:**                                      128.0 GiB
- **Processor:**                                   Cortex-X925 × 10 Cortex-A725 × 10
- **Graphics:**                                    NVIDIA GB10
- **Disk Capacity:**                               4.1 TB

## Software Information:
- **Firmware Version:**                            5.36_0ACUM028
- **OS Name:**                                     Ubuntu 24.04.5 LTS
- **OS Build:**                                    (null)
- **OS Type:**                                     64-bit
- **GNOME Version:**                               46
- **Windowing System:**                            X11
- **Kernel Version:**                              Linux 7.0.0-1019-nvidia

Oh, excellent. You have an NVIDIA DGX Spark. That's a seriously capable machine for this project.

We can build and run the entire AI stack locally on this machine. You have considerably more hardware than we need for the first prototype.
1. Your hardware
Component	Your machine	Assessment
System	Ubuntu 24.04.5	Excellent
GPU	NVIDIA GB10 Grace Blackwell	Excellent
Memory	128 GB unified memory	Excellent
CPU	20 ARM cores	Excellent
Storage	4.1 TB	Plenty
Architecture	ARM64	Important for software compatibility
What this means

    We can run a substantial Qwen language model locally.
    We can run Whisper locally.
    We can run Qwen3-TTS locally.
    We can connect all three without external AI APIs.
    We can eventually support multiple simultaneous conversations, subject to model performance and optimization.

One important detail: the DGX Spark uses unified CPU/GPU memory, rather than a conventional desktop GPU with separate VRAM.

This is a very good foundation for our project.
2. Our development approach

I recommend this setup:
Component	Technology
AI model runner	Ollama
AI brain	Qwen3
ATT	Whisper / Qwen3-ASR
TTA	Qwen3-TTS
Backend	Python + FastAPI
Interface	React

Ollama officially supports the GB10 GPU in the DGX Spark, and NVIDIA provides dedicated deployment guides for this hardware. GitHub+1

Useful resources:

    NVIDIA DGX Spark documentation
    Ollama for DGX Spark
    Qwen3-TTS

3. First step: Check your existing installation

I don't want to mess with your NVIDIA drivers or CUDA installation. Your DGX Spark already comes with an NVIDIA software stack.

Open your Ubuntu terminal and run:
bash

echo "===== SYSTEM ====="
uname -m
lsb_release -a

echo "===== NVIDIA GPU ====="
nvidia-smi

echo "===== CUDA ====="
nvcc --version

echo "===== PYTHON ====="
python3 --version

echo "===== OLLAMA ====="
ollama --version

echo "===== DOCKER ====="
docker --version

Some commands might not be installed; that's perfectly fine.

Paste the output here.

Then we'll do the following:

    Set up Ollama if necessary.
    Download our first Qwen model.
    Run the AI locally.
    Connect it to our OpenReceptionist interface.

We'll get the brain working before touching TTA or ATT.

**One component at a time. No unnecessary installations, no paid services, and no messing up your DGX Spark configuration.**
Worked for 21s
Sources
For infrastructure as code, here’s an IaC platform option.
Learn more
Pulumi Corporation
Next-level IaC for humans and agents.
Ship cloud infrastructure at the speed of AI with languages and tools that stay out of your way.
Ad

"===== NVIDIA GPU ====="
nvidia-smi

echo "===== CUDA ====="
nvcc --version

echo "===== PYTHON ====="
python3 --version

echo "===== OLLAMA ====="
ollama --version

echo "===== DOCKER ====="
docker --version
===== SYSTEM =====
aarch64
No LSB modules are available.
Distributor ID:	Ubuntu
Description:	Ubuntu 24.04.5 LTS
Release:	24.04
Codename:	noble
===== NVIDIA GPU =====
Tue Nov 17 18:27:26 2026       
+-----------------------------------------------------------------------------------------+
| NVIDIA-SMI 580.178.04             Driver Version: 580.178.04     CUDA Version: 13.0     |
+-----------------------------------------+------------------------+----------------------+
| GPU  Name                 Persistence-M | Bus-Id          Disp.A | Volatile Uncorr. ECC |
| Fan  Temp   Perf          Pwr:Usage/Cap |           Memory-Usage | GPU-Util  Compute M. |
|                                         |                        |               MIG M. |
|=========================================+========================+======================|
|   0  NVIDIA GB10                    On  |   0000000F:01:00.0  On |                  N/A |
| N/A   35C    P8              4W /  N/A  | Not Supported          |      0%      Default |
|                                         |                        |                  N/A |
+-----------------------------------------+------------------------+----------------------+

+-----------------------------------------------------------------------------------------+
| Processes:                                                                              |
|  GPU   GI   CI              PID   Type   Process name                        GPU Memory |
|        ID   ID                                                               Usage      |
|=========================================================================================|
|    0   N/A  N/A          525214      G   /usr/lib/xorg/Xorg                      121MiB |
|    0   N/A  N/A          525369      G   /usr/bin/gnome-shell                    157MiB |
|    0   N/A  N/A          526462      G   .../9112/usr/lib/firefox/firefox        425MiB |
|    0   N/A  N/A          626229      G   /usr/bin/gnome-control-center            31MiB |
+-----------------------------------------------------------------------------------------+
===== CUDA =====
nvcc: NVIDIA (R) Cuda compiler driver
Copyright (c) 2005-2025 NVIDIA Corporation
Built on Wed_Aug_20_01:57:39_PM_PDT_2025
Cuda compilation tools, release 13.0, V13.0.88
Build cuda_13.0.r13.0/compiler.36424714_0
===== PYTHON =====
Python 3.12.3
===== OLLAMA =====
ollama version is 0.40.7
===== DOCKER =====
Docker version 29.6.2, build dfc4efb
cse455student@spark-75a3:~$ ^C
cse455student@spark-75a3:~$

Perfect. Your DGX Spark is ready for us to start. We don't need to install CUDA, Python, Docker, or NVIDIA drivers.

A few observations:

    ✅ NVIDIA GB10 detected.
    ✅ CUDA 13.0 installed.
    ✅ Python 3.12 installed.
    ✅ Docker installed.
    ✅ Ollama installed.
    ✅ ARM64 architecture confirmed.

Your Ollama version is 0.40.7. We'll test it before changing or upgrading anything.
Step 1 — Check Ollama

Run these commands:
bash

echo "===== OLLAMA SERVICE ====="
systemctl is-active ollama

echo "===== INSTALLED MODELS ====="
ollama list

echo "===== OLLAMA VERSION ====="
ollama --version

This tells us whether Ollama is running and whether you already have models installed.
Step 2 — Our first AI brain

I'm planning to start with Qwen3 32B.

Why?

    Strong reasoning and conversation abilities.
    Supports tool calling.
    Supports more than 100 languages.
    Apache 2.0 license.
    Approximately 20 GB for the Ollama Q4 model.

Your 128 GB unified memory gives us plenty of room to experiment.

Model details: Qwen3 32B – Ollama Library

Don't download anything yet. First, send me the output from Step 1. I want to make sure we don't overwrite or duplicate anything already installed.

Then we'll get your first local AI conversation working.
Worked for 34s
For setting up private AI on NVIDIA GPUs, here’s a server option.
Learn more
Hivelocity
40% Off GPU Servers for AI
Run private AI on NVIDIA L4 GPUs. Save 40% for 12 months. Code GPU4AI.
Ad

ve
===== INSTALLED MODELS =====
NAME                                                 ID              SIZE      MODIFIED    
ornith-1.5:35b                                       9f3b89b25219    22 GB     2 weeks ago    
qwen3.6:35b-a3b                                      a7eb95c53bcf    22 GB     3 weeks ago    
gpt-oss:20b                                          f38aa0c53da5    13 GB     3 weeks ago    
hf.co/jackrong/Qwopus3.8-27B-Flash-V2-GGUF:Q4_K_M    431d7207fe63    18 GB     3 weeks ago    
qwen3.8:27b                                          aaee06c39dcf    17 GB     3 weeks ago    
embeddinggemma:latest                                85462619ee72    621 MB    3 weeks ago    
gemma4:latest                                        dc35e8d9c606    6.6 GB    3 weeks ago    
gemma4:e4b                                           dc35e8d9c606    6.6 GB    3 weeks ago    
===== OLLAMA VERSION =====
ollama version is 0.40.7

Excellent! You already have a pretty substantial collection of local models. We don't need to download another 20–30 GB model right now.

In fact, I would change our original plan.
1. Let's reuse what you already have

Here is how I'd assign your existing models:
Model	Potential role
qwen3.6:35b-a3b	Primary AI brain
qwen3.8:27b	Alternative AI brain
ornith-1.5:35b	Experimental reasoning
gpt-oss:20b	Alternative reasoning
gemma4:latest	Alternative conversational model
embeddinggemma	Knowledge retrieval / embeddings

We'll benchmark them rather than assume which is best.

My first choice to test is qwen3.6:35b-a3b.

We can use it as the receptionist's brain if it performs well in conversation, instruction following and tool calling.
2. Let's inspect our first candidate

Before changing anything, run:
bash

ollama show qwen3.6:35b-a3b

Then test it:
bash

ollama run qwen3.6:35b-a3b

Once the model loads, paste this:
text

You are a professional business receptionist.

Your job is to welcome customers, understand their needs,
answer questions clearly, and maintain a natural,
friendly conversation.

You work for a dental clinic.

A customer says:
"Hi, I've never visited your clinic before.
Can I book an appointment?"

Respond as the receptionist.
Ask only one question at a time.
Do not invent appointment availability.

Check whether it:

    Sounds natural and professional.
    Understands the receptionist role.
    Asks appropriate follow-up questions.
    Avoids inventing information.

3. One important licensing detail

Some of your installed model names aren't standard official model names. We'll need to identify their original publishers and licenses before selecting them for commercial deployment.

Your gpt-oss:20b is another interesting candidate: its official model license is Apache 2.0. Ollama
4. What I need from you

Send me:

    The output of ollama show qwen3.6:35b-a3b.
    How the receptionist test performs.
    Whether the response is fast or slow.

Our immediate objective is to select the best AI brain from models you already own. No new downloads yet.
Worked for 30s
Sources
For running large models locally, here’s one NVIDIA DGX Spark option.
Learn more
NVIDIA DGX™ Spark
NVIDIA DGX Spark™
An AI supercomputer on Your Desk.
Ad

id like to use the ones we first think of.. only if they are better models

Agreed. We should use the models we originally selected unless an existing model is demonstrably better.

I don't want us settling for an inferior model just because it's already downloaded. Your DGX Spark has enough memory to run our preferred stack.
Our target AI stack
Component	Preferred model	Decision
AI Brain	Qwen3 (best suitable release)	Evaluate against existing models
TTA	Qwen3-TTS 1.7B	Download
ATT	Qwen3-ASR 1.7B	Download
Alternative ATT	Whisper Large-v3	Benchmark
Embeddings	EmbeddingGemma	Already installed

The official Qwen3-TTS and Qwen3-ASR repositories specify Apache 2.0 licensing. GitHub+1

Qwen3-TTS also supports streaming speech generation, which is particularly interesting for our receptionist. GitHub
One thing before downloading

I want to check your existing models against the intended architecture.

Run:
bash

ollama show qwen3.6:35b-a3b
ollama show qwen3.8:27b
ollama show gpt-oss:20b

And:
bash

ollama ps

Send me the results.
What we'll do next

    Select the best brain based on actual performance.
    Install Qwen3-ASR.
    Install Qwen3-TTS.
    Connect all three.
    Build our simple four-section AI Console.

One principle: quality first, zero API costs, commercial-use licensing.

We're building a product, not just experimenting with random models.
Sources

Log in for advice and recommendations tailored to you.
Log in
Sign up for free

Embeddings	EmbeddingGemma what is this ?

Great question! EmbeddingGemma is a model that gives your AI a searchable memory.

It doesn't talk, listen, or generate responses. Its job is to help your AI find relevant information.
1. Simple example

Imagine you're building an AI receptionist for a dental clinic.

You give it this information:

    The clinic opens at 8 AM.
    Dental cleaning costs $100.
    The clinic is closed on Sundays.
    New patients receive an initial consultation.
    The clinic is located at 123 Main Street.

EmbeddingGemma converts these documents into numerical representations called embeddings.

When a customer asks:

"How much does it cost to get my teeth cleaned?"

EmbeddingGemma helps find the relevant information:

"Dental cleaning costs $100."

That information is passed to Qwen3, which generates the actual response.
2. How it fits into our architecture
text

       CUSTOMER
           |
           v
      WHISPER ASR
           |
           v
      CUSTOMER TEXT
           |
           v
      EMBEDDINGGEMMA
           |
           v
      SEARCH KNOWLEDGE
           |
           v
      RELEVANT INFORMATION
           |
           v
         QWEN3
       (AI BRAIN)
           |
           v
      TEXT RESPONSE
           |
           v
       QWEN3-TTS
           |
           v
       CUSTOMER

This approach is called RAG (Retrieval-Augmented Generation).
3. Why is it useful?

EmbeddingGemma allows us to give each business its own knowledge base.

For example:
Business information	AI can retrieve
Services	What services are offered?
Pricing	How much does something cost?
Opening hours	When do you close?
Policies	What's your cancellation policy?
FAQs	Do you accept new customers?
Documents	What does your company offer?

We don't need to retrain Qwen3 every time a business changes its prices or opening hours.

We simply update the knowledge base.
4. Do we need it?

Yes, I recommend keeping it.

You already have embeddinggemma:latest installed, and it's lightweight.

Google describes EmbeddingGemma as a multilingual embedding model designed for semantic search and retrieval. Google AI+1

One licensing note: the original EmbeddingGemma uses Google's Gemma Terms of Use, not Apache 2.0. We should review those terms before commercial deployment.

Official documentation: EmbeddingGemma
Our AI stack now looks like this:
Component	Model	Function
Brain	Qwen3	Thinks and responds
ATT	Qwen3-ASR / Whisper	Listens
TTA	Qwen3-TTS	Speaks
Memory/Search	EmbeddingGemma	Finds relevant business information

Think of it this way: Qwen3 is the brain, EmbeddingGemma is the librarian who finds the right information for the brain.
Sources
For embedding model choices and improvements, here’s a vector search option.
Learn more
Oracle
Fast Similarity Lookups
Embeddings indexed alongside your tables
Ad

Model
    architecture        qwen35moe          
    parameters          35.5B              
    context length      262144             
    embedding length    2048               
    quantization        Q4_K_M             
    requires            0.30.0             
    renderer            qwen3.5            
    parser              qwen3.5            
    template source     renderer_parser    

  Capabilities
    completion     
    vision         
    tools          
    thinking       
        levels     false, true    
        default    true           

  Projector
    architecture        clip       
    parameters          446.57M    
    embedding length    1152       
    dimensions          2048       

  Parameters
    repeat_penalty       1       
    temperature          1       
    top_k                20      
    top_p                0.95    
    draft_num_predict    2       
    min_p                0       
    presence_penalty     1.5     

  License
    Apache License               
    Version 2.0, January 2004    
    ...                          

  Model
    architecture        qwen35             
    parameters          27.3B              
    context length      262144             
    embedding length    5120               
    quantization        Q4_K_M             
    requires            0.32.12            
    renderer            qwen3.8            
    parser              qwen3.5            
    template source     renderer_parser    

  Capabilities
    completion     
    vision         
    tools          
    thinking       
        levels     false, low, medium, xhigh    
        default    medium                       

  Projector
    architecture        clip       
    parameters          460.73M    
    embedding length    1152       
    dimensions          5120       

  Parameters
    min_p                0       
    presence_penalty     0       
    repeat_penalty       1       
    temperature          1       
    top_k                20      
    top_p                0.95    
    draft_num_predict    4       

  License
    Apache License               
    Version 2.0, January 2004    
    ...                          

  Model
    architecture        gpt-oss    
    parameters          20.9B      
    context length      131072     
    embedding length    2880       
    quantization        MXFP4      
    requires            0.30.0     
    template source     harmony    

  Capabilities
    completion     
    tools          
    thinking       
        levels     low, medium, high    
        default    medium               

  Parameters
    temperature    1    

  License
    Apache License               
    Version 2.0, January 2004    
    ...                          

cse455student@spark-75a3:~$ ^[[200~ollama ps
ollama: command not found
cse455student@spark-75a3:~$ ~
bash: /home/cse455student: Is a directory
cse455student@spark-75a3:~$ ollama ps
NAME    ID    SIZE    PROCESSOR    CONTEXT    RUNNER    UNTIL
Worked for 12s

Excellent. This gives us a much clearer picture. And there's good news: you already have two very capable Qwen models, both with Apache 2.0 licenses according to their model metadata.

Let's compare them.
1. Your existing Qwen models
Specification	Qwen3.6 35B-A3B	Qwen3.8 27B
Total parameters	35.5B	27.3B
Architecture	MoE	Qwen35
Quantization	Q4_K_M	Q4_K_M
Context window	262K	262K
Vision	Yes	Yes
Tool calling	Yes	Yes
Thinking	Yes	Yes
License	Apache 2.0	Apache 2.0
My interpretation

Qwen3.6 35B-A3B

    Mixture-of-Experts architecture.
    Approximately 3B active parameters per token, suggested by its A3B designation.
    Potentially efficient inference.
    Interesting candidate for fast conversations.

Qwen3.8 27B

    Larger active computation than a small-active-parameter MoE model.
    Supports configurable reasoning levels.
    Strong candidate for complex instructions and receptionist workflows.

I wouldn't automatically assume the 27B model is smarter. We need to benchmark them.
2. My recommendation

I'd test both, but start with:

Primary candidate: Qwen3.8 27B

Alternative: Qwen3.6 35B-A3B

We should measure:

    Response quality.
    Response speed.
    Instruction following.
    Tool calling.
    Conversation consistency.

For a receptionist, natural and quick responses are more important than producing lengthy reasoning.
3. Let's benchmark them

First, test Qwen3.8:
bash

ollama run qwen3.8:27b

Give it this prompt:
text

You are a professional AI receptionist
for a dental clinic.

Your personality is friendly, professional,
patient and conversational.

A customer says:

"Hi, I want to book an appointment,
but I'm not sure what service I need."

Respond naturally.

Rules:
- Ask one question at a time.
- Keep responses short.
- Never invent prices or availability.
- Don't sound robotic.

Then repeat with:
bash

ollama run qwen3.6:35b-a3b

Use exactly the same prompt.
4. One more important observation

Your ollama ps output is empty.

That's normal if no model is currently running. Ollama hasn't loaded a model into memory yet.

We can monitor resource usage when testing.
5. Our final AI architecture

For now, I'm proposing:
Component	Model
AI Brain	Qwen3.8 or Qwen3.6
Speech-to-Text	Qwen3-ASR
Text-to-Speech	Qwen3-TTS
Knowledge retrieval	Embedding model (evaluate licensing)

Don't download anything yet.

Let's establish which brain performs best first. Then we'll install the dedicated speech models.

Your DGX Spark is powerful enough that we can build a serious local AI receptionist rather than relying on expensive commercial APIs.
For running embeddings and inference, here’s one cloud AI infrastructure option.
Learn more
Oracle
Lower Cost per Token
Efficient OCI infra for inference
Ad

Qwen3.8 or Qwen3.6 si thter ea more up to date one

Qwen3.8 is newer than Qwen3.6. And according to the official Qwen documentation, Qwen3.8 is the newer generation. GitHub+1
Release comparison
Model	Release	Status
Qwen3.6 35B-A3B	April 2026	Older
Qwen3.8 27B	August 2026	Newer
What I'd choose for OpenReceptionist

I'd keep both initially:

    Primary: Qwen3.8 27B — newer generation, strong reasoning and agent capabilities.
    Alternative: Qwen3.6 35B-A3B — potentially faster due to its MoE architecture.

Qwen3.8 introduces improvements in agent execution, complex task completion and reasoning control. GitHub
My recommendation

Let's use Qwen3.8 27B as our initial AI brain.

We don't need to download another model.

One important distinction: newer doesn't automatically mean better for voice conversations. We'll benchmark response quality and latency before making it our permanent choice.

Official repository: Qwen3.8 on GitHub
Sources
For running local AI models, here’s a GPU server option for private inference.
Learn more
Hivelocity
40% Off GPU Servers for AI
Run private AI on NVIDIA L4 GPUs. Save 40% for 12 months. Code GPU4AI.
Ad

so the 2.8 is the latest one? in general not only these two

No. Qwen3.8 is not necessarily the latest AI model overall. It's the latest generation in the Qwen family according to the official repository, but there are newer developments across other AI companies.

As of November 17, 2026, here's what matters:
1. Latest Qwen generation
Generation	Status
Qwen3	Older generation
Qwen3.5	Previous generation
Qwen3.6	Previous generation
Qwen3.8	Latest released generation
Qwen4	Max preview announced; full release not established

The official Qwen repository identifies Qwen3.8 as its latest open model generation. GitHub
2. Other AI model families worth considering

For our receptionist, I'd watch these:

    Qwen — strong open-weight models and tool calling.
    DeepSeek — reasoning and complex tasks.
    Mistral — efficient models and commercial deployment options.
    Gemma — efficient models, but check its specific licensing.
    GPT-OSS — open-weight reasoning models.

3. What I'd recommend for your DGX Spark

Don't chase model version numbers.

We need the best model for:

    Natural conversations.
    Fast responses.
    Following receptionist instructions.
    Tool calling.
    Reliable customer interactions.
    Commercial deployment rights.

My current choice remains Qwen3.8 27B as our starting candidate, but I'd benchmark it against other leading open-weight models before committing.

Official source: Qwen model repository

The important thing is that we choose the best model for the job, not simply the newest model available.
Sources
This might also interest you.
Learn more
NVIDIA DGX™ Spark
NVIDIA DGX Spark™
An AI supercomputer on Your Desk.
Ad

lets do it

Let's do it. We'll benchmark the best candidates for OpenReceptionist and choose based on actual performance, not hype.
1. Models we'll compare

Your DGX Spark has 128 GB unified memory, so we have room to test some substantial models.
Model	Why we're testing it
Qwen3.8 27B	Our current primary candidate
Qwen3.6 35B-A3B	Efficient MoE alternative
GPT-OSS 20B	Strong reasoning alternative
Gemma 4	Alternative model family

We'll also keep an eye on newer DeepSeek and Mistral releases.

Qwen3.8 is the latest generation in the Qwen family according to its official repository. That doesn't make it automatically the best overall model.
2. What matters for our receptionist?

I'll evaluate each model on five criteria:

    Conversation quality: Does it sound like a real receptionist?
    Response speed: Can it respond quickly?
    Instruction following: Does it follow business rules?
    Tool calling: Can it reliably trigger booking and other functions?
    Consistency: Does it maintain context throughout conversations?

For a voice receptionist, I'd prioritize speed and natural conversation over complicated reasoning.
3. First benchmark: Qwen3.8

Let's start with the model you already have.

Run:
bash

ollama run qwen3.8:27b

Then paste this test:
text

You are an AI receptionist for a dental clinic.

Your personality:
- Friendly
- Professional
- Natural
- Helpful
- Concise

A customer says:

"Hi, I've never visited your clinic before.
I have a toothache and would like to come in
as soon as possible. Can you help?"

Instructions:
1. Respond naturally.
2. Ask one question at a time.
3. Identify whether the situation may require urgent attention.
4. Never invent appointment availability.
5. Keep your response under 50 words.
6. Do not sound like a generic chatbot.

Pay attention to how quickly it responds and whether its answer sounds human.

Then repeat the same test with:
bash

ollama run qwen3.6:35b-a3b

And:
bash

ollama run gpt-oss:20b

4. What happens after benchmarking?

We'll select one primary brain and one backup.

Then we'll move to:
Component	Model
AI Brain	Winner of our benchmark
ATT	Qwen3-ASR
TTA	Qwen3-TTS
Embeddings	A commercially suitable embedding model

We'll build the interface around these models.

One rule: we're not downloading anything else until we know what we actually need.

Send me the three model responses and their approximate response times. We'll choose our AI brain together.
Worked for 27s
This might also interest you.
Learn more
Cerebras Systems
Speed Changes What AI Can Do
Meet CS-4. Up to 30x faster AI inference.
Ad

3.8 was the best erpsonse out of them all the second fastest  due to the word count tho.. chatgpt was the fasstest but that one and the 3.6 sound slike a robot

Perfect. I think we've found our initial AI brain. 😁

Based on your testing, Qwen3.8 27B wins for OpenReceptionist.

And your observation about GPT-OSS and Qwen3.6 sounding robotic is important. For a receptionist, conversational quality matters enormously.
1. Benchmark results so far
Model	Response quality	Speed	Verdict
Qwen3.8 27B	Excellent	2nd fastest	🏆 Winner
GPT-OSS 20B	Less natural	Fastest	Backup candidate
Qwen3.6 35B-A3B	Robotic	Slower	Not preferred

These are preliminary subjective results, not formal benchmarks.
2. Let's optimize Qwen3.8 for receptionist conversations

We want it to:

    Speak naturally.
    Avoid unnecessarily long answers.
    Ask one question at a time.
    Avoid repeating itself.
    Sound friendly without being overly enthusiastic.
    Respond quickly.

I'd start with these Ollama parameters:
text

temperature: 0.7
top_p: 0.85
top_k: 30
repeat_penalty: 1.1

We can benchmark these against the current defaults.
3. Our AI architecture is taking shape
Component	Selection	Status
AI Brain	Qwen3.8 27B	✅ Selected
ATT	Qwen3-ASR	Pending
TTA	Qwen3-TTS	Pending
Embeddings	Embedding model	Pending licensing review
4. Next: Give Qwen3.8 a proper receptionist personality

I want to test something slightly different.

Run:
bash

ollama run qwen3.8:27b

Paste:
text

You are Sarah, a professional AI receptionist.

You communicate like a real human receptionist,
not a chatbot.

PERSONALITY:
- Warm and approachable.
- Professional but relaxed.
- Natural conversational language.
- Confident and helpful.

CONVERSATION RULES:
- Keep most responses between 10 and 30 words.
- Ask only one question at a time.
- Never repeat information unnecessarily.
- Avoid robotic phrases and generic greetings.
- Never explain your internal reasoning.
- Never invent business information.
- If you don't know something, say so naturally.

IMPORTANT:
Sound like someone answering a business phone,
not someone writing an email.

A customer says:

"Hey, I've been meaning to book an appointment
but I'm not really sure what I need."

Respond naturally.

What we're looking for

I want to see whether we can make Qwen3.8 sound even more human through prompting and configuration without sacrificing its intelligence.

Once we're happy with its personality, we'll move on to Qwen3-ASR (the ears) and Qwen3-TTS (the voice).

We're building this in the right order.
For comparing AI agent frameworks, here’s a structured learning option.
Learn more
AWS Marketplace
Your Framework
Compare agent frameworks. Choose yours.
Ad

Totally okay, happens all the time. Can you give me a rough idea of what's been on 
your mind? That'll help me point you the right direction.

>>> Send a message (/? for help)
 yeah i mena its not the best but its workab;e I think the voice sound is what will mark the biggest impact tho

I completely agree. In fact, I think the voice will have a bigger impact on perceived quality than the difference between our current LLM candidates.

A receptionist can have brilliant intelligence, but if it sounds like a robotic GPS, customers won't enjoy interacting with it.

We should focus heavily on TTS.
1. Our voice engine: Qwen3-TTS

I'd stick with our original choice for now.

Qwen3-TTS

Why:

    Natural-sounding speech.
    Voice design capabilities.
    Multiple languages.
    Voice cloning capabilities, subject to appropriate voice consent.
    Local inference.
    Apache 2.0 licensing.

Official repository: Qwen3-TTS
2. But let's compare voices before committing

I'd like to test three approaches:
Voice approach	Description
Natural female voice	Warm, friendly receptionist
Professional female voice	Clear, confident business receptionist
Conversational voice	Relaxed, natural, less scripted

We should also test male voices, accents and multilingual pronunciation.
3. The architecture we're building
text

       CUSTOMER SPEAKS
              |
              v
          QWEN3-ASR
              |
              v
          QWEN3.8
          AI BRAIN
              |
              v
        RESPONSE TEXT
              |
              v
          QWEN3-TTS
              |
              v
       NATURAL HUMAN VOICE
              |
              v
          CUSTOMER

4. One thing I want to optimize

We should eventually make the receptionist sound conversational rather than simply reading generated text.

For example:

Robotic: "Hello. Thank you for calling our dental clinic. How may I assist you today?"

Natural: "Hi there! Thanks for calling. What can I help you with today?"

The difference is enormous.

We'll also need to optimize:

    Speaking speed.
    Pauses between sentences.
    Intonation.
    Pronunciation.
    Emotional expression.
    Response latency.

5. Next step: Install Qwen3-TTS

Before downloading, let's check whether your DGX Spark has the necessary Python environment and dependencies.

Run:
bash

python3 -m venv ~/openreceptionist-venv
source ~/openreceptionist-venv/bin/activate

python --version
pip --version

Don't install anything else yet.

My goal is to get you to a point where you can type a sentence, select a voice, click Generate, and hear your AI receptionist speak through your speakers.

Then we'll connect it to Qwen3.8.
Learn more
Digital Ocean
Build Agents, Not Infra
Skip the setup. Focus on what agents can do.
Ad

pip --version
Python 3.12.3
pip 24.0 from /home/cse455student/openreceptionist-venv/lib/python3.12/site-packages/pip (python 3.12)
(openreceptionist-venv) cse455student@spark-75a3:~$

Perfect! Your Python virtual environment is working correctly. ✅

We're ready to prepare the TTS engine.

One thing: because you're running an ARM-based DGX Spark with CUDA 13.0, I want to be careful with PyTorch. We don't want to accidentally install a CPU-only version and lose GPU acceleration.

The official Qwen3-TTS project supports Python 3.12. GitHub
Step 1 — Check PyTorch

With (openreceptionist-venv) still active, run:
bash

echo "===== PYTORCH ====="

python -c "import torch; print('Version:', torch.__version__); print('CUDA available:', torch.cuda.is_available()); print('CUDA version:', torch.version.cuda) "

If it says No module named torch, that's fine.
Step 2 — Check NVIDIA's existing Python environment

Run:
bash

deactivate

python3 -c "import torch; print('Version:', torch.__version__); print('CUDA available:', torch.cuda.is_available()); print('CUDA version:', torch.version.cuda)"

This helps us determine whether NVIDIA's PyTorch installation is already available outside the virtual environment.
Step 3 — Our TTS target

We'll initially use:

Qwen3-TTS 1.7B CustomVoice

It offers:

    Natural-sounding voices.
    Multiple speaker options.
    Voice instructions and expressive speech.
    Multilingual generation.
    Local inference.

Official project: Qwen3-TTS

We'll initially avoid installing FlashAttention or changing CUDA dependencies.

Send me the two test outputs. Then I'll give you the correct installation commands for your DGX Spark.
Worked for 8s
Sources
This might also interest you.
Learn more
Oracle
Efficient AI on OCI
GPU capacity at flat price. See a demo.
Ad

no module name torch

No problem. That means PyTorch isn't installed in your virtual environment.

Before installing it, let's check whether NVIDIA already provides a GPU-enabled PyTorch installation on your DGX Spark.
Step 1 — Exit the virtual environment
bash

deactivate

Step 2 — Check system Python
bash

python3 -c "import torch; print('PyTorch:', torch.__version__); print('CUDA available:', torch.cuda.is_available()); print('CUDA:', torch.version.cuda)"

There are two possible outcomes:

    PyTorch found: Great. We'll check whether it supports your GB10 GPU.
    No module named torch: Also fine. We'll install a compatible NVIDIA PyTorch environment.

Important

Don't run pip install torch yet.

Your DGX Spark uses ARM64 and GB10 Blackwell hardware. We want an NVIDIA-compatible PyTorch build, not a generic installation that might fail to use your GPU.

Send me the output, and we'll proceed with Qwen3-TTS.
This might also interest you.
Learn more
Oracle
Ground LLMs in Data
Pair any model with Oracle AI Database
Ad

no moduel name d torch

That's fine. PyTorch isn't installed system-wide either.

We'll install it specifically for your NVIDIA DGX Spark (GB10, ARM64).

Before that, let's check whether NVIDIA's CUDA-enabled Python packages are available.

Run:
bash

python3 -m pip list | grep -Ei 'torch|cuda|nvidia'

Also run:
bash

ls /usr/local/

Send me both outputs.

Important: I want to use NVIDIA's compatible PyTorch distribution for DGX Spark rather than accidentally installing a CPU-only version. We should get GPU acceleration working before installing Qwen3-TTS.
This might also interest you.
Learn more
Oracle
Lower Cost per Token
Efficient OCI infra for inference
Ad

l last):
  File "<string>", line 1, in <module>
ModuleNotFoundError: No module named 'torch'
cse455student@spark-75a3:~$ python3 -m pip list | grep -Ei 'torch|cuda|nvidia'
\
> ^C
cse455student@spark-75a3:~$ python3 -m pip list | grep -Ei 'torch|cuda|nvidia'
cse455student@spark-75a3:~$ ls /usr/local/
bin  cuda  cuda-13  cuda-13.0  etc  games  include  lib  man  sbin  share  src
cse455student@spark-75a3:~$

Good! Now we know exactly what we're dealing with.

Your results confirm:

    CUDA 13.0 is installed.
    NVIDIA drivers are installed.
    PyTorch is not installed.
    No existing PyTorch installation will be affected by our new virtual environment.

Your DGX Spark's driver and CUDA versions are documented in NVIDIA's DGX Spark release notes. NVIDIA Docs
Step 1 — Prepare PyTorch installation

Let's use the CUDA 13.0 PyTorch package index, rather than installing a generic CPU-only package.

First, activate our virtual environment:
bash

source ~/openreceptionist-venv/bin/activate

Update pip:
bash

python -m pip install --upgrade pip

Now check which PyTorch package pip would install:
bash

python -m pip install torch \
  --index-url https://download.pytorch.org/whl/cu130 \
  --dry-run

The --dry-run means it checks compatibility without installing anything.
Step 2 — Send me the output

I want to verify:

    It finds an ARM64-compatible wheel.
    It selects a CUDA-enabled PyTorch version.
    It doesn't attempt to compile PyTorch from source.

Once confirmed, we'll install it.
Step 3 — Our first GPU test

After installation, we'll run:
bash

python -c "import torch; print('PyTorch:',torch.__version__); print('CUDA:',torch.cuda.is_available()); print('GPU:',torch.cuda.get_device_name(0) if torch.cuda.is_available() else 'Not detected')"

Our target:
text

PyTorch: 2.x.x
CUDA: True
GPU: NVIDIA GB10

Then we move straight to Qwen3-TTS.

I want to get your first natural-sounding AI voice generated on that DGX Spark before we build anything else.
Worked for 15s
Sources
For missing module issues, here’s one AI-first engineering team enablement option.
Learn more
New Possibilities Group LLC
Make Your Engineering Team AI-First
We help teams adopt Claude, Codex & GitHub Enterprise with a tailored agentic coding playbook.
Ad

