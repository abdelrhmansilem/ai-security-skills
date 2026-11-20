---
name: bugbounty-web
description: Web vulnerability hunting covering XSS, SQLi, SSRF, SSTI, XXE, IDOR, auth bypass, OAuth, JWT, CORS, CSRF, race conditions, request smuggling, file upload, and WAF bypass, with payloads for every class. Use when the user hunts web bugs, asks for payloads, needs exploitation steps for a web vuln class, or wants a per-vuln testing checklist.
license: MIT
---

# Bug Bounty Web Vulnerabilities

Web hunting guides plus ready payloads (paths relative to `BugBountySkills/`).

## Vulnerability guides

All files under `../../SKILL_FILES/VULNERABILITIES/WEB/` — highlights:
`../../SKILL_FILES/VULNERABILITIES/WEB/xss_reflected_stored_dom.md`, `../../SKILL_FILES/VULNERABILITIES/WEB/sqli_all_types.md`, `../../SKILL_FILES/VULNERABILITIES/WEB/ssrf_all_types.md`,
`../../SKILL_FILES/VULNERABILITIES/WEB/ssti_all_engines.md`, `../../SKILL_FILES/VULNERABILITIES/WEB/xxe_all_types.md`, `../../SKILL_FILES/VULNERABILITIES/WEB/idor_bola_bfla.md`,
`../../SKILL_FILES/VULNERABILITIES/WEB/auth_bypass_all_types.md`, `../../SKILL_FILES/VULNERABILITIES/WEB/account_takeover_chains.md`,
`../../SKILL_FILES/VULNERABILITIES/WEB/2fa_mfa_bypass.md`, `../../SKILL_FILES/VULNERABILITIES/WEB/jwt_attacks.md`, `../../SKILL_FILES/VULNERABILITIES/WEB/oauth_misconfig.md`,
`../../SKILL_FILES/VULNERABILITIES/WEB/cors_misconfig.md`, `../../SKILL_FILES/VULNERABILITIES/WEB/csrf_all_types.md`, `../../CHECKLISTS/race_conditions.md`,
`http_request_smuggling.md`, `../../SKILL_FILES/VULNERABILITIES/WEB/file_upload_bypass.md`,
`../../SKILL_FILES/VULNERABILITIES/WEB/waf_bypass_all_techniques.md`, `../../SKILL_FILES/VULNERABILITIES/WEB/rce_all_vectors.md`, and more.

## Payloads

All files under `../../SKILL_FILES/PAYLOADS/`:
`../../SKILL_FILES/PAYLOADS/xss_payloads_all_contexts.md`, `../../SKILL_FILES/PAYLOADS/sqli_payloads_all_dbs.md`,
`../../SKILL_FILES/PAYLOADS/ssrf_payloads_bypasses.md`, `../../SKILL_FILES/PAYLOADS/ssti_payloads_all_engines.md`,
`../../SKILL_FILES/PAYLOADS/xxe_payloads.md`, `../../SKILL_FILES/PAYLOADS/rce_payloads_all_langs.md`, `../../SKILL_FILES/PAYLOADS/jwt_exploit_payloads.md`,
`../../SKILL_FILES/PAYLOADS/lfi_payloads_wrappers.md`, `../../SKILL_FILES/PAYLOADS/waf_bypass_payloads.md`,
`../../SKILL_FILES/PAYLOADS/polyglot_payloads.md`, `../../SKILL_FILES/PAYLOADS/open_redirect_payloads.md`, `../../SKILL_FILES/PAYLOADS/csrf_payloads.md`,
`../../SKILL_FILES/PAYLOADS/deserialization_payloads.md`, `../../SKILL_FILES/PAYLOADS/prototype_pollution_payloads.md`,
`../../SKILL_FILES/PAYLOADS/prompt_injection_payloads.md`.

## Checklists and writeups

`../../CHECKLISTS/xss.md`, `../../CHECKLISTS/sqli.md`, `../../CHECKLISTS/ssrf.md`, `../../CHECKLISTS/ssti.md`, `../../CHECKLISTS/idor.md`, `../../CHECKLISTS/jwt.md`,
`../../CHECKLISTS/oauth.md`, `../../CHECKLISTS/cors.md`, `../../CHECKLISTS/csrf.md`, `../../CHECKLISTS/open_redirect.md`, `../../CHECKLISTS/file_upload.md`,
`../../CHECKLISTS/deserialization.md`, `../../CHECKLISTS/race_conditions.md`, `../../CHECKLISTS/cache_poisoning.md`,
`../../CHECKLISTS/clickjacking.md`, `../../CHECKLISTS/auth_bypass.md`, plus `../../CHECKLISTS/checklist_pack_2/`.
Worked examples live in `../../KNOWLEDGE_BASE/` (e.g. `../../KNOWLEDGE_BASE/ssti_jinja2_rce.md`,
`../../KNOWLEDGE_BASE/server-side_request_forgery_imds.md`, `../../KNOWLEDGE_BASE/race_condition_single-packet_attack.md`).
