# AI Tools, Workflows & Practices

## AI Tools in Daily Use

### OpenAI Ecosystem
- **ChatGPT** — conversational AI for research, brainstorming, problem-solving
- **Codex** — CLI + App for code generation and assistance
- **Atlas** — knowledge/project management
- **Sora** — video generation

### Anthropic Ecosystem
- **Claude** — conversational AI
- **Claude Code** — CLI + App for agentic coding workflows
  - Plugins, channels, hooks
  - Custom skills creation and management
  - Subagents for parallel task execution
  - MCP (Model Context Protocol) server integrations
  - Git worktrees for isolated agent work
- **Cowork** — collaborative AI workflows

### Multi-Agent Systems
- **OpenClaw** — Personal multi-agent system running on a dedicated computer
  - Built **Mission Control** (TypeScript) — web UI for managing OpenClaw agent operations
  - Task dispatching, agent identity management, quality gates
  - Local LLM via **Ollama** for token economics
  - GitHub: `arraydude/mission-control`
- **AI Agents for PR reviewing and monitoring** — automated code review pipeline

### Development Tools
- **Cursor** — AI-powered IDE with multi-agent workflows, PR reviewing
- **OpenCode** — AI coding tool
- **OpenRouter** — multi-provider LLM routing

## AI Workflow Concepts & Expertise

### MCP (Model Context Protocol)
- Building and configuring MCP servers for tool integration
- Connecting AI agents to external services (GitHub, browsers, databases)

### Skills System
- Created a **foundation of skills for Mailberry's team** to improve and standardize AI-assisted development
- Published skills: frontend-design, react-query best practices, websocket architecture, composition patterns, React best practices, web design guidelines
- Skills.sh ecosystem
- Personal agent-skills repo (`arraydude/agent-skills`)

### Agent Architecture
- Agent tools and subagent orchestration
- Custom Claude Code commands: analyze, automation, autonomous-task-processor, clarify, implement, plan, validate-pr, and more
- Custom agents: backend-specialist
- Constitution files for agent behavior governance

### Workflow Automation
- PR validation agents
- Task processing pipelines (single-task and autonomous processors)
- Git worktrees for parallel agent execution

## Building AI-Powered Products (Mailberry)

### Product-Level AI Integration
- **Vercel AI SDK** — multi-provider integration (Anthropic, OpenAI, Google GenAI, OpenRouter)
- **The Email Brain** — AI-powered email marketing automation platform
- AI content generation for email campaigns (copy + layout)
- **Data Analyst Agent** — customer behavior analysis and campaign suggestions
- **Content Strategist** — on-brand copy and email layout generation

### AI Infrastructure at Mailberry
- `.claude/` directory with skills, agents, and commands for the entire team
- Standardized AI-assisted development workflows across the engineering team
- Code review automation
- Crawlee/Puppeteer for AI-assisted web scraping

## Personal AI Projects

### Mission Control (`arraydude/mission-control`)
- Full operational dashboard for OpenClaw multi-agent system (TypeScript, React, Vite, shadcn/ui)
- Reads real agent state: configured agents, session counts, latest activity, channel policies
- Gateway monitoring: service/runtime/listening state, operational blockers detection
- Persistent task board (SQLite-backed): Inbox → Ready → Doing → Blocked → Done pipeline
- Agent assignment, priority management, status tracking across the multi-agent fleet
- Local API endpoints for task CRUD operations

### HPTuners Ranger Agent (`arraydude/hptuners-ranger-agent`)
- Domain-expert AI agent for Ford Ranger Raptor 3.0L EcoBoost V6 ECU tuning
- Deep technical knowledge base: torque-based PCM model, wastegate position control, knock octane modifiers, LSPI protection, boost/spark swap dynamics
- Goal: AI assistant for tuning decisions, datalog analysis, and calibration guidance
- Built with Claude Code — intersection of AI engineering expertise and motorsports domain knowledge

### Tribe Shipping — AI-Managed Side Business
- Runs **Tribe Shipping** — a premium automotive parts import service in Argentina (BMW specialists)
- Full business management via Claude Code: order tracking, quoting, stock management, profit analysis
- Custom `/tribe-orders` skill for the team's workflow
- Dedicated repo (`arraydude/tribe`) with Claude Code integration (CLAUDE.md, skills)
- Demonstrates applying AI tools beyond software engineering — to real business operations

### Agent Skills (`arraydude/agent-skills`)
- Reusable skill library: feature-workflow, react-query-best-practices

### Chatbot (`arraydude/chatbot`)
- Python/Streamlit chatbot application

## AI in Previous Roles
- **Raven[Ops]:** Built visualization tools for QA team to iterate AI/ML robotics models faster
- **Streamlit:** The framework itself is used by ML/data science teams worldwide — deep understanding of how data scientists work with AI
- **Snowflake:** (TBD)

## Leadership Angle
- Established AI-assisted development standards for Mailberry's engineering team
- Created reusable skill libraries that standardize how the team uses AI tools
- Built internal tooling (commands, agents, constitutions) to guide AI behavior in the codebase
- Experience training/onboarding team members on AI-augmented workflows
