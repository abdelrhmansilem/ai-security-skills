# Skill Index

Every skill in this repository, grouped by category. Each skill lives in its own directory with a `SKILL.md` entrypoint.

### Security (agent-skills/security) — 143 skills

| Skill | Description |
|---|---|
| `01-program-selection` | Evaluate HackerOne / Bugcrowd / Intigriti programs before committing time. Decide signal-to-noise, payout history, response time, scope size, and c... |
| `02-scope-analysis` | Parse HackerOne / Bugcrowd / Intigriti scope into a structured asset list with in-scope, out-of-scope, and excluded-vuln-class breakdowns. Use when... |
| `03-threat-modeling-mindmap` | Build a mental and visual map of the target application before hunting — entry points, trust boundaries, data flows, and high-value functionality. ... |
| `04-subdomain-enum` | Enumerate subdomains using passive and active techniques (subfinder, amass, chaos, assetfinder, crtsh, DNS brute force). Use when the user has a ro... |
| `05-asset-discovery` | Probe subdomain list with httpx/dnsx/naabu to identify live hosts, open ports, status codes, titles, and basic fingerprints. Use after subdomain-en... |
| `06-fingerprinting` | Identify exact technology stack, frameworks, versions, and CMS on live hosts. Use when the user has a live host list and needs to know what's runni... |
| `07-js-analysis` | Extract endpoints, secrets, and hidden routes from JavaScript files using LinkFinder, SecretFinder, JSluice, and source-map analysis. Use when the ... |
| `08-content-discovery` | Fuzz directories, files, and parameters using ffuf, feroxbuster, arjun, paramspider, and x8. Use when the user has live hosts and needs to find hid... |
| `09-continuous-monitoring` | Set up nightly monitoring of subdomain changes, JS file diffs, new endpoints, and CVE matches against in-scope assets, with Discord/Slack/Telegram ... |
| `10-idor-hunting` | Hunt Insecure Direct Object Reference (IDOR) — test horizontal and vertical privilege escalation across user IDs, org IDs, tenant boundaries, and u... |
| `11-auth-bypass` | Hunt authentication and authorization bypasses — forced browsing, path traversal in auth, header injection, JWT downgrade, OAuth state confusion, r... |
| `12-ato-chains` | Hunt full Account Takeover (ATO) by chaining lower-severity findings — IDOR-to-email-disclosure, password-reset-token-theft, OAuth-redirect-uri abu... |
| `13-xss` | Hunt reflected, stored, and DOM-based Cross-Site Scripting (XSS) including CSP bypass, polyglot payloads, mutation XSS (mXSS), markdown XSS, and te... |
| `14-sqli` | Hunt SQL injection in REST/GraphQL/SOAP/raw parameters using sqlmap, ghauri, manual UNION/Time/Boolean techniques, and custom WAF-bypass tamper scr... |
| `15-ssrf` | Hunt Server-Side Request Forgery (SSRF) — internal network access, cloud metadata exploitation, gopher/file/dict protocol abuse, and 11 IP-filter b... |
| `16-ssti` | Hunt Server-Side Template Injection (SSTI) in Jinja2, Twig, Freemarker, Velocity, Smarty, ERB, Handlebars, Mustache, and Spring (SpEL). Use when in... |
| `17-file-upload` | Hunt file upload vulnerabilities — bypass content-type/extension/magic-byte/size filters, achieve XSS via SVG/HTML upload, achieve RCE via .phtml/.... |
| `18-graphql` | Hunt GraphQL-specific vulns — introspection abuse, field-level authorization (IDOR), batched queries for brute force, alias-based rate limit bypass... |
| `19-jwt-attacks` | Hunt JSON Web Token (JWT) vulnerabilities — alg=none bypass, RS256→HS256 key confusion, weak HMAC secret cracking, kid path traversal, JWKS injecti... |
| `20-oauth-oidc` | Hunt OAuth 2.0 and OIDC flaws — redirect_uri abuse, state CSRF, PKCE bypass, scope manipulation, implicit-flow token theft, postMessage origin tric... |
| `21-business-logic` | Hunt business logic flaws — race conditions, workflow state bypass, parameter pollution affecting logic, coupon/discount abuse, refund logic, multi... |
| `22-subdomain-takeover` | Detect and exploit subdomain takeover via dangling DNS records pointing to deprovisioned cloud services (S3, GitHub Pages, Heroku, Azure, Shopify, ... |
| `23-cache-poisoning` | Hunt web cache poisoning, CDN cache poisoning, and cache deception attacks. Use when target uses a CDN (Cloudflare, Akamai, Fastly, AWS CloudFront)... |
| `24-http-smuggling` | Hunt HTTP Request Smuggling (CL.TE, TE.CL, TE.TE, H2.CL, H2.TE, downgrade smuggling). Use when target is behind a reverse proxy / load balancer / C... |
| `25-llm-ai-security` | Hunt vulnerabilities in LLM-powered applications — direct/indirect prompt injection, system prompt extraction, ASCII smuggling, RCE via code tools,... |
| `26-mobile-recon-android` | Mobile (Android) app recon and analysis — decompile APK, extract secrets, find hardcoded endpoints, exposed Firebase / AWS / API keys, deeplink abu... |
| `27-cloud-misconfig` | Hunt cloud misconfigurations exposed externally — open S3/GCS buckets, exposed IAM-tied EC2 metadata, Cognito misconfig, GitHub Actions secret leak... |
| `28-triage-validation` | Validate a bug bounty finding before writing a report — the 7-Question Gate, 4 pre-submission gates, always-rejected list, conditional chain table,... |
| `29-hackerone-reporting` | Write production-grade HackerOne reports — title formula, impact-led writing, CVSS 3.1 scoring, complete PoC formatting, attached files, and submis... |
| `30-bugcrowd-reporting` | Write Bugcrowd-format reports — VRT (Vulnerability Rating Taxonomy) mapping, P1-P5 severity, impact-led writing, and Bugcrowd-specific submission e... |
| `active-directory` | (no description in frontmatter) |
| `apk-redteam-pipeline` | End-to-end Android APK red-team pipeline — automated APK acquisition (Play Store + apkpure + apkmirror fallback), jadx decompilation, secret/URL/JW... |
| `apk-reverse` | Unified reverse engineering toolkit covering Android APK decompilation, |
| `bb-local-toolkit` | Local-tooling companion to the bug-bounty orchestrator — carries the SAME complete bug-bounty workflow, but reach for THIS variant when you also ne... |
| `bb-methodology` | Use at the START of any bug bounty hunting session, when switching targets, or when feeling lost about what to do next. Master orchestrator that co... |
| `blue-team` | (no description in frontmatter) |
| `bug-bounty` | Complete bug bounty workflow — recon (subdomain enumeration, asset discovery, fingerprinting, HackerOne scope, source code audit), pre-hunt learnin... |
| `bug-bounty-hunter` | (no description in frontmatter) |
| `bugcrowd-reporting` | "Bugcrowd-specific reporting tactics complementing report-writing: VRT category search-and-fallback strategy when no exact match exists, manual sev... |
| `clean-code-guard` | Review generated or changed production code before it ships, using Clean Code, SOLID, DRY, KISS, YAGNI, and LLM-specific failure-mode checks in any... |
| `cloud-iam-deep` | Cloud IAM red-team attack chain across AWS, Azure, GCP — focused on EXTERNAL exploitation paths and post-credential-discovery privilege analysis. C... |
| `cloud-security` | (no description in frontmatter) |
| `code-review` | (no description in frontmatter) |
| `cpp-security` | (no description in frontmatter) |
| `ctf-solver` | (no description in frontmatter) |
| `docs-guard` | "Review generated or changed documentation before it ships — READMEs, API references, docstrings, PHPDoc/JSDoc, changelogs, tutorials, and doc site... |
| `enterprise-vpn-attack` | External SSL VPN / remote-access appliance attack matrix — Cisco ASA/AnyConnect, Fortinet FortiGate/FortiOS, Citrix NetScaler/ADC, Palo Alto Global... |
| `evidence-hygiene` | "Evidence-capture and PoC-redaction discipline for bug-bounty submissions: cookie redaction protocol (which fields to mask, Preview annotation / Bu... |
| `hunt-api-misconfig` | "Hunt API security misconfiguration — mass assignment, prototype pollution, HTTP verb tampering. Mass assignment: send {is_admin:true, role:admin, ... |
| `hunt-aspnet` | Hunt ASP.NET-specific surface — ViewState deserialization (signed-only vs encrypted), machineKey recovery, dual-parser MAC-bypass anti-pattern, req... |
| `hunt-ato` | "Hunt account takeover taxonomy — 9 distinct paths to ATO, plus chains. Paths: (1) password reset flaws (host-header injection redirects token, pre... |
| `hunt-auth-bypass` | Hunting skill for auth bypass vulnerabilities. Built from 12 public bug bounty reports across SAML XSW / parser-differential (GitHub Enterprise CVE... |
| `hunt-brute-force` | "Hunt Missing/Weak Rate Limiting — login brute force, OTP/2FA brute force (10^6 keyspace), password-reset-token brute, credential stuffing, usernam... |
| `hunt-business-logic` | Hunting skill for business logic vulnerabilities. Built from 12 public bug bounty reports. Covers coupon-race-stacking (Instacart, Stripe, Reverb),... |
| `hunt-cache-poison` | Hunting skill for cache poison vulnerabilities. Built from 10 public bug bounty reports including X-Forwarded-Host poisoning, X-HTTP-Method-Overrid... |
| `hunt-captcha-bypass` | "Hunt CAPTCHA Bypass — 6 distinct patterns: (1) CAPTCHA field simply omitted from the request (server-side validation absent), (2) CAPTCHA token re... |
| `hunt-cicd` | "Hunt CI/CD pipeline vulnerabilities — GitHub Actions workflow injection (pull_request_target Pwnrequest + ${{ }}-into-shell), self-hosted runner p... |
| `hunt-clickjacking` | "Hunt Clickjacking — missing X-Frame-Options / CSP frame-ancestors lets an attacker embed the target page in an invisible iframe and trick victims ... |
| `hunt-cloud-misconfig` | "Hunt cloud / infrastructure misconfigurations. AWS: public S3 buckets (s3:GetObject anonymous), permissive bucket policies (PutObjectAcl public-wr... |
| `hunt-cors` | "Hunt CORS Misconfiguration — origin-reflection with credentials, null-origin trust, subdomain-regex bypass (unanchored vs unescaped-dot vs prefix-... |
| `hunt-csrf` | Hunting skill for csrf vulnerabilities. Built from 15 public bug bounty reports including modern variants — SameSite=Lax sibling-subdomain bypass (... |
| `hunt-deserialization` | Hunt Insecure Deserialization — Java gadget chains (ysoserial), PHP object injection (phpggc), Python pickle RCE, .NET BinaryFormatter, Ruby Marsha... |
| `hunt-dispatch` | Skill-set loader for /hunt orchestrator. Fingerprints the target, picks the right platform attack skills, and loads the Red Team or WAPT skill set.... |
| `hunt-dom` | "Hunt client-side DOM vulnerabilities — DOM Clobbering (overwrite JS globals via HTML injection), PostMessage hijacking (missing origin check), Ser... |
| `hunt-exceptional-conditions` | "Hunt mishandling of exceptional conditions — feed an endpoint malformed/unexpected input (wrong type, broken JSON, oversized field, null byte) and... |
| `hunt-file-upload` | "Hunt file upload bugs — RCE via webshell, XSS via SVG/HTML, SSRF via XXE in DOCX, path traversal via filename. Bypass tables (10 techniques): doub... |
| `hunt-fintech-graphql` | "Hunt fintech-specific GraphQL vulnerabilities: money-movement mutations (transfers, redemptions, withdrawals, card top-ups), ledger/balance/portfo... |
| `hunt-forgot-password` | "Hunt Forgot Password / Account Recovery Authentication Flaws — 5 distinct patterns: (1) username enumeration via different responses for valid vs ... |
| `hunt-graphql` | Hunting skill for graphql vulnerabilities. Built from 12 public bug bounty reports across IDOR via node() / GID, mutation IDOR including AI/LLM fea... |
| `hunt-grpc` | "Hunt gRPC vulnerabilities — server reflection enabled (enumerate all services/methods), missing authentication / metadata-stripping on internal en... |
| `hunt-host-header` | "Hunt Host Header Injection — password reset poisoning → ATO, web cache poisoning via unkeyed Host/X-Forwarded-Host, routing-based SSRF (Host picks... |
| `hunt-html-injection` | "Hunt HTML Injection — user-supplied input is rendered as raw HTML in the response without sanitisation, allowing an attacker to inject arbitrary H... |
| `hunt-http-smuggling` | "Hunt HTTP request smuggling (CL.TE, TE.CL, H2.CL, H2.TE). Cause: front-end proxy and back-end server disagree on where one request ends and the ne... |
| `hunt-idor` | Hunting skill for idor vulnerabilities. Built from 26 public bug bounty reports. Use when hunting idor on any target. |
| `hunt-jwt-crypto` | "Hunt JWT cryptographic failures — alg:none signature-stripping and RS256→HS256 key-confusion that let an attacker forge a token for any identity (... |
| `hunt-k8s` | "Hunt Kubernetes & Docker — API anonymous access, kubelet 10250 exec (SPDY/WebSocket, NOT plain POST) and the simpler /run primitive, etcd 2379 una... |
| `hunt-laravel` | Hunt Laravel specific vulnerabilities — Debug mode leakage (APP_DEBUG=true exposes full stack trace + env vars), Laravel Telescope/Horizon dashboar... |
| `hunt-ldap` | "Hunt LDAP Injection and XPath Injection — authentication bypass, blind char-by-char attribute exfiltration, AD user/group enumeration, XML-store X... |
| `hunt-lfi` | "Hunt Local File Inclusion (LFI), Remote File Inclusion (RFI), and Path Traversal — /etc/passwd read, log poisoning → RCE, PHP filter-chain RCE (no... |
| `hunt-llm-ai` | "Hunt LLM/AI feature bugs — prompt injection, indirect injection, exfiltration via tool-use/markdown, ASCII smuggling, agentic AI security (OWASP A... |
| `hunt-mfa-bypass` | "Hunt MFA / 2FA bypass — 7 distinct patterns. (1) MFA not enforced on sensitive endpoints (password change, email change accept without MFA challen... |
| `hunt-misc` | Hunting skill for misc vulnerabilities. Built from 225 public bug bounty reports. Use when hunting misc on any target. |
| `hunt-nextjs` | Hunt Next.js specific vulnerabilities — Server Actions arbitrary function execution, Middleware auth bypass via static asset paths, ISR cache poiso... |
| `hunt-nodejs` | Hunt Node.js specific vulnerabilities — Prototype Pollution → RCE chains (lodash/merge/assign), Express trust proxy misconfiguration, child_process... |
| `hunt-nosqli` | Hunt NoSQL Injection — MongoDB operator injection ($where, $regex, $gt, $ne), CouchDB, Redis command injection, auth bypass via NoSQLi, data dump. ... |
| `hunt-ntlm-info` | "Hunt NTLM/Negotiate information disclosure on internet-reachable IIS/SharePoint/Exchange. Anonymous NTLM Type-2 challenge capture leaks NetBIOS do... |
| `hunt-oauth` | Hunting skill for oauth vulnerabilities. Built from 19 public bug bounty reports. Use when hunting oauth on any target. |
| `hunt-open-redirect` | Hunt Open Redirect — all types including low-impact, chained to OAuth token theft → ATO, phishing chains. URL parameter manipulation, JavaScript re... |
| `hunt-race-condition` | Hunting skill for race condition vulnerabilities. Built from 12 public bug bounty reports including modern HTTP/2 single-packet attack cases (James... |
| `hunt-rag-vector` | "Hunt vector-store / embedding-layer weaknesses in RAG pipelines (OWASP LLM08 Vector and Embedding Weaknesses) — persistent corpus poisoning that s... |
| `hunt-rce` | Hunting skill for rce vulnerabilities. Built from 67 public bug bounty reports. Use when hunting rce on any target. |
| `hunt-saml` | "Hunt SAML / SSO attacks. Patterns: XML Signature Wrapping (XSW) — modify Assertion while keeping Signature valid by relocating signed element, com... |
| `hunt-session` | "Hunt Session Management vulnerabilities — session fixation (no regeneration on login), insufficient invalidation on logout / password-change / ema... |
| `hunt-shadow-api` | "Hunt shadow / zombie / undocumented API surface (OWASP API9 Improper Inventory Management) — enumerate the full API version history (v1/v2/beta/le... |
| `hunt-sharepoint` | Hunt Microsoft SharePoint Server (2013/2016/2019/Subscription Edition) on-prem farms — anonymous endpoint enumeration, version disclosure, legacy S... |
| `hunt-source-leak` | Hunt source code and build artifact leakage — JavaScript source maps (.js.map) reconstructing TypeScript/ES6 source, Swagger/OpenAPI JSON endpoint ... |
| `hunt-spa-api` | Discover a single-page-app's hidden backend API from its public JS bundle, then test that API for broken access control / missing authentication. O... |
| `hunt-springboot` | Hunt Spring Boot specific vulnerabilities — Actuator endpoints (heapdump, env, loggers, mappings, shutdown), Spring Expression Language (SpEL) inje... |
| `hunt-sqli` | Hunting skill for sqli vulnerabilities. Built from 12 public bug bounty reports including modern NoSQL injection (Rocket.Chat CVE-2021-22911 MongoD... |
| `hunt-ssrf` | Hunting skill for ssrf vulnerabilities. Built from 15 public bug bounty reports including AWS metadata SSRF (HackerOne $25k Analytics PDF, Shopify ... |
| `hunt-ssti` | "Hunt server-side template injection (SSTI) across Jinja2 (Flask/Django), Twig (Symfony), Freemarker (Java), ERB (Rails), Spring, Velocity, Mako, T... |
| `hunt-subdomain` | Hunting skill for subdomain takeover vulnerabilities. Includes modern provider fingerprints — Microsoft Azure DevOps `cloudapp.azure.com` regional-... |
| `hunt-tls-network` | "Hunt TLS/SSL and DNS misconfigurations — missing HSTS (downgrade attack), weak cipher suites, expired/invalid certificates, mTLS bypass, missing S... |
| `hunt-websocket` | "Hunt WebSocket vulnerabilities — Cross-Site WebSocket Hijacking (CSWSH), missing/weak Origin validation on the WS handshake, no per-message authen... |
| `hunt-xss` | Hunting skill for xss vulnerabilities. Built from 174 public bug bounty reports. Use when hunting xss on any target. For markup injection that refl... |
| `hunt-xxe` | Hunting skill for xxe vulnerabilities. Built from 10 public bug bounty reports including SVG-upload XXE, Office-doc (PPTX/DOCX) XXE, SOAP XXE, SAML... |
| `incident-response` | (no description in frontmatter) |
| `ios-redteam-pipeline` | End-to-end iOS red-team pipeline — IPA acquisition (App Store extraction, TestFlight, enterprise/ad-hoc sideload), class-dump/Hopper/Ghidra static ... |
| `linux-privesc` | (no description in frontmatter) |
| `m365-entra-attack` | Microsoft 365 / Entra ID red-team attack chain — current 2026 reality. AADSTS code reference, user enumeration vectors (with hardening status), Sma... |
| `malware-analysis` | (no description in frontmatter) |
| `meme-coin-audit` | Meme coin and token security audit — rug pull detection (honeypot, hidden mint, fee manipulation, LP lock bypass), Solana SPL token analysis (freez... |
| `mid-engagement-ir-detection` | Methodology for detecting client SOC patches, attacker activity, and security-state changes that occur DURING a red-team engagement — and convertin... |
| `mobile-pentest` | (no description in frontmatter) |
| `multi-agentic-threat-model` | Comprehensive threat modeling for multi-agent systems using CSA MAESTRO 7-layer framework and OWASP Multi-Agentic System Threat Modeling Guide v1.0... |
| `offensive-osint` | "Operational arsenal for authorized external red-team and bug-bounty recon. Concrete probes, wordlists, regexes, dorks, curl one-liners for: subdom... |
| `okta-attack` | Okta-as-IdP red-team attack chain — tenant discovery, user enumeration (multiple vectors), authentication flow analysis (factors enumeration, push-... |
| `osint-methodology` | "Comprehensive OSINT methodology for external red-team operations and authorized attack-surface assessments. Covers the 5-stage recon pipeline (see... |
| `python-security` | (no description in frontmatter) |
| `recon-automation` | (no description in frontmatter) |
| `recon-scope-triage` | Triage ASM/recon output for ownership before testing — separate the target's real assets from namespace-collision noise. Automated recon keyword-ma... |
| `red-team` | (no description in frontmatter) |
| `redteam-mindset` | Red-team operator discipline — the mindset corrections that separate offensive testing from defensive WAPT. Built from authorized red-team work whe... |
| `redteam-report-template` | Client-facing red-team deliverable format — codifies the Subject / Observations / Description / Impact / Recommendation / PoC structure used for ex... |
| `report-writer` | (no description in frontmatter) |
| `report-writing` | Bug bounty report writing for H1/Bugcrowd/Intigriti/Immunefi — report templates, human tone guidelines, impact-first writing, CVSS 3.1 scoring, tit... |
| `reverse-engineering` | (no description in frontmatter) |
| `security-arsenal` | Security payloads, bypass tables, wordlists, gf pattern names, always-rejected bug list, and conditionally-valid-with-chain table. Use when you nee... |
| `security-audit` | Security guidance and vulnerability review for codebases, APIs, services, CLI tools, libraries, and daemons. Use for security questions, focused re... |
| `soc-analyst` | (no description in frontmatter) |
| `supply-chain-attack-recon` | External recon for software supply-chain attack surface — package-namespace squatting candidates, dependency-confusion vulnerabilities, GitHub Acti... |
| `template` | Replace with a clear description of what this skill does. Use when <the situations that should trigger it>. |
| `test-guard` | "Review generated or changed test code against universal testing rules before it ships. Best used reactively after an agent writes, edits, generate... |
| `threat-modeling` | (no description in frontmatter) |
| `triage-validation` | Finding validation before writing any report — 7-Question Gate (all 7 questions), 4 pre-submission gates, always-rejected list, conditionally valid... |
| `vmware-vcenter-attack` | VMware vSphere / vCenter Server external attack matrix — version fingerprinting, the high-impact CVE chain (CVE-2021-21972 vRealize unauth file upl... |
| `web-pentest` | (no description in frontmatter) |
| `web2-recon` | Web2 recon pipeline — subdomain enumeration (subfinder, Chaos API, assetfinder), live host discovery (dnsx, httpx), URL crawling (katana, waybackur... |
| `web3-audit` | Smart contract security audit — 10 DeFi bug classes (accounting desync, access control, incomplete path, off-by-one, oracle, ERC4626, reentrancy, f... |
| `windows-internals` | (no description in frontmatter) |
| `windows-privesc` | (no description in frontmatter) |
| `woo-guard` | "Review generated or changed WooCommerce code — extensions, payment and shipping integrations, checkout customizations, and order/product logic — b... |
| `wp-guard` | "Review generated or changed WordPress code — plugins, themes, and blocks — before it ships. Best used reactively after an agent writes, edits, or ... |

### Development & Engineering (agent-skills/development) — 204 skills

| Skill | Description |
|---|---|
| `agy-delegate` | Delegate a coding task to the Google Antigravity CLI (`agy`) as a background implementer, then review |
| `aider-delegate` | Delegate a coding task to Aider (`aider`) as a background implementer, then review its diff and land |
| `api-and-interface-design` | Guides stable API and interface design. Use when designing APIs, module boundaries, or any public interface. Use when creating REST or GraphQL endp... |
| `archify` | "Create validated architecture, workflow, sequence, data-flow, lifecycle/state, entity-relationship, class/interface, tree, timeline, and execution... |
| `archify-review` | Review Archify issues, PRs, or code through value, cost, and impact to support evidence-based maintenance decisions. Use for issue triage, change r... |
| `archify-tuning` | Improve Archify diagram accuracy, visual quality and complete authoring speed with fewer repairs. Use for generation experiments or evaluating chan... |
| `architect` | "Sketch types, signatures, and module structure before code, then stay in the loop while implementation fills in. Use for /architect, 'architect th... |
| `arena` | "Spawn N parallel candidates at the same task, pick a base, graft the strongest parts of the losers into it. Use for /arena, 'arena this', 'throw i... |
| `ask-matt` | Ask which skill or flow fits your situation. A router over the skills in this repo. |
| `audit` | a user-authored audit skill |
| `automate-me` | "Use for \"automate me\", \"create/update/refresh my -mode skill\", \"turn/capture my preferences or working style into a skill\", or wanting agent... |
| `babysit` | Watch an open PR — fix failing CI, handle the straightforward review comments, and drive it to a mergeable state. Claude Code analog of Cursor's bu... |
| `babysit-pr` | "Babysit a pull request through its bot review rounds: verify, fix, reply, resolve. Use for any babysit or watch-the-PR ask." |
| `benchmark-checklist` | "Vet a perf measurement (limiter, tuning, limits, errors, repeatability, relevance, and whether the work happened) before you report or act on it. ... |
| `blast-radius` | "Find what a change could break somewhere else before it ships, beyond the diff, and prove the one fact it's safe because of by running real code i... |
| `brainstorming` | "You MUST use this before any creative work - creating features, building components, adding functionality, modifying behavior, or planning anythin... |
| `bro` | Use when the user asks to restate or explain the last message in plain, jargon-free language. |
| `browser-testing-with-devtools` | Tests in real browsers via Chrome DevTools MCP. Use when building or debugging anything that runs in a browser. Use when you need to inspect the DO... |
| `cavecrew` | When to delegate to `cavecrew-investigator` (locate code), `cavecrew-builder` |
| `caveman` | Terse caveman voice: answer first, fluff gone, every technical fact kept. |
| `caveman-commit` | Write a Conventional Commits message compressed to intent only. Use for |
| `caveman-compress` | Compress a memory file such as CLAUDE.md or a todo list into caveman format |
| `caveman-discover` | Find and label every LLM workflow in the repository so Caveman Cloud groups |
| `caveman-evidence-review` | Read-only review of Caveman Cloud evidence: cost, Cave Score, workflows, |
| `caveman-explore` | Read-only repository explorer for cold-start orientation, broad cross-file localization, or when a direct search failed. Skip it when the exact fil... |
| `caveman-help` | Quick-reference card for the three caveman skills and their commands. |
| `caveman-learn` | Act on a Caveman learn report - review the ranked token sinks, apply cost-lowering fixes with per-edit consent, and report what those fixes returne... |
| `caveman-manage` | Inspect Caveman Cloud's experiment lifecycle and block unsafe execution. Use |
| `caveman-optimize` | Turn a Caveman optimization observation into an operator-chosen candidate |
| `caveman-review` | Compressed code review - one line per finding with location, problem and fix. |
| `caveman-setup` | Wire a repository through the Caveman Cloud gateway so every LLM request is |
| `caveman-stats` | Show recorded output and cache-read token usage and mode attribution for |
| `chief-of-staff` | Pursue a long-running goal in a single session by co-ordinating subagents. |
| `ci-cd-and-automation` | Automates CI/CD pipeline setup. Use when setting up or modifying build and deployment pipelines. Use when you need to automate quality gates, confi... |
| `claude-delegate` | Delegate a coding task to a separate Claude Code CLI process or another Claude session as an |
| `claude-handoff` | Hand the current conversation off to a fresh background agent that picks up the work immediately. |
| `cline-delegate` | Delegate a coding task to the Cline coding agent CLI (`cline`) as a background implementer, then |
| `code-review` | "Review the changes since a fixed point (commit, branch, tag, or merge-base) along two axes: Standards (does the code follow this repo's documented... |
| `code-review-and-quality` | Conducts multi-axis code review. Use before merging any change. Use when reviewing code written by yourself, another agent, or a human. Use when yo... |
| `code-simplification` | Simplifies code for clarity. Use when refactoring code for clarity without changing behavior. Use when code works but is harder to read, maintain, ... |
| `codebase-design` | Shared vocabulary for designing deep modules. Use when the user wants to design or improve a module's interface, find deepening opportunities, deci... |
| `codex-background` | Keep a Codex orchestrator's delegation to an installed delegate skill pending until its registered relay completes, without model-driven progress p... |
| `codex-delegate` | Delegate a coding task to the OpenAI Codex CLI as a background implementer, then review its diff and |
| `commandcode-delegate` | Delegate a coding task to the Command Code CLI (`cmd`) as a background implementer, then review its |
| `constraint-driven-development` | Establishes a project's quality bar as a written contract and stops agents quietly lowering it. Interviews the user on which dimensions matter, sup... |
| `context-engineering` | Optimizes agent context setup. Use when starting a new session, when agent output quality degrades, when switching between tasks, or when you need ... |
| `copilot-delegate` | Delegate a coding task to the GitHub Copilot CLI (`copilot`) as a background implementer, then |
| `correct` | "Find the mistakes agents keep repeating in this repo and make each one impossible. Try architecture first, then types, then a lint whose error nam... |
| `create-verification-skill` | "Generate a project-local verification skill that drives your app the way a user does — any language, framework, or platform. Use for /create-verif... |
| `cursor-delegate` | Delegate a coding task to the Cursor Agent CLI (`cursor-agent`) as a background implementer, then |
| `debate-review` | Two-model debate review of a GitHub PR, GitLab MR, Azure DevOps PR, or local working tree, posted as inline comments or printed. Use for any PR/MR ... |
| `debugging-and-error-recovery` | Guides systematic root-cause debugging. Use when tests fail, builds break, something that worked yesterday broke, behavior doesn't match expectatio... |
| `delegate-setup` | Configure delegation fleet lanes: which implementer CLI handles which kind of work, |
| `deprecation-and-migration` | Manages deprecation and migration. Use when removing old systems, APIs, or features. Use when migrating users from one implementation to another. U... |
| `deslop` | Remove AI-generated code slop and clean up code style |
| `diagnosing-bugs` | Diagnosis loop for hard bugs and performance regressions. Use when the user says "diagnose"/"debug this", or reports something broken/throwing/fail... |
| `diagnosing-superpowers` | Use when a superpowers session went wrong and your human partner wants to know why — repeated work, ignored plans, stumbles, poor results, a skill ... |
| `dispatching-parallel-agents` | Use when facing 2+ independent tasks that can be worked on without shared state or sequential dependencies |
| `documentation-and-adrs` | Records decisions and documentation. Use when you need to document an architecture decision (ADR) or the reasoning behind a design choice, when cha... |
| `domain-modeling` | Build and sharpen a project's domain model. Use when discussing codebase terminology, writing or editing a GLOSSARY.md, or recording or editing an ... |
| `doubt-driven-development` | Subjects every non-trivial decision to a fresh-context adversarial review before it stands. Use when you want every assumption cross-examined befor... |
| `executing-plans` | Use when executing an implementation plan in the current session as the implementer yourself — your human partner chose inline execution, or no sub... |
| `figure-it-out` | "Design an auditable playbook when no narrower one fits: a large migration, an ambitious multi-part change, or work a human reviews after stepping ... |
| `finishing-a-development-branch` | Use when implementation is complete, all tests pass, and you need to decide how to integrate the work |
| `fix-ci` | Find failing PR checks, inspect logs or external check links, and apply focused fixes |
| `fix-merge-conflicts` | Resolve merge conflicts non-interactively, validate build and tests, and finalize conflict resolution |
| `frontend-ui-engineering` | Builds production-quality, accessible, responsive user-facing UIs. Use when building or modifying interfaces and pages, creating components, implem... |
| `get-pr-comments` | Fetch and summarize review comments from the active pull request |
| `git-guardrails-claude-code` | Set up Claude Code hooks to block dangerous git commands (push, reset --hard, clean, branch -D, etc.) before they execute. Use when user wants to p... |
| `git-workflow-and-versioning` | Structures git workflow practices. Use when making any code change. Use when committing, branching, resolving conflicts, splitting uncommitted work... |
| `grill-me` | A relentless interview to sharpen a plan or design. |
| `grill-with-docs` | A relentless interview to sharpen a plan or design, which also creates docs (ADR's and glossary) as we go. |
| `grilling` | Grill the user relentlessly about a plan, decision, or idea. Use when the user wants to stress-test their thinking, or uses any 'grill' trigger phr... |
| `grok-delegate` | Delegate a coding task to the Grok Build CLI as a background implementer, then review its diff and |
| `handoff` | Compact the current conversation into a handoff document for another agent to pick up. |
| `how` | Explain how a subsystem works, trace a runtime flow, or determine where code and ownership belong before making a change. |
| `image-crop-rotate` | Image processing skill for cropping images to 50% from center and rotating them 90 degrees clockwise. This skill should be used when users request ... |
| `impeccable` | "Use when the user wants to design, redesign, shape, critique, audit, polish, simplify, harden, animate, or otherwise improve a frontend interface:... |
| `implement` | "Implement a piece of work based on a spec or set of tickets." |
| `implement-spec` | "Implement the result of /to-spec and /to-tickets in code." |
| `improve-codebase-architecture` | Scan a codebase for deepening opportunities, present them as a visual HTML report, then grill through whichever one you pick. |
| `in-your-own-words` | "Restate in your own words what you think the user's goals are and what problem they're trying to solve. Use for /in-your-own-words." |
| `incremental-implementation` | Delivers changes incrementally in thin, verifiable slices. Use when implementing any feature or change that touches more than one file, or when pic... |
| `interrogate` | "Use for \"interrogate\", \"adversarial review\", \"multi-model review\", \"challenge this\", \"stress test this code\", \"find blind spots\", or \... |
| `investigate-first` | Diagnose ambiguous failures before editing. Use for unknown causes, intermittent behavior, performance regressions, or investigations needing evide... |
| `ketchup` | "Catch the user up on what changed in this chat since their last message, in a few plain sentences and small visuals. Give each action item just en... |
| `kimi-delegate` | Delegate a coding task to the Kimi Code CLI (`kimi`) as a background implementer, then review its |
| `lean-build` | Build feature work with high overbuilding risk. Use for new behavior, product slices, or integrations where repository reuse, strict scope, and an ... |
| `loop-me` | Grill me about specs for the workflows I want to build, within this workspace. |
| `maintain-verification-skill` | "Periodic pass that keeps a project's verification skill and feature map honest: parallel source readers per feature, one live session driving ever... |
| `make-pr-easy-to-review` | Prepare PRs for review by cleaning noisy history, improving PR descriptions, and adding reviewer guidance without changing code behavior. Use for "... |
| `megacave` | Caveman in Classical Chinese: 文言文 register, far fewer characters, technical |
| `migrate-to-shoehorn` | Migrate test files from `as` type assertions to @total-typescript/shoehorn. Use when user mentions shoehorn, wants to replace `as` in tests, or nee... |
| `migration` | Implement reversible compatibility-safe transitions. Use for schema, data, API, protocol, configuration, or dependency migrations requiring rollbac... |
| `muse-delegate` | Delegate a coding task to Muse Code (`muse`) as a background implementer, then review its diff and |
| `no-comments` | Use before review when the user asks to strip, remove, or clean up comments in code. |
| `observability-and-instrumentation` | Instruments code so production behavior is visible and diagnosable. Use when adding logging, metrics, tracing, or alerting. Use when shipping any f... |
| `omp-delegate` | Delegate a coding task to Oh My Pi (`omp`) as a background implementer, then review its |
| `opencode-delegate` | Delegate a coding task to the OpenCode CLI as a background implementer, then review its diff and |
| `pdf-text-replace` | Replace text in fillable PDF forms by updating form field values. This skill should be used when users need to update names, addresses, dates, or o... |
| `performance-optimization` | Optimizes application performance across frontend, backend, queries, and databases. Use when performance requirements exist, when you suspect perfo... |
| `pi-delegate` | Delegate a coding task to the Pi coding agent CLI (`pi`) as a background implementer, then review |
| `planning-and-task-breakdown` | Breaks work into ordered tasks. Use when you have a spec or clear requirements and need to break work into implementable tasks. Use when a task fee... |
| `ponytail` | "Lazy senior dev mode for any coding task: the smallest change that fully solves it, and a reply a busy human understands in one read." |
| `ponytail-audit` | "Quality audit of the whole repo: bugs, security, real load, missing tests, speed, and what to delete. Most important first." |
| `ponytail-debt` | "Harvest every shortcut: comment into one debt ledger, so deferrals get tracked instead of forgotten. One-shot report." |
| `ponytail-gain` | "Show ponytail measured impact as a scoreboard: less code, less cost, more speed, from the agentic benchmark averages. One-shot display." |
| `ponytail-help` | "Quick reference for ponytail's modes, skills, and commands. One-shot display." |
| `ponytail-review` | "Quality review of a diff: bugs, security, real load, missing tests, speed, and what to delete. Each finding says what goes wrong and how to fix it." |
| `poteto-help` | Guides users through pstack setup, /poteto-mode, and picking the skill, playbook, or principle for a task. Type /poteto-help with a question. |
| `poteto-mode` | Apply poteto's rigorous engineering workflow to non-trivial coding, investigation, review, migration, and verification tasks. |
| `pr` | "Use when writing a PR body." |
| `principle-attack-the-premise` | "Apply when two or more fixes that share one premise have failed the same gate. Write the premise down and test it directly before you write anothe... |
| `principle-boundary-discipline` | "Apply when wiring validation, error handling, or framework adapters. Concentrate guards at system boundaries (CLI, config, network, external APIs)... |
| `principle-build-the-lever` | "Apply to any non-trivial work, not just bulk work: edits, migrations, analyses, checks. Build the tool that does it or proves it (codemod, script,... |
| `principle-encode-lessons-in-structure` | "Apply when you catch yourself writing the same instruction a second time, or notice a recurring correction. Encode the rule as a lint, metadata fl... |
| `principle-exhaust-the-design-space` | "Apply when facing a novel UI interaction or architectural decision with no precedent in the codebase. Build 2-3 competing prototypes and compare s... |
| `principle-experience-first` | "Apply when product, UX, or feature-scope tradeoffs come up. Choose user delight over implementation convenience; ship fewer polished features over... |
| `principle-explain-the-number` | "Apply before you trust, report, or act on a number you measured: a speedup, a regression, a throughput, a latency, or an eval result. Find what li... |
| `principle-fix-root-causes` | "Apply when debugging. Trace each symptom to its root cause and fix it there; reproduce first, ask why until you reach it, resist nil-check guards ... |
| `principle-foundational-thinking` | "Apply before writing logic: choosing core types and data structures, sequencing scaffold-vs-feature work, asking what concurrent actors share. Get... |
| `principle-guard-the-context-window` | "Apply when context is filling up: large outputs, long files, repeated reads, fan-out planning. Route bulk to subagents; keep summaries in the main... |
| `principle-laziness-protocol` | "Apply when refactoring, evaluating diff size, or tempted to add abstractions, layers, or signal threading. Bias toward deletion and the smallest c... |
| `principle-make-operations-idempotent` | "Apply when designing commands, lifecycle steps, or processing loops that run amid crashes, restarts, and retries. Converge to the same end state r... |
| `principle-migrate-callers-then-delete-legacy-apis` | "Apply when introducing a new internal API while old callers still exist. Migrate callers and delete the old API in the same wave instead of preser... |
| `principle-minimize-reader-load` | "Apply when reviewing or shaping code that's hard to trace. Count layers between question and answer, and hidden state in the reader's head; collap... |
| `principle-model-the-domain` | "Apply when writing stateful logic, or when code branches a lot or repeats a shape assumption across files. Encode the domain in a structure instea... |
| `principle-never-block-on-the-human` | "Apply when tempted to ask 'should I do X?' on reversible work. Proceed, present the result, let the human course-correct after the fact; reserve c... |
| `principle-outcome-oriented-execution` | "Apply during planned rewrites and migrations with explicit phase boundaries. Converge on the target architecture; don't preserve smooth intermedia... |
| `principle-prove-it-works` | "Apply after completing a task, before declaring done. Verify against the real artifact (run the feature, read the actual value, inspect the diff),... |
| `principle-redesign-from-first-principles` | "Apply when integrating a new requirement into an existing design. Redesign as if the requirement had been a foundational assumption from day one, ... |
| `principle-separate-before-serializing-shared-state` | "Apply when concurrent actors might write to the same file, branch, key, or state object. Eliminate the sharing first; serialize structurally only ... |
| `principle-sequence-verifiable-units` | "Apply to multi-step work (sweeps, migrations, runs of similar edits) and to how you stack commits and PRs. Break work into small units that each e... |
| `principle-subtract-before-you-add` | "Apply when sequencing an addition, refactor, or rewrite. Remove dead weight, redundant validators, and stub references first, then build on the si... |
| `principle-test-behavior-not-implementation` | "Apply when you write, change, or keep a test. Assert what the code's users can observe, so that the test fails when that behavior breaks and keeps... |
| `principle-type-system-discipline` | "Apply when designing types, reviewing a function signature, or writing code in any statically-typed language. Make illegal states unrepresentable,... |
| `prototype` | Build a throwaway prototype to answer a design question. Use when the user wants to sanity-check whether a state model or logic feels right, or exp... |
| `qoder-delegate` | Delegate a coding task to the Qoder CLI (`qodercli`) as a background implementer, then review its |
| `recall` | "Reconstruct your recent working context from your own chat history, live state, and the shared record (user reports, prior fixes, incidents), then... |
| `receiving-code-review` | Use when receiving code review feedback, before implementing suggestions, especially if feedback seems unclear or technically questionable - requir... |
| `reflect` | Spawn three parallel review subagents over the active transcript, surface learnings, and route each to a concrete edit on an existing skill. Use wh... |
| `requesting-code-review` | Use when completing tasks, implementing major features, or before merging to verify work meets requirements |
| `research` | Investigate a question against high-trust primary sources and capture the findings as a Markdown file in the repo. Use when the user wants a topic ... |
| `retro` | "Conduct a retrospective on a coding session." |
| `safe-refactor` | Restructure code while preserving behavior. Use for extraction, consolidation, ownership moves, or cleanup where verification must bracket structur... |
| `scaffold-exercises` | Create exercise directory structures with sections, problems, solutions, and explainers that pass linting. Use when user wants to scaffold exercise... |
| `security-and-hardening` | Hardens code against vulnerabilities. Use when auditing an input handler for vulnerabilities, when handling user input, authentication, data storag... |
| `setup-matt-pocock-skills` | "Configure this repo for the engineering skills: set up its issue tracker, triage label vocabulary, and domain doc layout. Run once before first us... |
| `setup-pre-commit` | Set up Husky pre-commit hooks with lint-staged (Prettier), type checking, and tests in the current repo. Use when user wants to add pre-commit hook... |
| `setup-pstack` | Configure which models pstack uses per role. Detects available models and writes the current runtime's override sheet. Use for /setup-pstack, "conf... |
| `setup-ts-deep-modules` | Wire dependency-cruiser into a TypeScript repo so each package is a deep module, with implementation hidden in subfolders and reachable only throug... |
| `sharpen` | "Sharpen a task before starting: the expert approach, what the user is really after, and the right level of specification. Use for /sharpen." |
| `shipping-and-launch` | Prepares production launches. Use when preparing to deploy to production, or when asking what needs to be in place before shipping. Use when you ne... |
| `show-me-your-work` | "Keep a reviewable decision trail for long-running or unattended work: a TSV log with one row per decision (what, why, evidence, result). Local by ... |
| `simplify-codebase` | Simplification audit or authorized codebase simplification whose stated objective is to remove accidental complexity. Use for evidence-backed delet... |
| `source-driven-development` | Grounds every implementation decision in official documentation. Use when you want to verify an approach against the official docs before implement... |
| `spec-driven-development` | Creates specs before coding. Use when starting a new project, feature, or significant change and no specification exists yet. Use when drafting a P... |
| `subagent-driven-development` | Use when executing implementation plans with independent tasks in the current session |
| `surgical-patch` | Fix bugs and small behavior changes at the narrowest responsible layer. Use when regression proof, preserved surrounding behavior, and task-relevan... |
| `swarm` | "Fan out N independent workers, collect their results, and return one report for coverage, races, gauntlets, or exploration." |
| `systematic-debugging` | Use when encountering any bug, test failure, or unexpected behavior, before proposing fixes |
| `tdd` | "Use only when the user explicitly asks for TDD, a failing test, or a regression test, OR when the bug has an obvious cheap local test target. Skip... |
| `teach` | "Explain a body of work plainly so a person actually understands it. Runs the `how` and `why` skills and weaves what they find into one clear expla... |
| `technical-writing` | "Layered technical-writing standard: Diátaxis structure, Google developer style sentences, STE instruction rules, Global English syntax. Use for /t... |
| `test-driven-development` | Use when implementing any feature or bugfix, before writing implementation code |
| `test-value` | Improve test value and feedback cost when auditing slow, flaky, redundant or brittle tests; choosing tests during implementation; or reviewing test... |
| `thermo-nuclear-code-quality-review` | Run an extremely strict maintainability review for abstraction quality, giant files, and spaghetti-condition growth. Use for a thermo-nuclear code ... |
| `thermo-nuclear-review` | Comprehensive security and correctness audit of a branch's changes. Use for thermo nuclear, thermonuclear, or deep review requests, or branch/PR di... |
| `thermos` | "Launch both thermo-nuclear review subagents in parallel, then synthesize their findings. Use for thermos, double thermo review, or combined bug/se... |
| `to-questionnaire` | Turn a decision you can't fully answer into a questionnaire for someone else to fill in. |
| `to-spec` | "Turn the current conversation into a spec and publish it to the project issue tracker: no interview, just synthesis of what you've already discuss... |
| `to-tickets` | Break a plan, spec, or the current conversation into a set of tracer-bullet tickets, each declaring its blocking edges, published to the configured... |
| `triage` | Move issues and external PRs through a state machine of triage roles, categorise, verify, grill if needed, and write agent-ready briefs. |
| `typescript-best-practices` | TypeScript best practices. Use when reading or editing any .ts or .tsx file. |
| `ultracave` | Caveman at maximum compression: fragments, one word when one word is enough, |
| `understand` | Analyze a codebase to produce an interactive knowledge graph for understanding architecture, components, and relationships |
| `understand-chat` | Use when you need to ask questions about a codebase or understand code using a knowledge graph |
| `understand-dashboard` | Launch the interactive web dashboard to visualize a codebase's knowledge graph |
| `understand-diff` | Use when you need to analyze git diffs or pull requests to understand what changed, affected components, and risks |
| `understand-domain` | Extract business domain knowledge from a codebase and generate an interactive domain flow graph. Works standalone (lightweight scan) or derives fro... |
| `understand-explain` | Use when you need a deep-dive explanation of a specific file, function, or module in the codebase |
| `understand-figma` | Analyze a Figma file via the Figma REST API and generate an interactive design knowledge graph (pages, screens, components, component sets, instanc... |
| `understand-knowledge` | Analyze a Karpathy-pattern LLM wiki knowledge base and generate an interactive knowledge graph with entity extraction, implicit relationships, and ... |
| `understand-onboard` | Use when you need to generate an onboarding guide for new team members joining a project |
| `unslop` | Cut AI tells from any writing. Must always apply. |
| `using-agent-skills` | Discovers and invokes agent skills. Use when starting a session, or when you need to decide which skill or workflow applies to the piece of work at... |
| `using-git-worktrees` | Use when starting feature work that needs isolation from current workspace or before executing implementation plans - ensures an isolated workspace... |
| `using-superpowers` | Use when starting any conversation - establishes how to find and use skills, requiring skill invocation before ANY response including clarifying qu... |
| `verification-before-completion` | Use when about to claim work is complete, fixed, or passing, before committing or creating PRs - requires running verification commands and confirm... |
| `verify-and-stop` | Prove existing work meets acceptance conditions without expanding scope. Use for validation-only tasks, completion checks, focused gate runs, and l... |
| `vibe-delegate` | Delegate a coding task to the Mistral Vibe CLI (`vibe`) as a background implementer, then review its |
| `wait-what` | "Stop. That last message did not land: re-pitch it." |
| `warp-delegate` | Delegate a coding task to the Warp Agent CLI (`oz`) as a background implementer, then review its |
| `wayfinder` | Plan a huge chunk of work (more than one agent session can hold) as a shared map of decision tickets on your issue tracker, and resolve them one at... |
| `what-did-i-get-done` | Summarize authored commits over a user-specified time period into a concise update |
| `why` | "Use for 'why does X work this way', 'why we picked Y', design rationale, regressions, postmortems, or data-backed thresholds. Discovers available ... |
| `wizard` | Generate an interactive bash wizard that walks a human through steps only they can perform. Use when provisioning infrastructure, setting up creden... |
| `writing-beats` | Writing, exploit; assemble raw material into a journey of beats, grounding each term before a beat leans on it. |
| `writing-for-agents` | Writing documents for agents. Use when creating or editing skills, or modifying AGENTS.md or CLAUDE.md. |
| `writing-fragments` | "Writing, explore: mine raw fragments, no structure yet." |
| `writing-plans` | Use when you have a spec or requirements for a multi-step task, before touching code |
| `writing-shape` | "Writing, exploit: shape raw material into an article, paragraph by paragraph." |
| `writing-skills` | Use when creating new skills, editing existing skills, or verifying skills work before deployment |
| `zcode-delegate` | Delegate a coding task to the Z.AI ZCode CLI as a background implementer, then review its diff and |

### Design & UX (agent-skills/design) — 10 skills

| Skill | Description |
|---|---|
| `banner-design` | "Design banners for social media, ads, website heroes, creative assets, and print. Multiple art direction options with optional generated or suppli... |
| `brand` | Brand voice, visual identity, messaging frameworks, asset management, brand consistency. Activate for branded content, tone of voice, marketing ass... |
| `design` | "Comprehensive design skill: brand identity, design tokens, UI styling, logo generation (55 styles, Gemini, Atlas Cloud, or MuAPI AI), corporate id... |
| `design-system` | Token architecture, component specifications, and slide generation. Three-layer tokens (primitive→semantic→component), CSS variables, spacing/typog... |
| `graphify` | "Use for any question about a codebase, its architecture, file relationships, or project content — especially when graphify-out/ exists, where the ... |
| `idea-refine` | Refines raw ideas into sharp, actionable concepts through structured divergent and convergent thinking. Use when an idea is still vague, when you n... |
| `interview-me` | Extracts what the user actually wants instead of what they think they should want. Achieves this through one-question-at-a-time interview until ~95... |
| `slides` | Create strategic HTML presentations with Chart.js, design tokens, responsive layouts, copywriting formulas, and contextual slide strategies. |
| `ui-styling` | Create beautiful, accessible user interfaces with shadcn/ui components (built on Radix UI + Tailwind), Tailwind CSS utility-first styling, and canv... |
| `ui-ux-pro-max` | "UI/UX design intelligence for web, mobile, and desktop. This skill should be used when designing, building, reviewing, or fixing interfaces, inclu... |

### Official — Anthropic (agent-skills/official) — 13 skills

| Skill | Description |
|---|---|
| `algorithmic-art` | Creating algorithmic art using p5.js with seeded randomness and interactive parameter exploration. Use this when users request creating art using c... |
| `brand-guidelines` | Applies Anthropic's official brand colors and typography to any sort of artifact that may benefit from having Anthropic's look-and-feel. Use it whe... |
| `canvas-design` | Create beautiful visual art in .png and .pdf documents using design philosophy. You should use this skill when the user asks to create a poster, pi... |
| `claude-api` | Reference for the Claude API / Anthropic SDK — model ids, pricing, params, streaming, tool use, MCP, agents, caching, token counting, model migration. |
| `doc-coauthoring` | Guide users through a structured workflow for co-authoring documentation. Use when user wants to write documentation, proposals, technical specs, d... |
| `frontend-design` | Guidance for distinctive, intentional visual design when building new UI or reshaping an existing one. Helps with aesthetic direction, typography, ... |
| `internal-comms` | A set of resources to help me write all kinds of internal communications, using the formats that my company likes to use. Claude should use this sk... |
| `mcp-builder` | Guide for creating high-quality MCP (Model Context Protocol) servers that enable LLMs to interact with external services through well-designed tool... |
| `skill-creator` | Create new skills, modify and improve existing skills, and measure skill performance. Use when users want to create a skill from scratch, edit, or ... |
| `slack-gif-creator` | Knowledge and utilities for creating animated GIFs optimized for Slack. Provides constraints, validation tools, and animation concepts. Use when us... |
| `theme-factory` | Toolkit for styling artifacts with a theme. These artifacts can be slides, docs, reportings, HTML landing pages, etc. There are 10 pre-set themes w... |
| `web-artifacts-builder` | Suite of tools for creating elaborate, multi-component claude.ai HTML artifacts using modern frontend web technologies (React, Tailwind CSS, shadcn... |
| `webapp-testing` | Toolkit for interacting with and testing local web applications using Playwright. Supports verifying frontend functionality, debugging UI behavior,... |

### SaaS & Tool Integrations (agent-skills/integrations) — 864 skills

| Skill | Description |
|---|---|
| `-21risk-automation` | "Automate 21risk tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `-2chat-automation` | "Automate 2chat tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ably-automation` | "Automate Ably tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `abstract-automation` | "Automate Abstract tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `abuselpdb-automation` | "Automate Abuselpdb tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `abyssale-automation` | "Automate Abyssale tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `accelo-automation` | "Automate Accelo tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `accredible-certificates-automation` | "Automate Accredible Certificates tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `acculynx-automation` | "Automate Acculynx tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `active-campaign-automation` | "Automate ActiveCampaign tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `addresszen-automation` | "Automate Addresszen tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `adobe-automation` | "Automate Adobe tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `adrapid-automation` | "Automate Adrapid tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `adyntel-automation` | "Automate Adyntel tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `aero-workflow-automation` | "Automate Aero Workflow tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `aeroleads-automation` | "Automate Aeroleads tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `affinda-automation` | "Automate Affinda tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `affinity-automation` | "Automate Affinity tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `agencyzoom-automation` | "Automate Agencyzoom tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `agent-mail-automation` | "Automate Agent Mail tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `agentql-automation` | "Automate Agentql tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `agenty-automation` | "Automate Agenty tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `agiled-automation` | "Automate Agiled tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `agility-cms-automation` | "Automate Agility CMS tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ahrefs-automation` | "Automate SEO research with Ahrefs -- analyze backlink profiles, research keywords, track domain metrics history, audit organic rankings, and perfo... |
| `ai-ml-api-automation` | "Automate AI ML API tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `aivoov-automation` | "Automate Aivoov tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `alchemy-automation` | "Automate Alchemy tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `algodocs-automation` | "Automate Algodocs tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `algolia-automation` | "Automate Algolia tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `all-images-ai-automation` | "Automate All Images AI tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `alpha-vantage-automation` | "Automate Alpha Vantage tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `altoviz-automation` | "Automate Altoviz tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `alttext-ai-automation` | "Automate Alttext AI tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `amara-automation` | "Automate Amara tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `amazon-automation` | "Automate Amazon tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ambee-automation` | "Automate Ambee tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ambient-weather-automation` | "Automate Ambient Weather tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `amcards-automation` | "Automate Amcards tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `anchor-browser-automation` | "Automate Anchor Browser tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `anonyflow-automation` | "Automate Anonyflow tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `anthropic-administrator-automation` | "Automate Anthropic Admin tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `anthropic_administrator-automation` | "Automate Anthropic Admin tasks via Rube MCP (Composio): API keys, usage, workspaces, and organization management. Always search tools first for cu... |
| `apaleo-automation` | "Automate Apaleo tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `apex27-automation` | "Automate Apex27 tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `api-bible-automation` | "Automate API Bible tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `api-labz-automation` | "Automate API Labz tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `api-ninjas-automation` | "Automate API Ninjas tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `api-sports-automation` | "Automate API Sports tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `api2pdf-automation` | "Automate Api2pdf tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `apiflash-automation` | "Automate Apiflash tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `apify-automation` | "Automate web scraping and data extraction with Apify -- run Actors, manage datasets, create reusable tasks, and retrieve crawl results through the... |
| `apilio-automation` | "Automate Apilio tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `apipie-ai-automation` | "Automate Apipie AI tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `apitemplate-io-automation` | "Automate Apitemplate IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `apiverve-automation` | "Automate Apiverve tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `apollo-automation` | "Automate Apollo.io lead generation -- search organizations, discover contacts, enrich prospect data, manage contact stages, and build targeted out... |
| `appcircle-automation` | "Automate Appcircle tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `appdrag-automation` | "Automate Appdrag tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `appointo-automation` | "Automate Appointo tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `appsflyer-automation` | "Automate Appsflyer tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `appveyor-automation` | "Automate Appveyor tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `artifacts-builder` | Suite of tools for creating elaborate, multi-component claude.ai HTML artifacts using modern frontend web technologies (React, Tailwind CSS, shadcn... |
| `aryn-automation` | "Automate Aryn tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ascora-automation` | "Automate Ascora tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ashby-automation` | "Automate recruiting and hiring workflows in Ashby -- manage candidates, jobs, applications, interviews, and notes through natural language commands." |
| `asin-data-api-automation` | "Automate Asin Data API tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `astica-ai-automation` | "Automate Astica AI tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `async-interview-automation` | "Automate Async Interview tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `atlassian-automation` | "Automate Atlassian tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `attio-automation` | "Automate Attio CRM operations -- search records, query contacts and companies with advanced filters, manage notes, list attributes, and navigate y... |
| `auth0-automation` | "Automate Auth0 tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `autobound-automation` | "Automate Autobound tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `autom-automation` | "Automate Autom tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `axonaut-automation` | "Automate Axonaut tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ayrshare-automation` | "Automate Ayrshare tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `backendless-automation` | "Automate Backendless tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bannerbear-automation` | "Automate Bannerbear tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bart-automation` | "Automate Bart tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `baselinker-automation` | "Automate Baselinker tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `baserow-automation` | "Automate Baserow tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `basin-automation` | "Automate Basin tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `battlenet-automation` | "Automate Battlenet tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `beaconchain-automation` | "Automate Beaconchain tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `beaconstac-automation` | "Automate Beaconstac tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `beamer-automation` | "Automate Beamer tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `beeminder-automation` | "Automate Beeminder tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bench-automation` | "Automate Bench tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `benchmark-email-automation` | "Automate Benchmark Email tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `benzinga-automation` | "Automate Benzinga tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bestbuy-automation` | "Automate Bestbuy tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `better-proposals-automation` | "Automate Better Proposals tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `better-stack-automation` | "Automate Better Stack tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bidsketch-automation` | "Automate Bidsketch tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `big-data-cloud-automation` | "Automate Big Data Cloud tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bigmailer-automation` | "Automate Bigmailer tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bigml-automation` | "Automate Bigml tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bigpicture-io-automation` | "Automate Bigpicture IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bitquery-automation` | "Automate Bitquery tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bitwarden-automation` | "Automate Bitwarden tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `blackbaud-automation` | "Automate Blackbaud tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `blackboard-automation` | "Automate Blackboard tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `blocknative-automation` | "Automate Blocknative tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `boldsign-automation` | "Automate Boldsign tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bolna-automation` | "Automate Bolna tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `boloforms-automation` | "Automate Boloforms tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bolt-iot-automation` | "Automate Bolt Iot tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bonsai-automation` | "Automate Bonsai tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bookingmood-automation` | "Automate Bookingmood tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `booqable-automation` | "Automate Booqable tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `borneo-automation` | "Automate Borneo tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `botbaba-automation` | "Automate Botbaba tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `botpress-automation` | "Automate Botpress tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `botsonic-automation` | "Automate Botsonic tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `botstar-automation` | "Automate Botstar tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bouncer-automation` | "Automate Bouncer tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `boxhero-automation` | "Automate Boxhero tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `braintree-automation` | "Braintree Automation: manage payment processing via Stripe-compatible tools for customers, subscriptions, payment methods, and transactions" |
| `brand-guidelines` | Applies Anthropic's official brand colors and typography to any sort of artifact that may benefit from having Anthropic's look-and-feel. Use it whe... |
| `brandfetch-automation` | "Automate Brandfetch tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `breeze-automation` | "Automate Breeze tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `breezy-hr-automation` | "Automate Breezy HR tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `brex-automation` | "Automate Brex tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `brex-staging-automation` | "Automate Brex Staging tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `brightdata-automation` | "Automate Brightdata tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `brightpearl-automation` | "Automate Brightpearl tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `brilliant-directories-automation` | "Automate Brilliant Directories tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `browseai-automation` | "Automate Browseai tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `browser-tool-automation` | "Automate Browser Tool tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `browserbase-tool-automation` | "Automate Browserbase Tool tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `browserhub-automation` | "Automate Browserhub tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `browserless-automation` | "Automate Browserless tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `btcpay-server-automation` | "Automate Btcpay Server tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bubble-automation` | "Automate Bubble tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bugbug-automation` | "Automate Bugbug tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bugherd-automation` | "Automate Bugherd tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bugsnag-automation` | "Automate Bugsnag tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `buildkite-automation` | "Automate Buildkite tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `builtwith-automation` | "Automate Builtwith tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `bunnycdn-automation` | "Automate Bunnycdn tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `byteforms-automation` | "Automate Byteforms tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `cabinpanda-automation` | "Automate Cabinpanda tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `cal-automation` | "Automate Cal tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `calendarhero-automation` | "Automate Calendarhero tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `callerapi-automation` | "Automate Callerapi tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `callingly-automation` | "Automate Callingly tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `callpage-automation` | "Automate Callpage tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `campaign-cleaner-automation` | "Automate Campaign Cleaner tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `campayn-automation` | "Automate Campayn tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `canny-automation` | "Automate Canny tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `canvas-automation` | "Automate Canvas tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `canvas-design` | Create beautiful visual art in .png and .pdf documents using design philosophy. You should use this skill when the user asks to create a poster, pi... |
| `capsule-crm-automation` | "Automate Capsule CRM operations -- manage contacts (parties), run structured filter queries, track tasks and projects, log entries, and handle org... |
| `capsule_crm-automation` | "Automate Capsule CRM tasks via Rube MCP (Composio): contacts, opportunities, cases, tasks, and pipeline management. Always search tools first for ... |
| `carbone-automation` | "Automate Carbone tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `cardly-automation` | "Automate Cardly tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `castingwords-automation` | "Automate Castingwords tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `cats-automation` | "Automate Cats tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `cdr-platform-automation` | "Automate Cdr Platform tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `census-bureau-automation` | "Automate Census Bureau tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `centralstationcrm-automation` | "Automate Centralstationcrm tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `certifier-automation` | "Automate Certifier tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `changelog-generator` | Automatically creates user-facing changelogs from git commits by analyzing commit history, categorizing changes, and transforming technical commits... |
| `chaser-automation` | "Automate Chaser tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `chatbotkit-automation` | "Automate Chatbotkit tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `chatfai-automation` | "Automate Chatfai tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `chatwork-automation` | "Automate Chatwork tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `chmeetings-automation` | "Automate Chmeetings tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `cincopa-automation` | "Automate Cincopa tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `claid-ai-automation` | "Automate Claid AI tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `classmarker-automation` | "Automate Classmarker tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `clearout-automation` | "Automate Clearout tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `clickmeeting-automation` | "Automate Clickmeeting tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `clockify-automation` | "Automate time tracking workflows in Clockify -- create and manage time entries, workspaces, and users through natural language commands." |
| `cloudcart-automation` | "Automate Cloudcart tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `cloudconvert-automation` | "Automate Cloudconvert tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `cloudflare-api-key-automation` | "Automate Cloudflare API tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `cloudflare-automation` | "Automate Cloudflare tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `cloudflare-browser-rendering-automation` | "Automate Cloudflare Browser Rendering tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `cloudinary-automation` | "Automate Cloudinary media management including folder organization, upload presets, asset lookup, transformations, and usage monitoring through na... |
| `cloudlayer-automation` | "Automate Cloudlayer tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `cloudpress-automation` | "Automate Cloudpress tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `coassemble-automation` | "Automate Coassemble tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `codacy-automation` | "Automate Codacy tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `codeinterpreter-automation` | "Automate Codeinterpreter tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `codereadr-automation` | "Automate Codereadr tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `coinbase-automation` | "Coinbase Automation: list and manage cryptocurrency wallets, accounts, and portfolio data via Coinbase CDP SDK" |
| `coinmarketcal-automation` | "Automate Coinmarketcal tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `coinmarketcap-automation` | "Automate Coinmarketcap tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `coinranking-automation` | "Automate Coinranking tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `college-football-data-automation` | "Automate College Football Data tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `competitive-ads-extractor` | Extracts and analyzes competitors' ads from ad libraries (Facebook, LinkedIn, etc.) to understand what messaging, problems, and creative approaches... |
| `composio-automation` | "Automate Composio tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `composio-search-automation` | "Automate Composio Search tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `connect` | Connect Claude to any app. Send emails, create issues, post messages, update databases - take real actions across Gmail, Slack, GitHub, Notion, and... |
| `connect-apps` | Connect Claude to external apps like Gmail, Slack, GitHub. Use this skill when the user wants to send emails, create issues, post messages, or take... |
| `connecteam-automation` | "Automate Connecteam tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `content-research-writer` | Assists in writing high-quality content by conducting research, adding citations, improving hooks, iterating on outlines, and providing real-time f... |
| `contentful-automation` | "Automate headless CMS operations in Contentful -- list spaces, retrieve space metadata, and update space configurations through the Composio Conte... |
| `contentful-graphql-automation` | "Automate Contentful Graphql tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `control-d-automation` | "Automate Control D tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `conversion-tools-automation` | "Automate Conversion Tools tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `convertapi-automation` | "Automate Convertapi tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `conveyor-automation` | "Automate Conveyor tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `convolo-ai-automation` | "Automate Convolo AI tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `corrently-automation` | "Automate Corrently tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `countdown-api-automation` | "Automate Countdown API tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `coupa-automation` | "Automate Coupa tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `craftmypdf-automation` | "Automate Craftmypdf tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `crowdin-automation` | "Automate Crowdin tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `crustdata-automation` | "Automate Crustdata tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `cults-automation` | "Automate Cults tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `curated-automation` | "Automate Curated tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `currents-api-automation` | "Automate Currents API tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `customerio-automation` | "Automate customer engagement workflows including broadcast triggers, message analytics, segment management, and newsletter tracking through Custom... |
| `customgpt-automation` | "Automate Customgpt tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `customjs-automation` | "Automate Customjs tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `cutt-ly-automation` | "Automate Cutt Ly tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `d2lbrightspace-automation` | "Automate D2lbrightspace tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `dadata-ru-automation` | "Automate Dadata Ru tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `daffy-automation` | "Automate Daffy tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `dailybot-automation` | "Automate Dailybot tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `datagma-automation` | "Automate Datagma tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `datarobot-automation` | "Automate Datarobot tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `deadline-funnel-automation` | "Automate Deadline Funnel tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `deel-automation` | "Automate Deel tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `deepgram-automation` | "Automate Deepgram tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `demio-automation` | "Automate Demio tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `desktime-automation` | "Automate Desktime tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `detrack-automation` | "Automate Detrack tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `developer-growth-analysis` | Analyzes your recent Claude Code chat history to identify coding patterns, development gaps, and areas for improvement, curates relevant learning r... |
| `dialmycalls-automation` | "Automate Dialmycalls tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `dialpad-automation` | "Automate Dialpad tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `dictionary-api-automation` | "Automate Dictionary API tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `diffbot-automation` | "Automate Diffbot tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `digicert-automation` | "Automate Digicert tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `digital-ocean-automation` | "Automate DigitalOcean tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `discordbot-automation` | "Automate Discordbot tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `dnsfilter-automation` | "Automate Dnsfilter tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `dock-certs-automation` | "Automate Dock Certs tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `docker-hub-automation` | "Automate Docker Hub operations -- manage organizations, repositories, teams, members, and webhooks via the Composio MCP integration." |
| `docker_hub-automation` | "Automate Docker Hub tasks via Rube MCP (Composio): repositories, images, tags, and container registry management. Always search tools first for cu... |
| `docmosis-automation` | "Automate Docmosis tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `docnify-automation` | "Automate Docnify tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `docsbot-ai-automation` | "Automate Docsbot AI tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `docsumo-automation` | "Automate Docsumo tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `docugenerate-automation` | "Automate Docugenerate tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `documenso-automation` | "Automate Documenso tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `documint-automation` | "Automate Documint tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `docupilot-automation` | "Automate Docupilot tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `docupost-automation` | "Automate Docupost tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `docuseal-automation` | "Automate Docuseal tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `docx` | "Comprehensive document creation, editing, and analysis with support for tracked changes, comments, formatting preservation, and text extraction. W... |
| `domain-name-brainstormer` | Generates creative domain name ideas for your project and checks availability across multiple TLDs (.com, .io, .dev, .ai, etc.). Saves hours of bra... |
| `doppler-marketing-automation-automation` | "Automate Doppler Marketing Automation tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `doppler-secretops-automation` | "Automate Doppler Secretops tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `dotsimple-automation` | "Automate Dotsimple tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `dovetail-automation` | "Automate Dovetail tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `dpd2-automation` | "Automate Dpd2 tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `draftable-automation` | "Automate Draftable tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `dreamstudio-automation` | "Automate Dreamstudio tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `drip-jobs-automation` | "Automate Drip Jobs tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `dripcel-automation` | "Automate Dripcel tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `dromo-automation` | "Automate Dromo tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `dropbox-sign-automation` | "Automate Dropbox Sign tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `dropcontact-automation` | "Automate Dropcontact tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `dungeon-fighter-online-automation` | "Automate Dungeon Fighter Online tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `dynamics365-automation` | "Dynamics 365 Automation: manage CRM contacts, accounts, leads, opportunities, sales orders, invoices, and cases via the Dynamics CRM Web API" |
| `echtpost-automation` | "Automate Echtpost tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `elevenlabs-automation` | "Automate ElevenLabs text-to-speech workflows -- generate speech from text, browse and inspect voices, check subscription limits, list models, stre... |
| `elorus-automation` | "Automate Elorus tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `emailable-automation` | "Automate Emailable tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `emaillistverify-automation` | "Automate Emaillistverify tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `emailoctopus-automation` | "Automate Emailoctopus tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `emelia-automation` | "Automate Emelia tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `encodian-automation` | "Automate Encodian tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `endorsal-automation` | "Automate Endorsal tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `enginemailer-automation` | "Automate Enginemailer tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `enigma-automation` | "Automate Enigma tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `entelligence-automation` | "Automate Entelligence tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `eodhd-apis-automation` | "Automate Eodhd Apis tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `epic-games-automation` | "Automate Epic Games tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `esignatures-io-automation` | "Automate Esignatures IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `espocrm-automation` | "Automate Espocrm tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `esputnik-automation` | "Automate Esputnik tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `etermin-automation` | "Automate Etermin tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `evenium-automation` | "Automate Evenium tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `eventbrite-automation` | "Automate Eventbrite event management, attendee tracking, organization discovery, and category browsing through natural language commands" |
| `eventee-automation` | "Automate Eventee tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `eventzilla-automation` | "Automate Eventzilla tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `everhour-automation` | "Automate Everhour tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `eversign-automation` | "Automate Eversign tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `exa-automation` | "Automate Exa tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `excel-automation` | "Excel Automation: create workbooks, manage worksheets, read/write cell data, and format spreadsheets via Microsoft Excel and Google Sheets integra... |
| `exist-automation` | "Automate Exist tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `expofp-automation` | "Automate Expofp tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `extracta-ai-automation` | "Automate Extracta AI tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `facebook-automation` | "Automate Facebook Page management including post creation, scheduling, video uploads, Messenger conversations, and audience engagement via Composio" |
| `faceup-automation` | "Automate Faceup tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `factorial-automation` | "Automate Factorial tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `feathery-automation` | "Automate Feathery tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `felt-automation` | "Automate Felt tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `fibery-automation` | "Automate Fibery tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `fidel-api-automation` | "Automate Fidel API tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `file-organizer` | Intelligently organizes your files and folders across your computer by understanding context, finding duplicates, suggesting better structures, and... |
| `files-com-automation` | "Automate Files Com tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `fillout-forms-automation` | "Automate Fillout tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `fillout_forms-automation` | "Automate Fillout tasks via Rube MCP (Composio): forms, submissions, workflows, and form builder. Always search tools first for current schemas." |
| `finage-automation` | "Automate Finage tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `findymail-automation` | "Automate Findymail tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `finerworks-automation` | "Automate Finerworks tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `fingertip-automation` | "Automate Fingertip tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `finmei-automation` | "Automate Finmei tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `fireberry-automation` | "Automate Fireberry tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `firecrawl-automation` | "Automate web crawling and data extraction with Firecrawl -- scrape pages, crawl sites, extract structured data, batch scrape URLs, and map website... |
| `fireflies-automation` | "Automate Fireflies tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `firmao-automation` | "Automate Firmao tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `fitbit-automation` | "Automate Fitbit tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `fixer-automation` | "Automate Fixer tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `fixer-io-automation` | "Automate Fixer IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `flexisign-automation` | "Automate Flexisign tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `flowiseai-automation` | "Automate Flowiseai tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `flutterwave-automation` | "Automate Flutterwave tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `fluxguard-automation` | "Automate Fluxguard tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `folk-automation` | "Automate Folk tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `fomo-automation` | "Automate Fomo tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `forcemanager-automation` | "Automate Forcemanager tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `formbricks-automation` | "Automate Formbricks tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `formcarry-automation` | "Automate Formcarry tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `formdesk-automation` | "Automate Formdesk tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `formsite-automation` | "Automate Formsite tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `foursquare-automation` | "Automate Foursquare tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `fraudlabs-pro-automation` | "Automate Fraudlabs Pro tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `freshbooks-automation` | "FreshBooks Automation: manage businesses, projects, time tracking, and billing in FreshBooks cloud accounting" |
| `front-automation` | "Automate Front tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `fullenrich-automation` | "Automate Fullenrich tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `gagelist-automation` | "Automate Gagelist tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `gamma-automation` | "Automate Gamma tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `gan-ai-automation` | "Automate Gan AI tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `gatherup-automation` | "Automate Gatherup tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `gemini-automation` | "Automate Gemini tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `gender-api-automation` | "Automate Gender API tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `genderapi-io-automation` | "Automate Genderapi IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `genderize-automation` | "Automate Genderize tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `geoapify-automation` | "Automate Geoapify tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `geocodio-automation` | "Automate Geocodio tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `geokeo-automation` | "Automate Geokeo tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `getform-automation` | "Automate Getform tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `gift-up-automation` | "Automate Gift Up tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `gigasheet-automation` | "Automate Gigasheet tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `giphy-automation` | "Automate Giphy tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `gist-automation` | "Automate Gist tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `givebutter-automation` | "Automate Givebutter tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `gladia-automation` | "Automate Gladia tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `gleap-automation` | "Automate Gleap tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `globalping-automation` | "Automate Globalping tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `go-to-webinar-automation` | "Automate GoToWebinar tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `godial-automation` | "Automate Godial tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `gong-automation` | "Automate Gong conversation intelligence -- retrieve call recordings, transcripts, detailed analytics, speaker stats, and workspace data -- using n... |
| `goodbits-automation` | "Automate Goodbits tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `goody-automation` | "Automate Goody tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `google-address-validation-automation` | "Automate Google Address Validation tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `google-admin-automation` | "Automate Google Workspace Admin tasks via Rube MCP (Composio): manage users, groups, memberships, suspend accounts, create users, add aliases. Alw... |
| `google-classroom-automation` | "Automate Google Classroom tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `google-cloud-vision-automation` | "Automate Google Cloud Vision tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `google-maps-automation` | "Automate Google Maps tasks via Rube MCP (Composio): geocode addresses, search places, get directions, compute route matrices, reverse geocode, aut... |
| `google-search-console-automation` | "Automate Google Search Console tasks via Rube MCP (Composio): query search analytics, list sites, inspect URLs, submit sitemaps, monitor search pe... |
| `googleads-automation` | "Automate Google Ads analytics tasks via Rube MCP (Composio): list Google Ads links, run GA4 reports, check compatibility, list properties and acco... |
| `googlebigquery-automation` | "Automate Google BigQuery tasks via Rube MCP (Composio): run SQL queries, explore datasets and metadata, execute MBQL queries via Metabase integrat... |
| `googlecalendar-automation` | "Automate Google Calendar tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `googledocs-automation` | "Automate Google Docs tasks via Rube MCP (Composio): create, edit, search, export, copy, and update documents. Always search tools first for curren... |
| `googledrive-automation` | "Automate Google Drive tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `googlemeet-automation` | "Automate Google Meet tasks via Rube MCP (Composio): create Meet spaces, schedule video conferences via Calendar events, manage meeting access. Alw... |
| `googlephotos-automation` | "Automate Google Photos tasks via Rube MCP (Composio): upload media, manage albums, search photos, batch add items, create and update albums. Alway... |
| `googleslides-automation` | "Automate Google Slides tasks via Rube MCP (Composio): create presentations, add slides from Markdown, batch update, copy from templates, get thumb... |
| `googlesuper-automation` | "Automate Google Super tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `googletasks-automation` | "Automate Google Tasks via Rube MCP (Composio): create, list, update, delete, move, and bulk-insert tasks and task lists. Always search tools first... |
| `google_admin-automation` | "Automate Google Admin tasks via Rube MCP (Composio): user management, org units, groups, and domain administration. Always search tools first for ... |
| `google_classroom-automation` | "Automate Google Classroom tasks via Rube MCP (Composio): course management, assignments, student rosters, and announcements. Always search tools f... |
| `google_maps-automation` | "Automate Google Maps tasks via Rube MCP (Composio): geocoding, directions, place search, and distance calculations. Always search tools first for ... |
| `google_search_console-automation` | "Automate Google Search Console tasks via Rube MCP (Composio): search performance, URL inspection, sitemaps, and indexing status. Always search too... |
| `gorgias-automation` | "Automate e-commerce customer support workflows in Gorgias -- manage tickets, customers, tags, and teams through natural language commands." |
| `gosquared-automation` | "Automate Gosquared tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `grafbase-automation` | "Automate Grafbase tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `graphhopper-automation` | "Automate Graphhopper tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `griptape-automation` | "Automate Griptape tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `grist-automation` | "Automate Grist tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `groqcloud-automation` | "Automate AI inference, chat completions, audio translation, and TTS voice management through GroqCloud's high-performance API via Composio" |
| `gumroad-automation` | "Automate Gumroad product management, sales tracking, license verification, and webhook subscriptions using natural language through the Composio M... |
| `habitica-automation` | "Automate Habitica tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `hackernews-automation` | "Automate Hackernews tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `happy-scribe-automation` | "Automate Happy Scribe tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `harvest-automation` | "Automate time tracking, project management, and invoicing workflows in Harvest -- log hours, manage projects, clients, and tasks through natural l... |
| `hashnode-automation` | "Automate Hashnode tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `helcim-automation` | "Automate Helcim tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `helloleads-automation` | "Automate Helloleads tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `helpwise-automation` | "Automate Helpwise tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `here-automation` | "Automate Here tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `heygen-automation` | "Automate AI video generation, avatar browsing, template-based video creation, and video status tracking through HeyGen's platform via Composio" |
| `heyreach-automation` | "Automate Heyreach tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `heyzine-automation` | "Automate Heyzine tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `highergov-automation` | "Automate Highergov tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `highlevel-automation` | "Automate Highlevel tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `honeybadger-automation` | "Automate Honeybadger tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `honeyhive-automation` | "Automate Honeyhive tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `hookdeck-automation` | "Automate Hookdeck tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `hotspotsystem-automation` | "Automate Hotspotsystem tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `html-to-image-automation` | "Automate Html To Image tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `humanitix-automation` | "Automate Humanitix tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `humanloop-automation` | "Automate Humanloop tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `hunter-automation` | "Automate Hunter.io email intelligence -- search domains for email addresses, find specific contacts, verify email deliverability, manage leads, an... |
| `hypeauditor-automation` | "Automate Hypeauditor tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `hyperbrowser-automation` | "Automate Hyperbrowser tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `hyperise-automation` | "Automate Hyperise tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `hystruct-automation` | "Automate Hystruct tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `icims-talent-cloud-automation` | "Automate Icims Talent Cloud tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `icypeas-automation` | "Automate Icypeas tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `idea-scale-automation` | "Automate Idea Scale tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `identitycheck-automation` | "Automate Identitycheck tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ignisign-automation` | "Automate Ignisign tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `image-enhancer` | Improves the quality of images, especially screenshots, by enhancing resolution, sharpness, and clarity. Perfect for preparing images for presentat... |
| `imagekit-io-automation` | "Automate Imagekit IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `imgbb-automation` | "Automate Imgbb tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `imgix-automation` | "Automate Imgix tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `influxdb-cloud-automation` | "Automate Influxdb Cloud tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `insighto-ai-automation` | "Automate Insighto AI tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `instacart-automation` | "Automate Instacart tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `instantly-automation` | "Automate Instantly cold email outreach -- manage campaigns, sending accounts, lead lists, bulk lead imports, and campaign analytics -- using natur... |
| `intelliprint-automation` | "Automate Intelliprint tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `internal-comms` | A set of resources to help me write all kinds of internal communications, using the formats that my company likes to use. Claude should use this sk... |
| `interzoid-automation` | "Automate Interzoid tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `invoice-organizer` | Automatically organizes invoices and receipts for tax preparation by reading messy files, extracting key information, renaming them consistently, a... |
| `ip2location-automation` | "Automate Ip2location tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ip2location-io-automation` | "Automate Ip2location IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ip2proxy-automation` | "Automate Ip2proxy tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ip2whois-automation` | "Automate Ip2whois tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ipdata-co-automation` | "Automate Ipdata co tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ipinfo-io-automation` | "Automate Ipinfo IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `iqair-airvisual-automation` | "Automate Iqair Airvisual tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `jigsawstack-automation` | "Automate Jigsawstack tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `jobnimbus-automation` | "Automate Jobnimbus tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `jotform-automation` | "Automate Jotform form listing, user management, activity history, folder organization, and plan inspection through natural language commands" |
| `jumpcloud-automation` | "Automate Jumpcloud tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `junglescout-automation` | "Automate Junglescout tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `kadoa-automation` | "Automate Kadoa tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `kaggle-automation` | "Automate Kaggle tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `kaleido-automation` | "Automate Kaleido tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `keap-automation` | "Automate Keap tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `keen-io-automation` | "Automate Keen IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `kickbox-automation` | "Automate Kickbox tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `kit-automation` | "Automate Kit tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `klipfolio-automation` | "Automate Klipfolio tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ko-fi-automation` | "Automate Ko Fi tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `kommo-automation` | "Automate Kommo CRM operations -- manage leads, pipelines, pipeline stages, tasks, and custom fields -- using natural language through the Composio... |
| `kontent-ai-automation` | "Automate Kontent AI tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `kraken-io-automation` | "Automate Kraken IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `l2s-automation` | "Automate L2s tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `labs64-netlicensing-automation` | "Automate Labs64 Netlicensing tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `landbot-automation` | "Automate Landbot tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `langbase-automation` | "Automate Langbase tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `langsmith-fetch` | Debug LangChain and LangGraph agents by fetching execution traces from LangSmith Studio. Use when debugging agent behavior, investigating errors, a... |
| `lastpass-automation` | "Automate Lastpass tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `launch-darkly-automation` | "Automate LaunchDarkly feature flag management -- list projects and environments, create and delete trigger workflows, and track code references vi... |
| `launch_darkly-automation` | "Automate LaunchDarkly tasks via Rube MCP (Composio): feature flags, environments, segments, and rollout management. Always search tools first for ... |
| `lead-research-assistant` | Identifies high-quality leads for your product or service by analyzing your business, searching for target companies, and providing actionable cont... |
| `leadfeeder-automation` | "Automate Leadfeeder tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `leadoku-automation` | "Automate Leadoku tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `leiga-automation` | "Automate Leiga tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `lemlist-automation` | "Automate Lemlist multichannel outreach -- manage campaigns, enroll leads, add personalization variables, export campaign data, and handle unsubscr... |
| `lemon-squeezy-automation` | "Automate Lemon Squeezy store management -- products, orders, subscriptions, customers, discounts, and checkout tracking -- using natural language ... |
| `lemon_squeezy-automation` | "Automate Lemon Squeezy tasks via Rube MCP (Composio): products, orders, subscriptions, checkouts, and digital sales. Always search tools first for... |
| `lessonspace-automation` | "Automate Lessonspace tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `lever-automation` | "Automate recruiting workflows in Lever ATS -- manage opportunities, job postings, requisitions, pipeline stages, and candidate tags through the Co... |
| `lever-sandbox-automation` | "Automate Lever Sandbox tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `leverly-automation` | "Automate Leverly tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `lexoffice-automation` | "Automate Lexoffice tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `linguapop-automation` | "Automate Linguapop tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `linkhut-automation` | "Automate Linkhut tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `linkup-automation` | "Automate Linkup tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `listclean-automation` | "Automate Listclean tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `listennotes-automation` | "Automate Listennotes tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `livesession-automation` | "Automate Livesession tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `lmnt-automation` | "Automate Lmnt tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `lodgify-automation` | "Automate Lodgify tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `logo-dev-automation` | "Automate Logo Dev tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `loomio-automation` | "Automate Loomio tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `loyverse-automation` | "Automate Loyverse tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `magnetic-automation` | "Automate Magnetic tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mailbluster-automation` | "Automate Mailbluster tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mailboxlayer-automation` | "Automate Mailboxlayer tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mailcheck-automation` | "Automate Mailcheck tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mailcoach-automation` | "Automate Mailcoach tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mailerlite-automation` | "Automate email marketing workflows including subscriber management, campaign analytics, group segmentation, and account monitoring through MailerL... |
| `mailersend-automation` | "Automate Mailersend tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mails-so-automation` | "Automate Mails So tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mailsoftly-automation` | "Automate Mailsoftly tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `maintainx-automation` | "Automate Maintainx tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `many-chat-automation` | "Automate ManyChat tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `many_chat-automation` | "Automate ManyChat tasks via Rube MCP (Composio): chatbot flows, subscribers, broadcasts, and messenger automation. Always search tools first for c... |
| `mapbox-automation` | "Automate Mapbox tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mapulus-automation` | "Automate Mapulus tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mboum-automation` | "Automate Mboum tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mcp-builder` | Guide for creating high-quality MCP (Model Context Protocol) servers that enable LLMs to interact with external services through well-designed tool... |
| `meeting-insights-analyzer` | Analyzes meeting transcripts and recordings to uncover behavioral patterns, communication insights, and actionable feedback. Identifies when you av... |
| `melo-automation` | "Automate Melo tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mem-automation` | "Automate Mem tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mem0-automation` | "Automate Mem0 tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `memberspot-automation` | "Automate Memberspot tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `memberstack-automation` | "Automate Memberstack tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `membervault-automation` | "Automate Membervault tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `metaads-automation` | "Automate Metaads tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `metaphor-automation` | "Automate Metaphor tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mezmo-automation` | "Automate Mezmo tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `microsoft-clarity-automation` | "Automate user behavior analytics with Microsoft Clarity -- export heatmap data, session metrics, and engagement analytics segmented by browser, de... |
| `microsoft-tenant-automation` | "Automate Microsoft Tenant tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `microsoft_clarity-automation` | "Automate Microsoft Clarity tasks via Rube MCP (Composio): session recordings, heatmaps, and user behavior analytics. Always search tools first for... |
| `minerstat-automation` | "Automate Minerstat tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `missive-automation` | "Automate Missive tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mistral-ai-automation` | "Automate Mistral AI operations -- manage files and libraries, upload documents for fine-tuning, batch processing, and OCR, track fine-tuning jobs,... |
| `mistral_ai-automation` | "Automate Mistral AI tasks via Rube MCP (Composio): completions, embeddings, fine-tuning, and model management. Always search tools first for curre... |
| `mocean-automation` | "Automate Mocean tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `moco-automation` | "Automate Moco tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `modelry-automation` | "Automate Modelry tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `moneybird-automation` | "Automate Moneybird tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `moonclerk-automation` | "Automate Moonclerk tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `moosend-automation` | "Automate Moosend tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mopinion-automation` | "Automate Mopinion tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `more-trees-automation` | "Automate More Trees tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `moxie-automation` | "Automate Moxie tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `moz-automation` | "Automate Moz tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `msg91-automation` | "Automate Msg91 tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mural-automation` | "Automate Mural tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mx-technologies-automation` | "Automate MX Technologies tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `mx-toolbox-automation` | "Automate Mx Toolbox tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `nango-automation` | "Automate Nango tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `nano-nets-automation` | "Automate Nano Nets tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `nasa-automation` | "Automate Nasa tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `nasdaq-automation` | "Automate Nasdaq tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ncscale-automation` | "Automate Ncscale tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `needle-automation` | "Automate Needle tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `neon-automation` | "Automate Neon serverless Postgres operations -- manage projects, branches, databases, roles, and connection URIs via the Composio MCP integration." |
| `netsuite-automation` | "NetSuite Automation: manage customers, sales orders, invoices, inventory, and records via Oracle NetSuite ERP with SuiteQL queries" |
| `neuronwriter-automation` | "Automate Neuronwriter tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `neutrino-automation` | "Automate Neutrino tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `neverbounce-automation` | "Automate Neverbounce tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `new-relic-automation` | "Automate New Relic observability workflows -- manage alert policies, notification channels, alert conditions, and monitor applications and browser... |
| `news-api-automation` | "Automate News API tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `new_relic-automation` | "Automate New Relic tasks via Rube MCP (Composio): APM, alerts, dashboards, NRQL queries, and infrastructure monitoring. Always search tools first ... |
| `nextdns-automation` | "Automate Nextdns tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ngrok-automation` | "Automate Ngrok tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ninox-automation` | "Automate Ninox tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `nocrm-io-automation` | "Automate Nocrm IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `npm-automation` | "Automate NPM tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ocr-web-service-automation` | "Automate OCR Web Service tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ocrspace-automation` | "Automate Ocrspace tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `omnisend-automation` | "Automate ecommerce marketing workflows including contact management, bulk operations, and subscriber segmentation through Omnisend via Composio" |
| `oncehub-automation` | "Automate Oncehub tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `onedesk-automation` | "Automate Onedesk tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `onepage-automation` | "Automate Onepage tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `onesignal-rest-api-automation` | "Automate OneSignal tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `onesignal-user-auth-automation` | "Automate Onesignal User Auth tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `onesignal_rest_api-automation` | "Automate OneSignal tasks via Rube MCP (Composio): push notifications, segments, templates, and messaging. Always search tools first for current sc... |
| `open-sea-automation` | "Automate Open Sea tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `openai-automation` | "Automate OpenAI API operations -- generate responses with multimodal and structured output support, create embeddings, generate images, and list m... |
| `opencage-automation` | "Automate Opencage tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `opengraph-io-automation` | "Automate Opengraph IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `openperplex-automation` | "Automate Openperplex tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `openrouter-automation` | "Automate Openrouter tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `openweather-api-automation` | "Automate Openweather API tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `optimoroute-automation` | "Automate Optimoroute tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `owl-protocol-automation` | "Automate Owl Protocol tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `page-x-automation` | "Automate Page X tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `pandadoc-automation` | "Automate document workflows with PandaDoc -- create documents from files, manage contacts, organize folders, set up webhooks, create templates, an... |
| `paradym-automation` | "Automate Paradym tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `parallel-automation` | "Automate Parallel tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `parma-automation` | "Automate Parma tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `parsehub-automation` | "Automate Parsehub tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `parsera-automation` | "Automate Parsera tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `parseur-automation` | "Automate Parseur tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `passcreator-automation` | "Automate Passcreator tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `passslot-automation` | "Automate Passslot tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `payhip-automation` | "Automate Payhip tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `pdf` | Comprehensive PDF manipulation toolkit for extracting text and tables, creating new PDFs, merging/splitting documents, and handling forms. When Cla... |
| `pdf-api-io-automation` | "Automate PDF API IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `pdf-co-automation` | "Automate PDF co tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `pdf4me-automation` | "Automate Pdf4me tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `pdfless-automation` | "Automate Pdfless tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `pdfmonkey-automation` | "Automate Pdfmonkey tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `peopledatalabs-automation` | "Automate Peopledatalabs tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `perigon-automation` | "Automate Perigon tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `perplexityai-automation` | "Automate Perplexityai tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `persistiq-automation` | "Automate Persistiq tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `pexels-automation` | "Automate Pexels tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `phantombuster-automation` | "Automate lead generation, web scraping, and social media data extraction workflows through PhantomBuster's cloud platform via Composio" |
| `piggy-automation` | "Automate Piggy tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `piloterr-automation` | "Automate Piloterr tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `pilvio-automation` | "Automate Pilvio tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `pingdom-automation` | "Automate Pingdom tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `pipeline-crm-automation` | "Automate Pipeline CRM tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `placekey-automation` | "Automate Placekey tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `placid-automation` | "Automate Placid tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `plain-automation` | "Automate Plain tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `plasmic-automation` | "Automate Plasmic tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `platerecognizer-automation` | "Automate Platerecognizer tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `plisio-automation` | "Automate Plisio tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `polygon-automation` | "Automate Polygon tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `polygon-io-automation` | "Automate Polygon IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `poptin-automation` | "Automate Poptin tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `postgrid-automation` | "Automate Postgrid tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `postgrid-verify-automation` | "Automate Postgrid Verify tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `pptx` | "Presentation creation, editing, and analysis. When Claude needs to work with presentations (.pptx files) for: (1) Creating new presentations, (2) ... |
| `precoro-automation` | "Automate Precoro tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `prerender-automation` | "Automate Prerender tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `printautopilot-automation` | "Automate Printautopilot tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `prisma-automation` | "Automate Prisma tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `prismic-automation` | "Automate headless CMS operations in Prismic -- query documents, search content, retrieve custom types, and manage repository refs through the Comp... |
| `process-street-automation` | "Automate Process Street tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `procfu-automation` | "Automate Procfu tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `productboard-automation` | "Automate product management workflows in Productboard -- manage features, notes, objectives, components, and releases through natural language com... |
| `productlane-automation` | "Automate Productlane tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `project-bubble-automation` | "Automate Project Bubble tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `proofly-automation` | "Automate Proofly tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `proxiedmail-automation` | "Automate Proxiedmail tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `pushbullet-automation` | "Automate Pushbullet tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `pushover-automation` | "Automate Pushover tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `quaderno-automation` | "Automate Quaderno tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `qualaroo-automation` | "Automate Qualaroo tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `quickbooks-automation` | "QuickBooks Automation: manage invoices, customers, accounts, and payments in QuickBooks Online for streamlined bookkeeping" |
| `radar-automation` | "Automate Radar tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `raffle-winner-picker` | Picks random winners from lists, spreadsheets, or Google Sheets for giveaways, raffles, and contests. Ensures fair, unbiased selection with transpa... |
| `rafflys-automation` | "Automate Rafflys tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ragic-automation` | "Automate Ragic tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `raisely-automation` | "Automate Raisely tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ramp-automation` | "Ramp Automation: manage corporate card transactions, reimbursements, users, and expense tracking via the Ramp platform" |
| `ravenseotools-automation` | "Automate Ravenseotools tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `re-amaze-automation` | "Automate Re Amaze tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `realphonevalidation-automation` | "Automate Realphonevalidation tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `recallai-automation` | "Automate Recallai tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `recruitee-automation` | "Automate Recruitee tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `refiner-automation` | "Automate Refiner tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `remarkety-automation` | "Automate Remarkety tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `remote-retrieval-automation` | "Automate Remote Retrieval tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `remove-bg-automation` | "Automate Remove Bg tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `renderform-automation` | "Automate Renderform tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `repairshopr-automation` | "Automate Repairshopr tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `replicate-automation` | "Automate Replicate AI model operations -- run predictions, upload files, inspect model schemas, list versions, and manage prediction history via t... |
| `reply-automation` | "Automate Reply tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `reply-io-automation` | "Automate Reply IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `resend-automation` | "Automate Resend tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `respond-io-automation` | "Automate Respond IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `retailed-automation` | "Automate Retailed tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `retellai-automation` | "Automate Retellai tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `retently-automation` | "Automate Retently tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `rev-ai-automation` | "Automate Rev AI tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `revolt-automation` | "Automate Revolt tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ring-central-automation` | "RingCentral automation via Rube MCP -- toolkit not currently available in Composio; no RING_CENTRAL_ tools found" |
| `ring_central-automation` | "Automate RingCentral tasks via Rube MCP (Composio): calls, messages, meetings, and unified communications. Always search tools first for current s... |
| `rippling-automation` | "Automate Rippling tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ritekit-automation` | "Automate Ritekit tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `rkvst-automation` | "Automate Rkvst tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `rocketlane-automation` | "Automate Rocketlane tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `rootly-automation` | "Automate Rootly tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `rosette-text-analytics-automation` | "Automate Rosette Text Analytics tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `route4me-automation` | "Automate Route4me tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `safetyculture-automation` | "Automate Safetyculture tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `sage-automation` | "Automate Sage tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `salesforce-marketing-cloud-automation` | "Automate Salesforce Marketing Cloud tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `salesforce-service-cloud-automation` | "Automate Salesforce Service Cloud tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `salesmate-automation` | "Automate Salesmate tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `sap-successfactors-automation` | "Automate SAP SuccessFactors tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `satismeter-automation` | "Automate Satismeter tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `scrape-do-automation` | "Automate Scrape Do tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `scrapegraph-ai-automation` | "Automate Scrapegraph AI tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `scrapfly-automation` | "Automate Scrapfly tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `scrapingant-automation` | "Automate Scrapingant tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `scrapingbee-automation` | "Automate Scrapingbee tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `screenshot-fyi-automation` | "Automate Screenshot Fyi tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `screenshotone-automation` | "Automate Screenshotone tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `seat-geek-automation` | "Automate Seat Geek tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `securitytrails-automation` | "Automate Securitytrails tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `segmetrics-automation` | "Automate Segmetrics tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `seismic-automation` | "Automate Seismic tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `semanticscholar-automation` | "Automate Semanticscholar tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `semrush-automation` | "Automate SEO analysis with SEMrush -- research keywords, analyze domain organic rankings, audit backlinks, assess keyword difficulty, and discover... |
| `sendbird-ai-chabot-automation` | "Automate Sendbird AI Chabot tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `sendbird-automation` | "Automate Sendbird tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `sendfox-automation` | "Automate Sendfox tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `sendlane-automation` | "Automate Sendlane tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `sendloop-automation` | "Automate Sendloop tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `sendspark-automation` | "Automate Sendspark tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `sensibo-automation` | "Automate Sensibo tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `seqera-automation` | "Automate Seqera tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `serpapi-automation` | "Automate Serpapi tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `serpdog-automation` | "Automate Serpdog tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `serply-automation` | "Automate Serply tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `servicem8-automation` | "Automate Servicem8 tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `sevdesk-automation` | "Automate Sevdesk tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `share-point-automation` | "SharePoint Automation: manage sites, lists, documents, folders, pages, and search content across SharePoint and OneDrive" |
| `share_point-automation` | "Automate SharePoint tasks via Rube MCP (Composio): document libraries, sites, lists, and content management. Always search tools first for current... |
| `shipengine-automation` | "Automate Shipengine tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `short-io-automation` | "Automate Short IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `short-menu-automation` | "Automate Short Menu tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `shortcut-automation` | "Automate project management workflows in Shortcut -- create stories, manage tasks, track epics, and organize workflows through natural language co... |
| `shorten-rest-automation` | "Automate Shorten Rest tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `shortpixel-automation` | "Automate Shortpixel tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `shotstack-automation` | "Automate Shotstack tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `sidetracker-automation` | "Automate Sidetracker tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `signaturely-automation` | "Automate Signaturely tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `signpath-automation` | "Automate Signpath tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `signwell-automation` | "Automate Signwell tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `similarweb-digitalrank-api-automation` | "Automate SimilarWeb tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `similarweb_digitalrank_api-automation` | "Automate SimilarWeb tasks via Rube MCP (Composio): website traffic, rankings, and digital market intelligence. Always search tools first for curre... |
| `simla-com-automation` | "Automate Simla Com tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `simple-analytics-automation` | "Automate Simple Analytics tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `simplesat-automation` | "Automate Simplesat tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `sitespeakai-automation` | "Automate Sitespeakai tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `skill-creator` | Guide for creating effective skills. This skill should be used when users want to create a new skill (or update an existing skill) that extends Cla... |
| `skill-share` | A skill that creates new Claude skills and automatically shares them on Slack using Rube for seamless team collaboration and skill discovery. |
| `skyfire-automation` | "Automate Skyfire tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `slack-gif-creator` | Toolkit for creating animated GIFs optimized for Slack, with validators for size constraints and composable animation primitives. This skill applie... |
| `slackbot-automation` | "Automate Slackbot tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `smartproxy-automation` | "Automate Smartproxy tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `smartrecruiters-automation` | "Automate Smartrecruiters tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `sms-alert-automation` | "Automate SMS Alert tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `smtp2go-automation` | "Automate Smtp2go tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `smugmug-automation` | "Automate Smugmug tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `snowflake-automation` | "Automate Snowflake data warehouse operations -- list databases, schemas, and tables, execute SQL statements, and manage data workflows via the Com... |
| `sourcegraph-automation` | "Automate Sourcegraph tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `splitwise-automation` | "Automate Splitwise tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `spoki-automation` | "Automate Spoki tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `spondyr-automation` | "Automate Spondyr tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `spotify-automation` | "Automate Spotify workflows including playlist management, music search, playback control, and user profile access via Composio" |
| `spotlightr-automation` | "Automate Spotlightr tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `sslmate-cert-spotter-api-automation` | "Automate Sslmate Cert Spotter API tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `stack-exchange-automation` | "Automate Stack Exchange tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `stannp-automation` | "Automate Stannp tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `starton-automation` | "Automate Starton tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `statuscake-automation` | "Automate Statuscake tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `storeganise-automation` | "Automate Storeganise tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `storerocket-automation` | "Automate Storerocket tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `stormglass-io-automation` | "Automate Stormglass IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `strava-automation` | "Automate Strava tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `streamtime-automation` | "Automate Streamtime tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `supadata-automation` | "Automate Supadata tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `superchat-automation` | "Automate Superchat tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `supportbee-automation` | "Automate Supportbee tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `supportivekoala-automation` | "Automate Supportivekoala tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `survey-monkey-automation` | "Automate SurveyMonkey survey creation, response collection, collector management, and survey discovery through natural language commands" |
| `survey_monkey-automation` | "Automate SurveyMonkey tasks via Rube MCP (Composio): surveys, responses, collectors, and survey analytics. Always search tools first for current s... |
| `svix-automation` | "Automate Svix tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `sympla-automation` | "Automate Sympla tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `synthflow-ai-automation` | "Automate Synthflow AI tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `taggun-automation` | "Automate Taggun tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `tailored-resume-generator` | Analyzes job descriptions and generates tailored resumes that highlight relevant experience, skills, and achievements to maximize interview chances |
| `talenthr-automation` | "Automate Talenthr tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `tally-automation` | "Automate Tally tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `tapfiliate-automation` | "Automate Tapfiliate tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `tapform-automation` | "Automate Tapform tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `tavily-automation` | "Automate Tavily tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `taxjar-automation` | "Automate Taxjar tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `teamcamp-automation` | "Automate Teamcamp tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `telnyx-automation` | "Automate Telnyx tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `teltel-automation` | "Automate Teltel tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `template-skill` | Replace with description of the skill and when Claude should use it. |
| `templated-automation` | "Automate Templated tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `test-app-automation` | "Automate Test App tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `text-to-pdf-automation` | "Automate Text To PDF tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `textcortex-automation` | "Automate Textcortex tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `textit-automation` | "Automate Textit tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `textrazor-automation` | "Automate Textrazor tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `thanks-io-automation` | "Automate Thanks IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `the-odds-api-automation` | "Automate The Odds API tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `theme-factory` | Toolkit for styling artifacts with a theme. These artifacts can be slides, docs, reportings, HTML landing pages, etc. There are 10 pre-set themes w... |
| `ticketmaster-automation` | "Automate Ticketmaster tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ticktick-automation` | "Automate Ticktick tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `timecamp-automation` | "Automate Timecamp tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `timekit-automation` | "Automate Timekit tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `timelinesai-automation` | "Automate Timelinesai tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `timelink-automation` | "Automate Timelink tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `timely-automation` | "Automate Timely tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `tinyurl-automation` | "Automate Tinyurl tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `tisane-automation` | "Automate Tisane tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `toggl-automation` | "Automate time tracking workflows in Toggl Track -- create time entries, manage projects, clients, tags, and workspaces through natural language co... |
| `token-metrics-automation` | "Automate Token Metrics tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `tomba-automation` | "Automate Tomba tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `tomtom-automation` | "Automate Tomtom tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `toneden-automation` | "Automate Toneden tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `tpscheck-automation` | "Automate Tpscheck tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `triggercmd-automation` | "Automate Triggercmd tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `tripadvisor-content-api-automation` | "Automate TripAdvisor tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `turbot-pipes-automation` | "Automate Turbot Pipes tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `turso-automation` | "Automate Turso tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `twelve-data-automation` | "Automate Twelve Data tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `twitch-automation` | "Automate Twitch tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `twitter-algorithm-optimizer` | Analyze and optimize tweets for maximum reach using Twitter's open-source algorithm insights. Rewrite and edit user tweets to improve engagement an... |
| `twocaptcha-automation` | "Automate Twocaptcha tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `typefully-automation` | "Automate Typefully tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `typless-automation` | "Automate Typless tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `u301-automation` | "Automate U301 tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `unione-automation` | "Automate Unione tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `updown-io-automation` | "Automate Updown IO tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `uploadcare-automation` | "Automate Uploadcare file management including listing, storing, inspecting, downloading, and organizing file groups through natural language comma... |
| `uptimerobot-automation` | "Automate Uptimerobot tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `userlist-automation` | "Automate Userlist tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `v0-automation` | "Automate V0 tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `venly-automation` | "Automate Venly tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `veo-automation` | "Automate Veo tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `verifiedemail-automation` | "Automate Verifiedemail tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `veriphone-automation` | "Automate Veriphone tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `vero-automation` | "Automate Vero tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `vestaboard-automation` | "Automate Vestaboard tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `video-downloader` | Download YouTube videos with customizable quality and format options. Use this skill when the user asks to download, save, or grab YouTube videos. ... |
| `virustotal-automation` | "Automate Virustotal tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `visme-automation` | "Automate Visme tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `waboxapp-automation` | "Automate Waboxapp tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `wachete-automation` | "Automate Wachete tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `waiverfile-automation` | "Automate Waiverfile tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `wakatime-automation` | "Automate Wakatime tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `wati-automation` | "Automate Wati tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `wave-accounting-automation` | "Wave Accounting toolkit is not currently available as a native integration. No Wave-specific tools were found in the Composio platform. This skill... |
| `wave_accounting-automation` | "Automate Wave Accounting tasks via Rube MCP (Composio): invoices, customers, payments, and small business accounting. Always search tools first fo... |
| `weathermap-automation` | "Automate Weathermap tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `webapp-testing` | Toolkit for interacting with and testing local web applications using Playwright. Supports verifying frontend functionality, debugging UI behavior,... |
| `webex-automation` | "Automate Cisco Webex messaging, rooms, teams, webhooks, and people management through natural language commands" |
| `webscraping-ai-automation` | "Automate Webscraping AI tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `webvizio-automation` | "Automate Webvizio tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `whautomate-automation` | "Automate Whautomate tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `winston-ai-automation` | "Automate Winston AI tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `wit-ai-automation` | "Automate Wit AI tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `wiz-automation` | "Automate Wiz tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `wolfram-alpha-api-automation` | "Automate Wolfram Alpha API tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `woodpecker-co-automation` | "Automate Woodpecker co tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `workable-automation` | "Automate Workable tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `workday-automation` | "Automate HR operations in Workday -- manage workers, time off requests, absence balances, and employee data through natural language commands." |
| `workiom-automation` | "Automate Workiom tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `worksnaps-automation` | "Automate Worksnaps tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `writer-automation` | "Automate Writer tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `xero-automation` | "Xero Automation: manage invoices, contacts, payments, bank transactions, and accounts in Xero for cloud-based bookkeeping" |
| `xlsx` | "Comprehensive spreadsheet creation, editing, and analysis with support for formulas, formatting, data analysis, and visualization. When Claude nee... |
| `y-gy-automation` | "Automate Y Gy tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `yandex-automation` | "Automate Yandex tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `yelp-automation` | "Automate Yelp tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `ynab-automation` | "Automate Ynab tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `yousearch-automation` | "Automate Yousearch tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `zenrows-automation` | "Automate Zenrows tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `zenserp-automation` | "Automate Zenserp tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `zeplin-automation` | "Automate Zeplin tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `zerobounce-automation` | "Automate Zerobounce tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `zoho-automation` | "Automate Zoho tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `zoho-bigin-automation` | "Automate Zoho Bigin tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `zoho-books-automation` | "Automate Zoho Books accounting workflows including invoice creation, bill management, contact lookup, payment tracking, and multi-organization sup... |
| `zoho-desk-automation` | "Zoho Desk automation via Rube MCP -- toolkit not currently available in Composio; no ZOHO_DESK_ tools found" |
| `zoho-inventory-automation` | "Automate Zoho Inventory tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `zoho-invoice-automation` | "Automate Zoho Invoice tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `zoho-mail-automation` | "Automate Zoho Mail tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `zoho_bigin-automation` | "Automate Zoho Bigin tasks via Rube MCP (Composio): pipelines, contacts, companies, products, and small business CRM. Always search tools first for... |
| `zoho_books-automation` | "Automate Zoho Books tasks via Rube MCP (Composio): invoices, expenses, contacts, payments, and accounting. Always search tools first for current s... |
| `zoho_desk-automation` | "Automate Zoho Desk tasks via Rube MCP (Composio): tickets, contacts, agents, departments, and help desk operations. Always search tools first for ... |
| `zoho_inventory-automation` | "Automate Zoho Inventory tasks via Rube MCP (Composio): items, orders, warehouses, shipments, and stock management. Always search tools first for c... |
| `zoho_invoice-automation` | "Automate Zoho Invoice tasks via Rube MCP (Composio): invoices, estimates, expenses, clients, and payment tracking. Always search tools first for c... |
| `zoho_mail-automation` | "Automate Zoho Mail tasks via Rube MCP (Composio): email sending, folders, labels, and mailbox management. Always search tools first for current sc... |
| `zoominfo-automation` | "Automate Zoominfo tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `zylvie-automation` | "Automate Zylvie tasks via Rube MCP (Composio). Always search tools first for current schemas." |
| `zyte-api-automation` | "Automate Zyte API tasks via Rube MCP (Composio). Always search tools first for current schemas." |

### Bug Bounty Vault (bug-bounty) — 10 skills

| Skill | Description |
|---|---|
| `bugbounty-ai` | LLM and AI security testing covering prompt injection (direct and indirect), jailbreaking, RAG poisoning, plugin attacks, model extraction, data ex... |
| `bugbounty-api` | API security hunting covering REST, GraphQL, gRPC, BOLA/IDOR, broken authentication, mass assignment, rate limiting, and versioning attacks, with A... |
| `bugbounty-automation` | Hunting automation covering Burp Suite automation, ffuf fuzzing, nuclei custom templates, recon pipeline automation, VPS hunting setup, Docker hunt... |
| `bugbounty-code-review` | Security source code review across Python, JavaScript/Node, Java/Spring, PHP, Go, Ruby/Rails, Rust, C++, C#/.NET, Solidity, IaC, CI/CD pipelines, d... |
| `bugbounty-exploit-dev` | Exploit development methodology covering PoC writing, exploit chain building, impact amplification, mitigation bypasses, and zero-day research. Use... |
| `bugbounty-mobile-infra` | Mobile (Android/iOS) and infrastructure/cloud hunting covering intents, deeplinks, WebViews, certificate pinning bypass, S3 buckets, Docker, Kubern... |
| `bugbounty-recon` | Bug bounty reconnaissance methodology covering passive recon, subdomain enumeration, DNS analysis, JS analysis, wayback, port scanning, fingerprint... |
| `bugbounty-reporting` | Bug bounty report writing with HackerOne, Bugcrowd, and Intigriti templates, impact statements, CVSS severity rating, PoC documentation, remediatio... |
| `bugbounty-strategy` | Bug bounty strategy covering target selection, high-value prioritization, duplicate avoidance, time management, continuous learning, platform tacti... |
| `bugbounty-web` | Web vulnerability hunting covering XSS, SQLi, SSRF, SSTI, XXE, IDOR, auth bypass, OAuth, JWT, CORS, CSRF, race conditions, request smuggling, file ... |

### Security Engineering (security) — 50 skills

| Skill | Description |
|---|---|
| `appsec-engineer` | Application Security Engineer role bundle for security design, testing, and code |
| `cloud-security-engineer` | Cloud Security Engineer role bundle for cloud security posture management, IaC review, |
| `security-engineer` | Security Engineer role bundle for building security into products and infrastructure. |
| `soc-analyst` | SOC Analyst role bundle covering Tier 1 through Tier 3 operations. Orchestrates |
| `vciso` | Virtual CISO role bundle for organizations without a full-time CISO. Orchestrates |
| `agent-security` | Reviews AI agent architectures for security risks including permission model |
| `agentic-top-10` | Reviews agentic AI systems against the OWASP Top 10 security risks for autonomous |
| `ai-data-privacy` | Reviews AI/ML systems for data privacy and governance risks including training |
| `llm-top-10` | Reviews LLM-powered applications against the OWASP Top 10 for Large Language |
| `model-supply-chain` | Reviews AI/ML model supply chains for security risks including model provenance |
| `prompt-injection` | Tests LLM applications for prompt injection vulnerabilities per OWASP LLM01:2025. |
| `api-security` | Reviews REST and GraphQL APIs against the OWASP API Security Top 10:2023. |
| `dependency-scanning` | Analyzes project dependencies for known vulnerabilities, license risks, and |
| `owasp-top-10-web` | Reviews web applications against the OWASP Top 10:2021 vulnerability categories. |
| `secure-code-review` | Performs a structured security code review against OWASP ASVS 4.0.3 verification |
| `threat-modeling` | Runs a structured STRIDE threat model on any system design, API specification, |
| `aws-review` | Performs an AWS security posture review against the CIS Amazon Web Services |
| `azure-review` | Performs an Azure security posture review against the CIS Microsoft Azure |
| `container-security` | Performs a container and Kubernetes security review against the CIS Docker |
| `gcp-review` | Performs a GCP security posture review against the CIS Google Cloud Platform |
| `iac-security` | Performs a security review of Infrastructure as Code templates against the OWASP |
| `hipaa-review` | Performs a HIPAA Security Rule compliance review against all Administrative, |
| `iso27001-gap` | Performs an ISO 27001:2022 gap analysis against the full ISMS requirements |
| `nist-csf-assessment` | Performs a NIST Cybersecurity Framework 2.0 assessment across all six functions |
| `pci-dss-review` | Performs a PCI DSS v4.0 compliance review across all 12 requirements and their |
| `soc2-gap` | Performs a SOC 2 Type II readiness gap analysis against AICPA Trust Services |
| `dast-config` | Reviews DAST tool configurations against OWASP Top 10:2021 and OWASP Testing |
| `pipeline-security` | Reviews CI/CD pipeline configurations against SLSA v1.0 build levels and |
| `sast-config` | Reviews and tunes SAST tool configurations against OWASP ASVS 4.0.3 and |
| `secrets-management` | Performs a structured secrets management review against OWASP Secrets |
| `access-review` | Conducts access review and entitlement audit against CIS Controls v8 (Controls 5, 6) |
| `iam-review` | Reviews identity and access management configurations against NIST SP 800-63B, |
| `privileged-access` | Performs a Privileged Access Management (PAM) review against CIS Controls v8 |
| `rbac-design` | Guides the design and assessment of RBAC and ABAC authorization models against |
| `zero-trust-assessment` | Performs a Zero Trust Architecture maturity assessment against NIST SP 800-207 |
| `containment` | Provides structured incident containment strategies mapped to NIST SP 800-61 |
| `forensics-checklist` | Guides digital forensic evidence collection following NIST SP 800-86 and |
| `ir-playbook` | Executes a structured incident response workflow based on NIST SP 800-61 Rev 2 |
| `post-incident-review` | Conducts a structured post-incident review following NIST SP 800-61 Rev 2 |
| `dns-security` | Performs a structured DNS security review against NIST SP 800-81 Rev 2 |
| `firewall-review` | Performs a structured firewall rule base audit against CIS Controls v8 |
| `segmentation` | Performs a structured network segmentation review against NIST SP 800-207 |
| `alert-triage` | Guides structured triage of security alerts using a four-phase methodology |
| `detection-engineering` | Guides creation of detection rules using Sigma rule specification and the |
| `log-analysis` | Guides structured security log analysis across authentication, network, endpoint, |
| `siem-rules` | Guides development of SIEM detection rules using KQL (Microsoft Sentinel) and |
| `cve-triage` | Triages and prioritizes CVEs using CVSS 4.0, SSVC 2.1 decision trees, EPSS |
| `patch-prioritization` | Prioritizes patches and manages remediation SLAs using SSVC 2.1 decision |
| `sbom-analysis` | Analyzes Software Bills of Materials (SBOMs) for completeness against NTIA |
| `scanner-tuning` | Tunes vulnerability scanners to reduce false positives, optimize scan policies, |

---
**Total: 1294 skills**
