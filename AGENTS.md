# AGENTS.md — Master Workspace Guidance for /Users/up-mac/wokrspace

Master configuration and orchestration rules for all AI coding agents working inside `/Users/up-mac/wokrspace`.

---

## 1. Workspace Identity & GitHub Dual-Namespace Topology

`/Users/up-mac/wokrspace` ขับเคลื่อนโดย 2 เสาหลักตาม GitHub Accounts:
1. **`open-uppu/`** → [github.com/open-uppu](https://github.com/open-uppu) (Software House products, team deliverables, public SaaS)
2. **`mind/`** → [github.com/AtiwitchJ](https://github.com/AtiwitchJ) (Personal engineering labs, AI security, research platforms)

```
/Users/up-mac/wokrspace/
├── AGENTS.md                     # This master workspace guidance
├── README.md                     # Master workspace portfolio directory
├── open-uppu/                    # 🏢 Organization: github.com/open-uppu
└── mind/                         # 🧠 Personal Profile: github.com/AtiwitchJ
```

---

## 2. Dedicated OpenBot Teammate Roster & GitHub Mapping

| Cluster / Project | GitHub Repository | Agent Name | Role / Title |
|---|---|---|---|
| **Root Workspace** | `/Users/up-mac/wokrspace` | **Help wokrspace** | Workspace Coordinator |
| **`open-uppu/` Cluster** | [open-uppu](https://github.com/open-uppu) | **Help open-uppu** | Software House Delivery Lead |
| ↳ `open-uppu/jito-cli` | [open-uppu/jito](https://github.com/open-uppu/jito) | **Jito CLI ⚡** | Go AI Agent CLI Lead |
| ↳ `open-uppu/jito-ide` | [open-uppu/jito-ide](https://github.com/open-uppu/jito-ide) | **Jito IDE 🖥️** | VS Code Extension Lead |
| ↳ `open-uppu/omyxia` | [open-uppu/Omyxia](https://github.com/open-uppu/Omyxia) | **Omyxia SaaS 🏢** | Enterprise SaaS Lead |
| ↳ `open-uppu/qualabinance` | [open-uppu/qualabinance](https://github.com/open-uppu/qualabinance) | **Qualabinance 📊** | Quant Finance Lead |
| ↳ `open-uppu/llm-gateway` | [open-uppu/llm-gateway](https://github.com/open-uppu/llm-gateway) | **LLM Gateway 🌐** | LiteLLM & Infra Lead |
| **`Omyxia` Active Team** | [open-uppu/Omyxia](https://github.com/open-uppu/Omyxia) | | **On-hand Sprint Team** |
| ↳ `open-uppu/omyxia` | [open-uppu/Omyxia](https://github.com/open-uppu/Omyxia) | **Omyxia Manager 👔** | Agile Sprint & Roadmap Coordinator |
| ↳ `open-uppu/omyxia` | [open-uppu/Omyxia](https://github.com/open-uppu/Omyxia) | **Omyxia Frontend / UXUI 🎨** | Web UI/UX & Design System Engineer |
| ↳ `open-uppu/omyxia` | [open-uppu/Omyxia](https://github.com/open-uppu/Omyxia) | **Omyxia Backend ⚙️** | Core API & Distributed Database Lead |
| ↳ `open-uppu/omyxia` | [open-uppu/Omyxia](https://github.com/open-uppu/Omyxia) | **Omyxia QA Test 🧪** | Automated Testing & Security QA Lead |
| ↳ `open-uppu/omyxia` | [open-uppu/Omyxia](https://github.com/open-uppu/Omyxia) | **Omyxia HR 👥** | Knowledge Base & Team Operations |
| **`Jito` Active Team** | [open-uppu/jito-ide](https://github.com/open-uppu/jito-ide) | | **On-hand Sprint Team** |
| ↳ `open-uppu/jito-ide` | [open-uppu/jito-ide](https://github.com/open-uppu/jito-ide) | **Jito Manager 👔** | Sprint & Release Coordinator |
| ↳ `open-uppu/jito-ide` | [open-uppu/jito-ide](https://github.com/open-uppu/jito-ide) | **Jito Frontend / UXUI 🎨** | Extension Webview & UI/UX Specialist |
| ↳ `open-uppu/jito-ide` | [open-uppu/jito-ide](https://github.com/open-uppu/jito-ide) | **Jito Backend ⚙️** | Extension Host & Go Core Bridge |
| ↳ `open-uppu/jito-ide` | [open-uppu/jito-ide](https://github.com/open-uppu/jito-ide) | **Jito QA Test 🧪** | Multi-platform Test & Verification Lead |
| ↳ `open-uppu/jito-ide` | [open-uppu/jito-ide](https://github.com/open-uppu/jito-ide) | **Jito HR 👥** | Developer Docs & Contributor Ops |
| **`Qualabinance` Active Team** | [open-uppu/qualabinance](https://github.com/open-uppu/qualabinance) | | **On-hand Sprint Team** |
| ↳ `open-uppu/qualabinance` | [open-uppu/qualabinance](https://github.com/open-uppu/qualabinance) | **Qualabinance Manager 👔** | Quant Product & Research Manager |
| ↳ `open-uppu/qualabinance` | [open-uppu/qualabinance](https://github.com/open-uppu/qualabinance) | **Qualabinance Frontend / UXUI 🎨** | Quant Analytics & Visualizations Engineer |
| ↳ `open-uppu/qualabinance` | [open-uppu/qualabinance](https://github.com/open-uppu/qualabinance) | **Qualabinance Backend ⚙️** | Quantitative Engine & Core Systems Lead |
| ↳ `open-uppu/qualabinance` | [open-uppu/qualabinance](https://github.com/open-uppu/qualabinance) | **Qualabinance QA Test 🧪** | Model Validation & Risk QA Lead |
| ↳ `open-uppu/qualabinance` | [open-uppu/qualabinance](https://github.com/open-uppu/qualabinance) | **Qualabinance HR 👥** | Quant Knowledge & Research Operations |
| **`LLM Gateway` Active Team** | [open-uppu/llm-gateway](https://github.com/open-uppu/llm-gateway) | | **On-hand Sprint Team** |
| ↳ `open-uppu/llm-gateway` | [open-uppu/llm-gateway](https://github.com/open-uppu/llm-gateway) | **LLM Gateway Manager 👔** | Gateway & Routing Product Manager |
| ↳ `open-uppu/llm-gateway` | [open-uppu/llm-gateway](https://github.com/open-uppu/llm-gateway) | **LLM Gateway Frontend / UXUI 🎨** | Gateway Console & Portal Engineer |
| ↳ `open-uppu/llm-gateway` | [open-uppu/llm-gateway](https://github.com/open-uppu/llm-gateway) | **LLM Gateway Backend ⚙️** | Proxy Routing & Key Management Lead |
| ↳ `open-uppu/llm-gateway` | [open-uppu/llm-gateway](https://github.com/open-uppu/llm-gateway) | **LLM Gateway QA Test 🧪** | Load Testing & Failover QA Lead |
| ↳ `open-uppu/llm-gateway` | [open-uppu/llm-gateway](https://github.com/open-uppu/llm-gateway) | **LLM Gateway HR 👥** | API Documentation & Operations Lead |
| **`Trader` Active Team** | [open-uppu](https://github.com/open-uppu) | | **On-hand Sprint Team (daytrad, edca, hub)** |
| ↳ `open-uppu/trader` | [open-uppu/trader-hub](https://github.com/open-uppu/trader-hub) | **Trader Hub 📈** | Quantitative Trading Platform Lead |
| ↳ `open-uppu/trader` | [open-uppu/trader-hub](https://github.com/open-uppu/trader-hub) | **Trader Manager 👔** | Agile Sprint & Roadmap Coordinator |
| ↳ `open-uppu/trader` | [open-uppu/trader-hub](https://github.com/open-uppu/trader-hub) | **Trader Frontend / UXUI 🎨** | Web Dashboard & TradingView UI |
| ↳ `open-uppu/trader` | [open-uppu/trader-hub](https://github.com/open-uppu/trader-hub) | **Trader Backend ⚙️** | Core Services, MT5 Bridge & EDCA Engine |
| ↳ `open-uppu/trader` | [open-uppu/trader-hub](https://github.com/open-uppu/trader-hub) | **Trader QA Test 🧪** | Backtest & Risk QA Lead |
| ↳ `open-uppu/trader` | [open-uppu/trader-hub](https://github.com/open-uppu/trader-hub) | **Trader HR 👥** | Knowledge Base & Team Operations |
| **`open-uppu/plugins` Suite** | [open-uppu](https://github.com/open-uppu) | **OpenUppu Plugins Suite 🔌** | 10 CLI/IDE Agent Plugins (claude, cursor, kimi...) |
| **`mind/` Cluster** | [AtiwitchJ](https://github.com/AtiwitchJ) | **Help Mind** | AI Research & Systems Lead |
| ↳ `mind/moden-agent` | [AtiwitchJ/agent-orchestrator](https://github.com/AtiwitchJ/agent-orchestrator) | **Modern Agent 🤖** | Parallel Agent Orchestrator |
| ↳ `mind/NoJect` | [AtiwitchJ/NoJect-Gateway](https://github.com/AtiwitchJ/NoJect-Gateway) | **NoJect Sentinel 🛡️** | AI Security & WAF Lead |
| ↳ `mind/Voice AI Agent` | [AtiwitchJ/voice-ai-agent-architecture](https://github.com/AtiwitchJ/voice-ai-agent-architecture) | **Voice AI 🎙️** | Conversational Voice Lead |
| ↳ `mind/data-en` | [AtiwitchJ/data-en](https://github.com/AtiwitchJ/data-en) | **Data Platform 🗄️** | Data Platform Lead |
| ↳ `mind/strock` | Local / [AtiwitchJ/strock](https://github.com/AtiwitchJ/strock) | **Strock Quant 📈** | Stock Analysis & Quantitative Modeling |
| ↳ `mind/video editor agent` | [AtiwitchJ/video-editor-agent](https://github.com/AtiwitchJ/video-editor-agent) | **Video Editor AI 🎬** | NLE & Video Agent Lead |
| ↳ `mind/customer-service-ai-chatbot` | [AtiwitchJ/customer-service-ai-chatbot](https://github.com/AtiwitchJ/customer-service-ai-chatbot) | **Customer Service AI 💬** | Chatbot Engineering Lead |
| ↳ `mind/lambase-app` & `lambase-mcp` | [AtiwitchJ/lambase-app](https://github.com/AtiwitchJ/lambase-app) | **Lambase Platform 🧩** | BaaS & MCP Lead |
| ↳ `mind/42bk-Research-Assistant-AI` | [AtiwitchJ/42bk-Research-Assistant-AI](https://github.com/AtiwitchJ/42bk-Research-Assistant-AI) | **42BK Research AI 🎓** | Research Assistant AI Lead |
| ↳ `mind/habit` | [AtiwitchJ/habit](https://github.com/AtiwitchJ/habit) | **Habit Tracker 📋** | Habit Platform Lead |
| ↳ `mind/gym` | [AtiwitchJ/gym](https://github.com/AtiwitchJ/gym) | **Gym & Fitness 🏋️‍♂️** | Fitness & Workout Web Lead |
| ↳ `mind/speech-to-text` | [AtiwitchJ/speech-to-text](https://github.com/AtiwitchJ/speech-to-text) | **Speech-to-Text 🔊** | Audio Transcription Lead |
| ↳ `mind/payment gateway transaction` | [AtiwitchJ/payment-gateway-transaction](https://github.com/AtiwitchJ/payment-gateway-transaction) | **Payment Gateway 💳** | Payment Microservice Lead |
| ↳ `mind/Atiwitch_Jitamornpak_Resume` | [AtiwitchJ/Atiwitch_Jitamornpak_Resume](https://github.com/AtiwitchJ/Atiwitch_Jitamornpak_Resume) | **Portfolio & Resume 📄** | Personal Brand & Web Lead |
| ↳ `mind/AI-Engineer-Programming-Bangkok-Bank-` | [AtiwitchJ/AI-Engineer-Programming-Bangkok-Bank-](https://github.com/AtiwitchJ/AI-Engineer-Programming-Bangkok-Bank-) | **BBL AI Assessment 🏦** | AI Assessment Specialist |
| ↳ `mind/emworkgroup` | [AtiwitchJ/emworkgroup](https://github.com/AtiwitchJ/emworkgroup) | **EM Workgroup 🏢** | Enterprise Solutions Lead |
| ↳ `mind/somchai-main` | [AtiwitchJ/somchai-main](https://github.com/AtiwitchJ/somchai-main) | **Somchai ML 🧪** | ML Metrics & Explainability Lead |
| ↳ `mind/liefcapital` | [AtiwitchJ/liefcapital](https://github.com/AtiwitchJ/liefcapital) | **Lief Capital 💼** | Quantitative Assessment Lead |
| ↳ `mind/monday` | [AtiwitchJ/monday](https://github.com/AtiwitchJ/monday) | **Monday Workflow 📅** | Workflow App Lead |
| ↳ `mind/agent-coder-plugin-cc` & `skill-project-docs` | Local / [AtiwitchJ/skill-project-docs](https://github.com/AtiwitchJ/skill-project-docs) | **Agent Tools & Skills 🛠️** | Agent Tools & Ecosystem Lead |
| ↳ `mind/go-basic-interview` | [AtiwitchJ/go-basic-interview](https://github.com/AtiwitchJ/go-basic-interview) | **Go Interview 🐹** | Go Assessment Lead |
| ↳ `mind/revenue` | Local (`mind/revenue`) | **Revenue & Cashflow 💰** | Cashflow & Finance Lead |
| ↳ `mind/test` | Local (`shrimp-shop`) | **Shrimp Shop 🦐** | Frontend Storefront Lead |
| **`GYM` Active Team** | [AtiwitchJ/gym](https://github.com/AtiwitchJ/gym) | | **On-hand Sprint Team** |
| ↳ `mind/gym` | [AtiwitchJ/gym](https://github.com/AtiwitchJ/gym) | **GYM Manager 👔** | Project & Engineering Manager |
| ↳ `mind/gym` | [AtiwitchJ/gym](https://github.com/AtiwitchJ/gym) | **GYM Frontend / UXUI 🎨** | Frontend & UX/UI Engineer |
| ↳ `mind/gym` | [AtiwitchJ/gym](https://github.com/AtiwitchJ/gym) | **GYM Backend ⚙️** | Backend & API Engineer |
| ↳ `mind/gym` | [AtiwitchJ/gym](https://github.com/AtiwitchJ/gym) | **GYM QA Test 🧪** | QA & Automation Test Lead |
| ↳ `mind/gym` | [AtiwitchJ/gym](https://github.com/AtiwitchJ/gym) | **GYM HR 👥** | People & Culture Specialist |
| **`habit` Active Team** | [AtiwitchJ/habit](https://github.com/AtiwitchJ/habit) | | **On-hand Sprint Team** |
| ↳ `mind/habit` | [AtiwitchJ/habit](https://github.com/AtiwitchJ/habit) | **Habit Manager 👔** | Product & Engineering Manager |
| ↳ `mind/habit` | [AtiwitchJ/habit](https://github.com/AtiwitchJ/habit) | **Habit Frontend / UXUI 🎨** | Frontend & UX/UI Engineer |
| ↳ `mind/habit` | [AtiwitchJ/habit](https://github.com/AtiwitchJ/habit) | **Habit Backend ⚙️** | Backend & Distributed Services Engineer |
| ↳ `mind/habit` | [AtiwitchJ/habit](https://github.com/AtiwitchJ/habit) | **Habit QA Test 🧪** | QA & Reliability Test Lead |
| ↳ `mind/habit` | [AtiwitchJ/habit](https://github.com/AtiwitchJ/habit) | **Habit HR 👥** | People & Team Operations Lead |

---

## 3. Universal Rules & Invariants

1. **Strict Cluster & Remote Isolation:**
   - Never push code meant for `open-uppu` to `AtiwitchJ`, or vice-versa. Maintain isolated remote configurations.
   - Products under `open-uppu/` are sibling git repositories. Never create cross-product dependencies without explicit approval.
2. **Evidence Before Assertions:**
   - Always run verification, type checks, and tests before claiming success. Raw command output is required.
3. **Local-First & Offline Resilience:**
   - Ensure tools and workflows run reliably locally without unauthorized external exfiltration.
4. **Environment & Secrets Safety:**
   - Never commit `.env` files, production API tokens, or private credentials into version control.
5. **Git Hygiene & Authorship:**
   - Follow Conventional Commits.
   - Maintain the standard co-author trailer when requested:
     `Co-authored-by: OpenBot <335604065+openbotgit[bot]@users.noreply.github.com>`


---

## 4. Continuous Improvement, Branching & QA/HR KPI Governance

1. **Mandatory Continuous Improvement & Push:**
   - Proactively discover and apply fixes, security hardening, linting, test suites, and structural hygiene across all workspace repositories.
   - Verified changes must be pushed to GitHub regularly.
2. **Branch Strategy on Uncertainty:**
   - If not fully confident in a change or if it introduces breaking changes / experimental logic, agents MUST create a separate branch (`feat/*`, `dev/*`, `fix/*`) and push to that branch instead of `main`.
3. **QA Quality Gate & KPI Merge Verification:**
   - **Role:** Every merge or direct push to `main` is gated by the QA Role (`* QA Test 🧪`).
   - **QA KPIs:**
     - 100% test pass rate across unit and integration tests.
     - 0 sensitive leaks or uncommitted runtime artifacts (`.env`, `.DS_Store`, credentials).
     - Standardized `docker-compose.yml` healthcheck compliance.
   - **HR Role (`* HR 👥`):** Defines, audits, and maintains team KPIs and sprint deliverables. Unverified or failing code must remain in its isolated branch until QA signs off.
