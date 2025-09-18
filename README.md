🎙️ Iris - Your AI voice assistant for building your network

Your AI-Powered Networking Memory Assistant
Never forget another meaningful conversation. Transform every networking event into lasting professional relationships.

Show Image
Show Image
Show Image
Show Image

🚀 The Problem
We attend hundreds of networking events, make incredible connections, exchange that electric energy with like-minded people... then connect on LinkedIn and forget the magic. Three months later, you need an expert in exactly what someone discussed, but your brain betrays you. The essence of human connection is lost in our digital graveyard of forgotten conversations.
✨ The Solution
Meet Iris - your AI voice assistant who captures the SOUL of every conversation! Say "Iris, activate!" and watch as every laugh, insight, and collaboration opportunity gets preserved in your digital people directory forever.
🎯 Key Features

🎙️ Voice-Activated Recording - "Iris, activate!" for seamless conversation capture
🤖 AI Agent Processing - 5 specialized agents extract people, context, topics, and relationship intelligence
🧠 Semantic Search - Find connections by meaning: "Who do I know in blockchain?"
📍 Contextual Memory - Every conversation mapped to time, place, and circumstances
🔍 Time Travel Search - "Show me everyone I met on Sept 17th"
🌐 Smart Directory - Auto-building people database with rich relationship context
🔒 Privacy First - GDPR compliant with full data control

🛠️ Tech Stack
ComponentTechnologyPurposeFrontendNext.js + TypeScript + ReactModern web interfaceBackendNode.js + ExpressAPI server and orchestrationVoice InterfaceVapiRecording & voice queriesAI ProcessingWriter.comConversation analysis agentsVector DatabaseWeaviateSemantic search & storageOrchestrationOpsera CodeGlideMCP server & agent coordinationStylingTailwind CSSUI componentsDatabasePostgreSQLMetadata storage
🏗️ Architecture
mermaidgraph TD
    A[Vapi Voice Recording] --> B[Writer.com AI Agents]
    B --> C{5 Specialist Agents}
    C --> D[Person Detective]
    C --> E[Context Mapper]
    C --> F[Topic Intelligence]
    C --> G[Relationship Analyzer]
    C --> H[Memory Weaver]
    D --> I[Weaviate Vector DB]
    E --> I
    F --> I
    G --> I
    H --> I
    I --> J[Semantic Search Engine]
    J --> K[Iris Voice Response]
    L[Opsera CodeGlide MCP] --> B
    L --> I
    L --> J
🚀 Quick Start
Prerequisites

Node.js 18+
PostgreSQL 14+
API keys for Vapi, Writer.com, Weaviate, Opsera CodeGlide

Installation

Clone the repository

bash   git clone https://github.com/yourusername/convovault-iris.git
   cd convovault-iris

Install dependencies

bash   npm install

Set up environment variables

bash   cp .env.example .env.local
Fill in your API keys:
env   VAPI_API_KEY=your_vapi_key
   WRITER_API_KEY=your_writer_key
   WEAVIATE_URL=your_weaviate_url
   WEAVIATE_API_KEY=your_weaviate_key
   OPSERA_API_KEY=your_opsera_key
   DATABASE_URL=postgresql://user:pass@localhost:5432/convovault
   NEXT_PUBLIC_APP_URL=http://localhost:3000

Initialize the database

bash   npm run db:migrate
   npm run db:seed

Start the development server

bash   npm run dev

Visit http://localhost:3000 and say "Iris, activate!"

📱 Usage
Basic Workflow

Activate Recording

   "Iris, activate!"

Have Natural Conversations

Iris records and processes in real-time
Auto-extracts people, context, and topics


Query Your Network

   "Where did I meet Adam Chan?"
   "Who do I know in AI?"
   "Show me everyone from the GitHub event"
