---
name: bugbounty-reporting
description: Bug bounty report writing with HackerOne, Bugcrowd, and Intigriti templates, impact statements, CVSS severity rating, PoC documentation, remediation advice, and escalation/dispute templates. Use when the user needs to write up a finding, asks for a report template, needs a CVSS score, or wants to dispute a triage decision.
license: MIT
---

# Bug Bounty Reporting

Write reports that get triaged, not closed (paths relative to `BugBountySkills/`).

- `../../SKILL_FILES/REPORTING/report_writing_methodology.md` — start here.
- Templates: `../../SKILL_FILES/REPORTING/hackerone_report_template.md`, `../../SKILL_FILES/REPORTING/bugcrowd_report_template.md`,
  `../../SKILL_FILES/REPORTING/intigriti_report_template.md`, `../../SKILL_FILES/REPORTING/email_disclosure_template.md`.
- `../../SKILL_FILES/REPORTING/impact_statement_writing.md`, `../../SKILL_FILES/REPORTING/severity_rating_cvss.md`,
  `../../SKILL_FILES/REPORTING/poc_documentation.md`, `../../SKILL_FILES/REPORTING/remediation_advice.md`,
  `../../SKILL_FILES/REPORTING/escalation_dispute_templates.md`.
- `../../MASTER_SYSTEM_PROMPTS/` — model-specific hunting system prompts.

For opencode-native report generation, pair with the `bugbounty-reporter`
skill (triage gate plus submission-ready structure).
