# AB Agents Memory 🦀

**Long-term memory system for OpenClaw agents**

*by [AB-Agents](https://t.me/alexburr_agents)*

---

## Description

AB Agents Memory — система управления долгосрочной памятью агентов OpenClaw. Включает агента AB-Archivus и готовый Obsidian vault.

AB Agents Memory is a long-term memory management system for OpenClaw agents. Includes AB-Archivus agent and ready-to-use Obsidian vault.

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
cd memory
./setup.sh
```

One-liner:
```bash
git clone https://github.com/alexburrstudio/ab-agents-memory.git && cd memory && ./setup.sh
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
│   │   ├── Summaries/     # Context summaries
│   │   └── Processing/
│   │       └── Nightly/   # Nightly scripts
│   └── Templates/        # Entity templates
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

### AB-Archivus Agent

Dedicated OpenClaw agent for memory management:
- Reads/writes to Obsidian vault
- Updates entity database
- Processes session logs
- Maintains context summaries

### Obsidian Vault

Ready-to-use vault with:
- Entity templates (Person, Company, Topic)
- Folder structure for memory organization
- Nightly processing scripts
- Summary templates

## Installation

### Default Install

```bash
./setup.sh
```

This will:
1. Copy Obsidian vault to `/data/obsidian/AB-Memory-Vault/`
2. Install AB-Archivus agent to `~/.openclaw/agents/AB-Archivus/`
3. Register agent with OpenClaw
4. Setup nightly cron at 03:00 MSK

### Custom Paths

```bash
VAULT_DEST=/custom/path ./setup.sh
```

### Skip Cron

```bash
./setup.sh --skip-cron
```

## Entity Templates

### Person

```markdown
## Identity
- **Name:**
- **Role:**
- **Contact:**
- **Channel:**
- **Location:**

## Relations
- Connected to:

## Notes

## Timeline
- YYYY-MM-DD: First contact
```

### Company

```markdown
## Identity
- **Name:**
- **Industry:**
- **Website:**
- **Location:**
- **Size:**

## Relations
- Partners:
- Clients:

## Notes

## Timeline
```

### Topic

```markdown
## Identity
- **Name:**
- **Category:**
- **Tags:**

## Description

## Key Points

## Related Entities

## Resources

## Timeline
```

## Configuration

### Vault Location

Default: `/data/obsidian/AB-Memory-Vault/`

### Nightly Processing

Default: 03:00 MSK daily

To change:
```bash
crontab -e
# Change: 0 3 * * *
```

## Memory Workflow

```
┌─────────────────────────────────────────────────────┐
│                     AGENT                            │
│  ┌─────────────┐    ┌─────────────┐    ┌─────────┐ │
│  │ Start Session│───▶│ Read Memory │───▶│ Work    │ │
│  └─────────────┘    └──────┬──────┘    └────┬────┘ │
│                            │                  │      │
│                      ┌─────▼─────┐      ┌────▼────┐ │
│                      │Write Log  │      │ Decisions│ │
│                      └─────┬─────┘      └────┬────┘ │
│                            │                  │      │
│                      ┌─────▼──────────────────▼────┐ │
│                      │     End Session → Vault     │ │
│                      └──────────────────────────────┘ │
└─────────────────────────────────────────────────────┘
```

## Requirements

- OpenClaw 2024+
- Obsidian (optional, for vault editing)
- bash >= 4.0
- cron

## 📢 Links

- 🌐 **Канал AB Agents:** https://t.me/alexburr_agents
- 👤 **Автор:** https://t.me/AlexBurrOne
- 🐛 **Issues:** https://github.com/alexburrstudio/ab-agents-memory/issues
- 📦 **ClawHub:** https://clawhub.com/ab-agents-memory

💰 Support 

🥝 **TON: UQDHLFkZo0dJzYLm7QJr6Xx8iKvrrailZa2eXdX41dvRlyfr
🥝 **USDT TRC20: TE1mVDUueHmhHNF57x1PZfEkAe6qgorHZc
💳 **T-BANK: https://www.tbank.ru/cf/3CfaY0mpVIt

**AB Agents Memory** — Your second brain for OpenClaw 🦀