Voice Commands
CommandExampleResultActivate"Iris, activate!"Start recording sessionPerson Search"How do I know Sarah?"Full conversation contextTopic Search"Who discussed blockchain?"Semantic matchesDate Search"Who did I meet yesterday?"Time-based filteringLocation Search"Show me the TechCrunch connections"Event-based results
🏗️ Project Structure
convovault-iris/
├── components/           # React UI components
│   ├── RecordingInterface.tsx
│   ├── ConversationCard.tsx
│   ├── PeopleDirectory.tsx
│   └── VoiceQuery.tsx
├── services/            # API integrations
│   ├── VapiService.ts
│   ├── WriterAgents.ts
│   ├── WeaviateService.ts
│   └── MCPServer.ts
├── agents/              # Writer.com agent configs
│   ├── PersonAgent.ts
│   ├── ContextAgent.ts
│   ├── TopicAgent.ts
│   ├── SentimentAgent.ts
│   └── SummaryAgent.ts
├── mcp/                 # Opsera CodeGlide setup
│   └── server.ts
├── pages/api/           # Next.js API routes
│   ├── recordings/
│   ├── people/
│   └── query/
├── types/               # TypeScript definitions
├── hooks/               # Custom React hooks
├── utils/               # Helper functions
└── prisma/              # Database schema
📡 API Endpoints
Recording

POST /api/recordings/start - Start conversation recording
POST /api/recordings/stop - Stop and process recording
GET /api/recordings/:id - Get recording details

People Directory

GET /api/people - Retrieve people directory
GET /api/people/:id - Get person details
PUT /api/people/:id - Update person information
DELETE /api/people/:id - Remove person (GDPR)

Search & Query

POST /api/query/voice - Voice query processing
GET /api/search/semantic - Semantic search endpoint
GET /api/search/date - Date-based search
GET /api/search/location - Location-based search

🤖 AI Agents
Writer.com Processing Pipeline

Person Detective Agent

Extracts names, titles, companies
Identifies contact information
Prevents duplicate entries


Context Mapper Agent

Captures meeting circumstances
Maps mutual connections
Records conversation triggers


Topic Intelligence Agent

Identifies expertise areas
Extracts collaboration opportunities
Maps industry knowledge


Relationship Analyzer Agent

Assesses connection strength
Identifies follow-up opportunities
Suggests engagement strategies


Memory Weaver Agent

Creates searchable narratives
Generates key quotes
Builds personality profiles



🧠 Weaviate Schema
typescriptinterface Person {
  name: string;
  company: string;
  title: string;
  meeting_context: string;
  location: string;
  date: Date;
  conversation_summary: string;
  topics_discussed: string[];
  contact_info: string;
  relationship_notes: string;
  follow_up_actions: string[];
  collaboration_potential: number;
  connection_strength: number;
}
🔒 Privacy & Security

🔐 End-to-end encryption for sensitive data
🗑️ GDPR-compliant data deletion
🎛️ Granular privacy controls
📍 Optional location tracking
🔒 Local data processing options

🤝 Contributing
We love contributions! Please see our Contributing Guide for details.

Fork the repository
Create your feature branch (git checkout -b feature/AmazingFeature)
Commit your changes (git commit -m 'Add some AmazingFeature')
Push to the branch (git push origin feature/AmazingFeature)
Open a Pull Request

📝 License
This project is licensed under the MIT License - see the LICENSE file for details.
🙏 Acknowledgments

Vapi for seamless voice interfaces
Writer.com for powerful AI agent processing
Weaviate for semantic search capabilities
Opsera CodeGlide for agent orchestration

🚀 What's Next?

 Mobile app development
 CRM integrations (Salesforce, HubSpot)
 LinkedIn auto-sync
 Team collaboration features
 Analytics dashboard
 Multi-language support


<div align="center">
Stop losing connections. Start building your networking superpower.
Website • Documentation • Discord • Twitter
Made with ❤️ for the networking community
</div>RetryClaude can make mistakes. Please double-check responses.
