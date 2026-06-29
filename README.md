# open-uppu 🏢

> **Multi-product software house workspace.**
> Each product is its own sibling folder under `open-uppu/` — git isolation, safe backups, clean separation.

---

## 🚀 Products (sibling folders)

| Folder | Product | Type | Stack | Status | GitHub | Owner |
|---|---|---|---|---|---|---|
| [`jito-cli/`](./jito-cli/) | **jito ⚡** — Multi-mode AI agent CLI | CLI tool (binary) | Go 1.22, cobra, Bubble Tea | ✅ v0.2.0 shipped | [open-uppu/jito](https://github.com/open-uppu/jito) | OpenUppu-BE |
| [`jito-ide/`](./jito-ide/) | **jito-ide ⚡🖥️** — VS Code extension | Editor extension | TypeScript, React, Node 20 | 🟡 v0.1.0 MVP (kickoff 2026-06-29) | [open-uppu/jito-ide](https://github.com/open-uppu/jito-ide) | jito-ide |
| [`omyxia/`](./omyxia/) | **omyxia 🏢** — Enterprise IT Master Blueprint | Multi-tenant SaaS | NestJS, Prisma, Next.js, RLS | ✅ v1.0.0 Production Hardened | [open-uppu/Omyxia](https://github.com/open-uppu/Omyxia) | OpenUppu-FE/BE |
| [`qualabinance/`](./qualabinance/) | **Qualabinance 📊** — Multi-asset Quant Finance | Quant platform | Python, uv, Minimax-M3 | 🟡 v0.1.0 bootstrap | [open-uppu/qualabinance](https://github.com/open-uppu/qualabinance) | QuantResearcher |

**Meta-repo:** [open-uppu/open-uppu](https://github.com/open-uppu/open-uppu) (this folder, indexes only)

> **Why sibling folders (not flat under `wokrspace/`):** CEO mandate 2026-06-29 17:16 — keep `open-uppu/` as the umbrella folder for all open-uppu products, but isolate each one as a sibling. After the 2026-06-27 17:08 incident where `rm -rf open-uppu/` wiped both source and nested target. Sibling folders under `open-uppu/` give us isolation without losing the workspace grouping.

---

## 🤖 Sub-agent ownership

| Agent | Owns | Tools |
|---|---|---|
| OpenUppu-BE | jito-cli (Go core) | codex, agy, jules |
| OpenUppu-FE | omyxia frontend | codex, agy, kilo |
| OpenUppu-BE | omyxia backend | codex, agy, jules |
| **jito-ide** | jito-ide (TS extension) | codex, agy, kilo, vsce |
| QuantResearcher | qualabinance | codex, agy, kilo, uv, python |

---

## 📚 Specs & docs

- **Workspace index:** [`~/.openclaw/workspace/MEMORY.md`](../../.openclaw/workspace/MEMORY.md)
- **Product specs:** [`~/.openclaw/workspace/companies/*.md`](../../.openclaw/workspace/companies/)
- **Agent specs:** [`~/.openclaw/workspace/agents/*.md`](../../.openclaw/workspace/agents/)

---

## 🛡️ Hard rules

1. **One product = one sibling folder.** Never nest a product inside another product's repo.
2. **No cross-product imports** without explicit CEO approval.
3. **Each product has its own git remote** (when going public).
4. **Backup each product independently** (no shared snapshot that mixes unrelated code).
5. **`open-uppu/` = umbrella + meta only.** Don't put product code at the root. If you need a new product, create a sibling folder under `open-uppu/`.
6. **Renames go through PM** with `cp -a` + verify + `rm` pattern. Never direct `mv` of folders with uncommitted work.

---

## 🔄 Conventions

```
~/wokrspace/open-uppu/          ← this folder (workspace umbrella)
├── .git/                       (workspace-level meta repo)
├── README.md                   (this file)
├── jito-cli/                   ← product 1 (Go CLI)
├── jito-ide/                   ← product 2 (VS Code ext)
├── omyxia/                     ← product 3 (SaaS)
└── qualabinance/               ← product 4 (Quant)
```

Naming pattern: short, memorable, brand-friendly names. No `open-uppu-` prefix needed since they already live under the `open-uppu/` umbrella.

---

## 🚀 Add a new product

```bash
# 1. Create sibling folder under open-uppu/
cd ~/wokrspace/open-uppu/
mkdir <name> && cd <name>

# 2. Init git
git init

# 3. Bootstrap
# ... (your scaffold here)

# 4. Add to MEMORY.md
# Edit ~/.openclaw/workspace/MEMORY.md → products section
# Edit ~/.openclaw/workspace/MEMORY.md → agent roster (if applicable)

# 5. Add to this README
# Edit this file → products table

# 6. Notify CEO + spawn any sub-agents
```

---

**Owner:** CEO-Profile (Loop Engineering Layer)
**Migration history:**
- 2026-06-29 17:00 — First migration: nested `open-uppu/{jito,jito-ide,omyxia,qualabinance}` → sibling at `wokrspace/` root.
- 2026-06-29 17:16 — Re-migration (CEO pivot): back to `open-uppu/` umbrella with sibling subfolders (`open-uppu/{jito-cli,jito-ide,omyxia,qualabinance}`). Each product keeps its own git repo for isolation. Backups at `~/.openclaw/backups/open-uppu-migration-20260629-1701/` (398M) and `~/.openclaw/backups/open-uppu-remigration-*/` (398M).