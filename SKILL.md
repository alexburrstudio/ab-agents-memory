---
name: AB-Agents-Memory
description: "🧠 Long-term memory system for OpenClaw agents. Manages entities, context, and knowledge base with Obsidian integration. By AB-Agents."
version: 1.0.1
author: AB-Agents
homepage: https://github.com/alexburrstudio/ab-agents-memory
license: MIT
tags: ["memory", "agents", "openclaw", "obsidian", "knowledge-base", "entities", "context", "ab-agents"]
acceptLicenseTerms: true
---

# AB Agents Memory 🦀

**Long-term memory system for OpenClaw agents**

---

## Features

- 🗂️ **Entity Management** — Store info about People, Companies, Topics
- 🔗 **Entity Linking** — Connect entities with relationships
- 📊 **Context Summaries** — Auto-generated summaries for agents
- 🌙 **Nightly Processing** — Automatic data processing pipeline
- 📁 **Obsidian Integration** — Ready-to-use vault with templates

## Quick Start

```bash
# Via ClawHub
clawhub install AB-Agents-Memory

# Or manually
git clone https://github.com/alexburrstudio/ab-agents-memory.git
cd ab-agents-memory
./setup.sh
```

## Structure

```
memory/
├── agents/
│   └── AB-Archivus/       # Memory keeper agent
│       ├── SOUL.md
│       ├── IDENTITY.md
│       └── AGENTS.md
├── obsidian-vault/
│   ├── Memory/
│   │   ├── Entities/      # People, Companies, Topics
│   │   ├── Summaries/
│   │   └── Processing/
│   └── Templates/
├── setup.sh              # One-command install
├── SKILL.md              # ClawHub metadata
└── README.md
```

## What's Included

| Component | Description |
|-----------|-------------|
| `agents/AB-Archivus/` | OpenClaw agent for memory management |
| `obsidian-vault/` | Ready-to-use Obsidian vault with templates |
| `setup.sh` | Automated installation script |

## Requirements

- OpenClaw 2024+
- bash >= 4.0
- cron

## 📢 Links

- 🌐 **Канал AB Agents:** https://t.me/alexburr_agents
- 👤 **Автор:** https://t.me/AlexBurrOne
- 🐛 **Issues:** https://github.com/alexburrstudio/ab-agents-memory/issues
- 📦 **ClawHub:** https://clawhub.com/ab-agents-memory

## 💰 Support / Поддержать

Если оказалось полезно — донат приветствуется:

- 🥝 **TON:** @alexburrone
- 💳 **Т-БАНК:** https://www.tinkoff.ru/rm/r_vUjKxXYgKE.yxNpCcsGqi/wQhhR62314

---

**AB Agents Memory** — Your second brain for OpenClaw 🦀
*Made with 🖤 by [Alex Burr](https://t.me/AlexBurrOne)*