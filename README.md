# open-uppu 🏢

> **Multi-product software house workspace.**
> Each product lives in its own sibling folder for git isolation, safe backups, and clean separation of concerns.

---

## 🚀 Products (sibling folders)

| Folder | Product | Type | Stack | Status | Owner |
|---|---|---|---|---|---|
| [`jito-cli/`](./jito-cli/) | **jito ⚡** — Multi-mode AI agent CLI | CLI tool (binary) | Go 1.22, cobra, Bubble Tea | ✅ v0.2.0 shipped | OpenUppu-BE |
| [`open-uppu-jito-ide/`](./open-uppu-jito-ide/) | **jito-ide ⚡🖥️** — VS Code extension | Editor extension | TypeScript, React, Node 20 | 🟡 v0.1.0 MVP (kickoff 2026-06-29) | jito-ide |
| [`open-uppu-omyxia/`](./open-uppu-omyxia/) | **omyxia 🏢** — Enterprise IT Master Blueprint | Multi-tenant SaaS | NestJS, Prisma, Next.js, RLS | ✅ v1.0.0 Production Hardened | OpenUppu-FE/BE |
| [`open-uppu-qualabinance/`](./open-uppu-qualabinance/) | **Qualabinance 📊** — Multi-asset Quant Finance | Quant platform | Python, uv, Minimax-M3 | 🟡 v0.1.0 bootstrap | QuantResearcher |

> **Why sibling folders, not nested:** CEO mandate 2026-06-29 17:00 — each product = isolated git repo, no cross-contamination, no accidental `rm -rf` of siblings. After the 2026-06-27 17:08 incident where `rm -rf open-uppu/` wiped both source and nested target.

---

## 🤖 Sub-agent ownership

| Agent | Owns | Tools |
|---|---|---|
| OpenUppu-BE | jito-cli (Go core) | codex, agy, jules |
| OpenUppu-FE | omyxia frontend | codex, agy, kilo |
| OpenUppu-BE | omyxia backend | codex, agy, jules |
| **jito-ide** | open-uppu-jito-ide (TS extension) | codex, agy, kilo, vsce |
| QuantResearcher | open-uppu-qualabinance | codex, agy, kilo, uv, python |

---

## 📚 Specs & docs

- **Workspace index:** [`~/.openclaw/workspace/MEMORY.md`](../../.openclaw/workspace/MEMORY.md)
- **Product specs:** [`~/.openclaw/workspace/companies/*.md`](../../.openclaw/workspace/companies/)
- **Agent specs:** [`~/.openclaw/workspace/agents/*.md`](../../.openclaw/workspace/agents/)

---

## 🛡️ Hard rules

1. **One product = one folder.** Never nest a product inside another.
2. **No cross-product imports** without explicit CEO approval.
3. **Each product has its own git remote** (when going public).
4. **Backup each product independently** (no shared snapshot that mixes unrelated code).
5. **`open-uppu/` = meta only.** Don't put source code here. If you need a new product, create a sibling folder.
6. **Renames go through PM** with `cp -a` + verify + `rm` pattern. Never direct `mv` of folders with uncommitted work.

---

## 🔄 Conventions

```
~/wokrspace/open-uppu/         ← this folder (workspace meta)
~/wokrspace/jito-cli/          ← product 1 (Go CLI)
~/wokrspace/open-uppu-jito-ide/ ← product 2 (VS Code ext)
~/wokrspace/open-uppu-omyxia/  ← product 3 (SaaS)
~/wokrspace/open-uppu-qualabinance/ ← product 4 (Quant)
```

Naming pattern:
- `open-uppu-<product>` for products with public/open-source ambitions
- Bare name (`jito-cli`) for products that ship as their own brand

---

## 🚀 Add a new product

```bash
# 1. Create sibling folder
cd ~/wokrspace/
mkdir open-uppu-<name> && cd open-uppu-<name>

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
- 2026-06-29 17:00 — Migrated from nested `open-uppu/{jito,jito-ide,omyxia,qualabinance}` to sibling folders. Backup at `~/.openclaw/backups/open-uppu-migration-20260629-1701/`.