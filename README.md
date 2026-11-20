# AI Security Skills

> **1,290+ production-ready Agent Skills** for bug bounty hunting, security engineering, secure development, design, and SaaS integrations — all following the open [Agent Skills](https://agentskills.io) standard (`SKILL.md` entrypoints).

![Skills](https://img.shields.io/badge/skills-1294%2B-blue.svg)
![License](https://img.shields.io/badge/license-MIT%20%2F%20Apache--2.0-green.svg)
![Format](https://img.shields.io/badge/format-Agent_Skills-SKILL.md-orange.svg)
![Claude Code](https://img.shields.io/badge/Claude_Code-compatible-purple.svg)
![Codex CLI](https://img.shields.io/badge/Codex_CLI-compatible-purple.svg)
![Cursor](https://img.shields.io/badge/Cursor-compatible-purple.svg)
![Gemini CLI](https://img.shields.io/badge/Gemini_CLI-compatible-purple.svg)

---

## ⚠️ Authorized Use Only

This repository contains offensive-security knowledge intended for **legal, authorized** work only: bug bounty programs with explicit scope, penetration testing engagements you are contracted for, CTF competitions, and defending your own systems. Anything else is your own responsibility and likely a crime. Act accordingly.

---

## What's Inside

```
ai-security-skills/
├── agent-skills/
│   ├── security/          # 143 skills — bug bounty methodology, recon, web/mobile/cloud exploitation, OSINT
│   ├── development/       # 204 skills — code review, TDD, debugging, architecture, CI/CD, agent workflows
│   ├── design/            #  10 skills — UI/UX, design systems, branding, slides
│   ├── official/          #  13 skills — Anthropic's open-source skills (Apache-2.0)
│   └── integrations/      # 864 skills — one skill per SaaS/API (Composio collection)
├── bug-bounty/            # Bug bounty vault: 630+ knowledge files, checklists, payloads, system prompts
├── security/              # Security engineering collection: 50 framework-grounded skills
├── SKILLS-INDEX.md        # Every skill listed with its description
├── ATTRIBUTION.md         # Sources and licenses for every included collection
└── LICENSE
```

### By category

| Category | Skills | Highlights |
|---|---|---|
| `agent-skills/security/` | 143 | Recon pipelines · XSS · SQLi · SSRF · SSTI · IDOR · JWT/OAuth attacks · business logic · subdomain takeover · mobile (APK) analysis · cloud misconfig · OSINT · bug bounty reporting |
| `agent-skills/development/` | 204 | Secure code review · threat modeling · TDD · debugging · architecture · Git workflows · delegation · agent discipline (superpowers, caveman, pstack) |
| `agent-skills/design/` | 10 | UI/UX pro · design systems · branding · slide decks |
| `agent-skills/official/` | 13 | Anthropic reference skills: `mcp-builder`, `skill-creator`, `claude-api`, `webapp-testing`, `theme-factory`, … |
| `agent-skills/integrations/` | 864 | One `SKILL.md` per service — Stripe, Slack, Notion, AWS, Google Workspace, GitHub, Zapier-style automations, 800+ more |
| `bug-bounty/` | 630+ files | `SKILL_FILES/` (recon, web/API/mobile/LLM/infra vulns, payloads, automation, reporting) · 380-file `KNOWLEDGE_BASE/` · 51 operational checklists · drop-in system prompts |
| `security/` | 50 | OWASP / NIST / MITRE ATT&CK / CIS-grounded skills across appsec, cloud, devsecops, identity, IR, secops, vuln management + SOC role playbooks |

**Full browsable list with descriptions → [SKILLS-INDEX.md](SKILLS-INDEX.md)**

---

## Quick Start

### Claude Code

```bash
git clone https://github.com/abdelrhmansleem/ai-security-skills.git
cd ai-security-skills

# All skills, globally (auto-discovery + /skill-name)
cp -r agent-skills/*/*/ ~/.claude/skills/
cp -r security/skills/*/* ~/.claude/skills/

# Or project-local
mkdir -p .claude/skills && cp -r agent-skills/*/*/ .claude/skills/
```

Then just ask naturally — e.g. *"hunt IDOR on this API"* loads the IDOR skill, or call it directly: `/13-xss`.

### Codex CLI / Other agents

```bash
codex --context agent-skills/security/15-ssrf/SKILL.md "Audit this endpoint"
```

### Cursor / Gemini CLI

```bash
cp -r agent-skills/ .cursor/rules/     # Cursor
cp -r agent-skills/ ~/.gemini/skills/  # Gemini CLI
```

Every skill is a self-contained directory with a `SKILL.md` file (YAML frontmatter: `name`, `description`, optional `tags`) plus optional scripts and references — the open [Agent Skills](https://agentskills.io) standard. Any agent that reads markdown can load them.

---

## The Bug Bounty Vault

`bug-bounty/` is a complete hunting knowledge system — 630+ markdown files, ~76k lines:

- **Load into any LLM** and it becomes a context-aware bug bounty partner: name the vuln class and target context, and you get working payloads, bypass techniques, copy-paste recon pipelines, and severity-calculated report drafts — not Wikipedia summaries.
- **Use without AI** as a standalone reference vault.
- Includes `MASTER_SYSTEM_PROMPTS/` with drop-in prompts for Claude, ChatGPT, Copilot, and local models.

Start at [`bug-bounty/README.md`](bug-bounty/README.md) and [`bug-bounty/INDEX.md`](bug-bounty/INDEX.md).

---

## Why Structured Skills (Not Prompt Dumps)

Generic prompting makes agents hallucinate framework control numbers, skip vulnerability classes, and produce inconsistent output. These skills ground the agent in published frameworks (OWASP, NIST, MITRE ATT&CK, CIS) and repeatable methodologies, so the same question produces the same auditable result every run.

---

## Attribution

Every third-party collection in this repo keeps its original license and is credited in **[ATTRIBUTION.md](ATTRIBUTION.md)** — including [anthropics/skills](https://github.com/anthropics/skills), [ComposioHQ/awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills), [obra/superpowers](https://github.com/obra/superpowers), [OWASP/secure-agent-playbook](https://github.com/OWASP/secure-agent-playbook), and 20+ more.

## License

The repository organization and original content are **MIT** — see [LICENSE](LICENSE). Third-party skills carry their original licenses (MIT / Apache-2.0 / CC-BY-4.0), documented per collection in [ATTRIBUTION.md](ATTRIBUTION.md).

## Disclaimer

This material is provided for **educational and authorized security testing purposes only**. The maintainers are not responsible for misuse. If you break the law with this content, that's on you.
