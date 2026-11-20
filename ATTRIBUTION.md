# Attribution

This repository aggregates agent skills from multiple open-source collections. Every source is credited below with its license and the number of skills included. Where a source has its own `LICENSE` file, it is preserved inside its directory.

## Top-level collections

| Directory | Source | License | Contents |
|---|---|---|---|
| `bug-bounty/` | [0xN0RMXL/BugBountySkills](https://github.com/0xN0RMXL/BugBountySkills) | MIT (kept in directory) | Bug bounty vault — 630+ knowledge files, checklists, payloads, system prompts, 10 skills |
| `security/` | [UnitOneAI/SecuritySkills](https://github.com/UnitOneAI/SecuritySkills) | MIT (kept in directory) | 50 framework-grounded security engineering skills |

## agent-skills/

| Source | License | Skills |
|---|---|---|
| [ComposioHQ/awesome-claude-skills](https://github.com/ComposioHQ/awesome-claude-skills) | Apache-2.0 (per upstream README) | 864 |
| [elementalsouls/Claude-BugHunter](https://github.com/elementalsouls/Claude-BugHunter) | MIT | 83 |
| [painhardcore/pstack](https://github.com/painhardcore/pstack) | MIT | 41 |
| [mattpocock/skills](https://github.com/mattpocock/skills) | MIT | 36 |
| [0xGhostCAT/claude-ai-cyber-security-skills](https://github.com/0xGhostCAT/claude-ai-cyber-security-skills) | MIT | 30 |
| [addyosmani/agent-skills](https://github.com/addyosmani/agent-skills) | MIT | 25 |
| [michael-denyer/pstack-claude](https://github.com/michael-denyer/pstack-claude) | MIT | 22 |
| [JuliusBrussee/caveman](https://github.com/JuliusBrussee/caveman) | Apache-2.0 | 22 |
| local collection (maintained in this repo) | MIT | 21 |
| [amElnagdy/delegate-skills](https://github.com/amElnagdy/delegate-skills) | MIT | 20 |
| [obra/superpowers](https://github.com/obra/superpowers) | MIT | 15 |
| [anthropics/skills](https://github.com/anthropics/skills) | Apache-2.0 | 13 |
| [Egonex-AI/Understand-Anything](https://github.com/Egonex-AI/Understand-Anything) | MIT | 9 |
| [nextlevelbuilder/ui-ux-pro-max-skill](https://github.com/nextlevelbuilder/ui-ux-pro-max-skill) | MIT | 7 |
| [DietrichGebert/ponytail](https://github.com/DietrichGebert/ponytail) | MIT | 6 |
| [tt-a1i/archify](https://github.com/tt-a1i/archify) | MIT | 5 |
| [amElnagdy/guard-skills](https://github.com/amElnagdy/guard-skills) | MIT | 5 |
| [pbakaus/impeccable](https://github.com/pbakaus/impeccable) | Apache-2.0 | 2 |
| [instavm/open-skills](https://github.com/instavm/open-skills) | Apache-2.0 | 2 |
| [amElnagdy/review-skills](https://github.com/amElnagdy/review-skills) | MIT | 2 |
| [OWASP/secure-agent-playbook](https://github.com/OWASP/secure-agent-playbook) | CC-BY-4.0 | 2 |
| [cloudflare/security-audit-skill](https://github.com/cloudflare/security-audit-skill) | MIT | 1 |
| [HSSkyBoy/apk-reverse](https://github.com/HSSkyBoy/apk-reverse) | MIT | 1 |
| [Graphify-Labs/graphify](https://github.com/Graphify-Labs/graphify) | Apache-2.0 | 1 |

**Total: ≈1,234 agent skills** + the two top-level collections above.

## Notes

- Anthropic's document-creation skills (`docx`, `pdf`, `pptx`, `xlsx`) are **source-available, not open source**, and are therefore **excluded** from this repository. Only Apache-2.0 skills from `anthropics/skills` are included under `agent-skills/official/`.
- Skills were deduplicated by name during aggregation; where the same skill existed in multiple sources, the first source listed above won.
- If you are a source owner and want your collection removed or re-credited differently, open an issue.
