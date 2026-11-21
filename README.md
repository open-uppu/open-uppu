# open-uppu 🏢

> **Multi-product software house workspace.**  
> GitHub Organization: [github.com/open-uppu](https://github.com/open-uppu)  
> Each product is its own sibling folder under `open-uppu/` — git isolation, safe backups, clean separation.

---

## 🚀 Products (sibling folders)

| Folder | Product | Type | Stack | Status | GitHub | Owner |
|---|---|---|---|---|---|---|
| [`jito-cli/`](./jito-cli/) | **jito ⚡** — Multi-mode AI agent CLI | CLI tool (binary) | Go 1.22, cobra, Bubble Tea | ✅ v0.2.0 shipped | [open-uppu/jito](https://github.com/open-uppu/jito) | OpenUppu-BE |
| [`jito-ide/`](./jito-ide/) | **jito-ide ⚡🖥️** — VS Code extension | Editor extension | TypeScript, React, Node 20 | 🟡 v0.1.0 MVP | [open-uppu/jito-ide](https://github.com/open-uppu/jito-ide) | jito-ide |
| [`omyxia/`](./omyxia/) | **omyxia 🏢** — Enterprise IT Master Blueprint | Multi-tenant SaaS | NestJS, Prisma, Next.js, RLS | ✅ v1.0.0 Production Hardened | [open-uppu/Omyxia](https://github.com/open-uppu/Omyxia) | OpenUppu-FE/BE |
| [`trader/qualabinance/`](./trader/qualabinance/) | **Qualabinance 📊** — Multi-asset Quant Finance | Quant platform | Python, uv, Minimax-M3 | 🟡 v0.1.0 bootstrap | [open-uppu/qualabinance](https://github.com/open-uppu/qualabinance) | QuantResearcher |
| [`llm-gateway/`](./llm-gateway/) | **LLM Gateway 🌐** — LiteLLM Router | Proxy & Gateway | Python, LiteLLM, Docker Compose | 🟢 Operational | [open-uppu/llm-gateway](https://github.com/open-uppu/llm-gateway) | OpenUppu-Infra |
| [`trader/`](./trader/) | **Trader Ecosystem 📈** — EDCA, Trader Hub, Qualabinance | Algorithmic Trading & Quant | Python, FastAPI, MT5, uv, Next.js | 🟢 Operational | [open-uppu/trader-hub](https://github.com/open-uppu/trader-hub) | OpenUppu-Quant |
| [`plugins/`](./plugins/) | **OpenUppu Plugins Suite 🔌** | Agent Extensions (10 CLI/IDE plugins) | TypeScript, Node, Shell | 🟢 Shipped | [open-uppu](https://github.com/open-uppu) | OpenUppu-Core |

---

## 🤖 Sub-agent & Team Structure

### 🏢 Omyxia Sprint Team (`open-uppu/omyxia/`)
| Agent | Role | ID | Tools / Focus |
|---|---|---|---|
| **Omyxia SaaS 🏢** | Product Lead & System Architect | `agent-e65d0a6b-2900-44c0-b429-c58c567772d0` | codex, agy, nest, prisma |
| **Omyxia Manager 👔** | Agile Sprint & Roadmap Coordinator | `agent-2039697e-455e-4709-9441-22d870857011` | sprint tracking, tasks, releases |
| **Omyxia Frontend / UXUI 🎨** | Web UI/UX & Design System Engineer | `agent-eb19ab61-eb36-4b5c-800f-930d8ebda443` | Next.js, Tailwind, component library |
| **Omyxia Backend ⚙️** | Core API & Distributed Database Lead | `agent-467b4fd7-9223-41b0-b85a-0f14213dbeb8` | NestJS, Prisma, PostgreSQL RLS |
| **Omyxia QA Test 🧪** | Automated Testing & Security QA Lead | `agent-397622fa-1e02-4831-890e-2336014a4bc8` | E2E, Vitest, regression audits |
| **Omyxia HR 👥** | Knowledge Base & Team Operations | `agent-c94b710e-b347-416b-a7a9-c65daddf942b` | docs, onboarding, workflow guides |

### ⚡ Jito Sprint Team (`open-uppu/jito-ide/` & `open-uppu/jito-cli/`)
| Agent | Role | ID | Tools / Focus |
|---|---|---|---|
| **Jito IDE 🖥️** | VS Code Extension Lead | `agent-664caae8-c6a5-41fb-98c3-d302b7e933aa` | TypeScript, VS Code API, webview |
| **Jito CLI ⚡** | Go Core Engine Lead | `agent-954ee8fa-c861-43f0-b675-6e1f7f6e6c11` | Go 1.22, Cobra CLI, Bubble Tea |
| **Jito Manager 👔** | Sprint & Release Coordinator | `agent-373af394-d334-45db-b996-e6e15531179b` | sprint planning, release coordination |
| **Jito Frontend / UXUI 🎨** | Extension Webview & UI/UX Specialist | `agent-59af22bc-a324-4536-9eb1-e8136b6337e2` | React, VS Code Theme API, UI/UX |
| **Jito Backend ⚙️** | Extension Host & Go Core Bridge | `agent-450b74f4-bdad-4609-9031-d1be6bb5f8b3` | IPC, Node/Go integration, LSP |
| **Jito QA Test 🧪** | Multi-platform Test & Verification Lead | `agent-0ced10fb-0815-4904-ae17-19c337b648c3` | VS Code extension tests, CLI tests |
| **Jito HR 👥** | Developer Docs & Contributor Ops | `agent-46f21ff1-2db5-404e-ac5a-64f84532f738` | developer guides, changelogs, RFCs |

### 📊 Qualabinance Sprint Team (`open-uppu/trader/qualabinance/`)
| Agent | Role | ID | Tools / Focus |
|---|---|---|---|
| **Qualabinance 📊** | Quantitative Research Lead | `agent-475fe798-75ea-4839-a590-0a52b237d2e0` | Python, uv, backtest, quant |
| **Qualabinance Manager 👔** | Quant Product & Research Manager | `agent-9ed4f561-6c73-46dc-9d07-e3dbd627f550` | Roadmap, Quant Sprint Planning, Backtesting & Risk Analytics |
| **Qualabinance Frontend / UXUI 🎨** | Quant Analytics & Visualizations Engineer | `agent-14a59029-159f-43b3-9fbf-84d0711e6643` | Equity Curves, Heatmaps, Web Dashboard |
| **Qualabinance Backend ⚙️** | Quantitative Engine & Core Systems Lead | `agent-b6820ede-c755-497f-a5fc-1beb328f5d6e` | Python/uv backtest engine, Alpha signals, Vectorized metrics |
| **Qualabinance QA Test 🧪** | Model Validation & Risk QA Lead | `agent-722dee97-6a33-4e2f-a235-c692567997ec` | Model Validation, Overfitting checks, Stress Testing |
| **Qualabinance HR 👥** | Quant Knowledge & Research Operations | `agent-a33d1275-e267-40aa-9d0a-6f020a09271a` | Quant docs, Research logs, Runbooks |

### 🌐 LLM Gateway Sprint Team (`open-uppu/llm-gateway/`)
| Agent | Role | ID | Tools / Focus |
|---|---|---|---|
| **LLM Gateway 🌐** | LiteLLM & Infra Lead | `agent-b3ebb359-9f20-4215-a0a3-067651350d19` | LiteLLM, Docker Compose, Proxy |
| **LLM Gateway Manager 👔** | Gateway & Routing Product Manager | `agent-584e0c25-4bd7-40ad-994b-d9776c5bc1a4` | Roadmap, Routing Policies, Quotas, Sprints |
| **LLM Gateway Frontend / UXUI 🎨** | Gateway Console & Portal Engineer | `agent-682c58ed-484b-44c8-b4b7-be30e59f9c71` | Management Console, Token Analytics, API Portal |
| **LLM Gateway Backend ⚙️** | Proxy Routing & Key Management Lead | `agent-54106e08-4b64-4872-bab8-1dcada6e1efb` | LiteLLM Proxy, Dynamic Key Probing, Fallbacks |
| **LLM Gateway QA Test 🧪** | Load Testing & Failover QA Lead | `agent-ede2eb4e-e9de-4b3e-8ca7-40d7a91ddfcf` | Load Testing, Provider Failover, SLA Checks |
| **LLM Gateway HR 👥** | API Documentation & Operations Lead | `agent-e746d8a3-7857-4d6f-a065-b0e3f9d51f48` | API docs, OpenAPI specs, Onboarding |

### 📈 Trader Sprint Team (`open-uppu/trader/`)
| Agent | Role | ID | Tools / Focus |
|---|---|---|---|
| **Trader Hub 📈** | Quantitative Trading & System Lead | `agent-1361e7ea-d013-400b-9ccf-133f32ed4b2c` | Trading Strategy, Bot Architecture, Quant Signals |
| **Trader Manager 👔** | Trading Product & Sprint Coordinator | `agent-9e15ec24-ff2f-4ebe-b74b-59db2f4a1914` | Agile Roadmap, Risk Limits, Sprint Management |
| **Trader Frontend / UXUI 🎨** | Trading Dashboard & Visualizer | `agent-874f8aba-3220-4499-bcf8-f03f867310d0` | TradingView widgets, Web UI, Real-time Charts |
| **Trader Backend ⚙️** | Execution Engine & Broker Integration | `agent-07283fad-fb72-443c-b0c6-ec791d3afcec` | FastAPI, MT5 Bridge, Order Execution, EDCA |
| **Trader QA Test 🧪** | Strategy Backtest & Risk QA | `agent-95fb3209-3023-4fa9-8740-410965b86e6e` | Backtesting QA, Slippage Validation, Stress Testing |
| **Trader HR 👥** | Trading Playbook & Operations | `agent-1f582bd9-fe2b-4fa0-8a6d-96b373026a75` | Runbooks, API Keys Safety, Strategy Logs |

### 🌐 Shared & Specialized Agents
| Agent | Owns | ID | Tools / Focus |
|---|---|---|---|
| **Help open-uppu** | Workspace Coordination | `agent-00b06c9f-d2c8-4dcc-8a3f-5c20d4d369b9` | OpenBot orchestration |

---

## 🛡️ Hard rules

1. **One product = one sibling folder.** Never nest a product inside another product's repo.
2. **No cross-product imports** without explicit CEO approval.
3. **Each product has its own git remote** under `github.com/open-uppu`.
4. **Backup each product independently**.
5. **`open-uppu/` = umbrella + meta only.**
