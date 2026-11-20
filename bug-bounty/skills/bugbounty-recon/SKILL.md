---
name: bugbounty-recon
description: Bug bounty reconnaissance methodology covering passive recon, subdomain enumeration, DNS analysis, JS analysis, wayback, port scanning, fingerprinting, GitHub and Google dorks, Shodan, cloud and mobile recon, API discovery, and fuzzing. Use when the user starts recon, asks how to enumerate subdomains or discover assets, or needs a recon pipeline or checklist.
license: MIT
---

# Bug Bounty Recon

End-to-end recon methodology backed by the files below (paths relative to the
`BugBountySkills/` repo root).

## Methodology files

- `../../SKILL_FILES/RECON/01_passive_recon.md` through
  `../../SKILL_FILES/RECON/16_recon_automation_pipeline.md` — run in order:
  passive recon, subdomain enumeration, DNS analysis, asset discovery, JavaScript
  analysis, wayback history, port scanning, tech-stack fingerprinting, GitHub
  dorks, Google dorks, Shodan/Censys/FoFA, cloud recon (AWS/GCP/Azure), mobile
  recon, API discovery, content discovery/fuzzing, automation pipeline.
- `../../SKILL_FILES/AUTOMATION/recon_pipeline_automation.md`,
  `../../SKILL_FILES/AUTOMATION/monitoring_new_assets.md`,
  `../../SKILL_FILES/AUTOMATION/monitoring_scope_changes.md` — continuous recon.
- `../../CHECKLISTS/recon_passive.md`, `../../CHECKLISTS/recon_active.md`,
  `../../CHECKLISTS/recon_aws.md` — per-run checklists.

## How to work

1. Confirm scope and program policy before any active step.
2. Run passive sources first (subdomains, certs, wayback, GitHub), then active
   (DNS, ports, fuzzing) at low rate.
3. Track every asset and its source; feed live hosts into content discovery and
   JS analysis for endpoint extraction.
