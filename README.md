# TeamDesk-AI-Customizable-AI-Powered-Mobile-Workspace
Help small businesses and teams manage their daily work using customizable tools and AI agents.


# 1. Project idea

TeamDesk AI is a mobile application that allows people to create a digital workspace tailored to their business needs. Instead of using separate applications for customer management, task tracking, project updates, and routine operations, users can manage these activities through one customizable app.
The main idea is that different users can configure TeamDesk AI for different types of work, while AI agents help them perform tasks, find information, and automate repetitive activities.
For example, a freelance consultant might use it to manage clients and appointments, while a software team might use it to track projects, assign tasks, and summarize progress.



# 2. Who will use it?
a) Freelancers and consultants
Manage clients, follow-ups, appointments, and personal work tasks.
b) Small business owners
Organize customer information, business activities, and recurring workflows.
c)Small teams and agencies
Coordinate projects, delegate tasks, manage clients, and monitor progress.


# 3. Main features
- Customizable workspace: Users choose how to organize their business activities.
- CRM: Store customer details, interaction history, and follow-up reminders.
- Task and project management: Create tasks, assign responsibilities, set deadlines, and track progress.
- AI assistant: Ask questions about business information in natural language.
- AI agents: Delegate defined tasks such as preparing client summaries, suggesting next steps, and drafting updates.
- Workflow automation: Use n8n to automate repetitive processes.
- Persistent memory: Retain relevant conversation context and workflow state across sessions.
- Reports and insights: Generate summaries of pending work, client activity, and project progress.
- Team access: Support multiple users with appropriate permissions.
  
# 4. How the AI works
Imagine a consultant opens TeamDesk AI and types:
“Show me clients I haven't contacted this week and prepare follow-up messages.”

The application could:
1. Retrieve the relevant client records from PostgreSQL.
2. Use the AI agent workflow built with LangGraph to identify clients needing follow-up.
3. Generate draft messages using a model accessed through OpenRouter.
4. Present the drafts for the user to review and approve.
5. Optionally trigger an approved automation through n8n.
The AI should not independently send messages or make sensitive changes without the necessary permissions and approval.

# 5. Technology Stack

| Layer | Technology | Role |
|---|---|---|
| Mobile App | Flutter + Dart | Android and iOS application |
| Backend | Python + FastAPI | Business logic and APIs |
| Database | PostgreSQL | Users, clients, tasks, and projects |
| Vector Search | pgvector | Semantic search over business information |
| AI Integration | LangChain | Model integration, retrieval, and tools |
| Agent Workflows | LangGraph | Stateful, multi-step AI execution |
| Memory | PostgreSQL | Persistent conversation and workflow state |
| Automation | n8n | Connect events and automate workflows |
| LLM Provider | OpenRouter | Access to compatible language models |
| Development | Docker | Consistent local development environment |


# 6. What makes this project valuable?
TeamDesk AI is more than a basic chatbot. It combines a real mobile business application with database-backed CRM functionality, configurable workflows, AI agents, persistent memory, and automation.
It can demonstrate practical skills in Flutter development, API design, database modelling, retrieval-augmented generation, agent orchestration, tool authorization, and reliable workflow execution.
