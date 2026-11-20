---
name: bugbounty-api
description: API security hunting covering REST, GraphQL, gRPC, BOLA/IDOR, broken authentication, mass assignment, rate limiting, and versioning attacks, with API checklists and attack scenarios. Use when the user tests an API, asks about GraphQL introspection or BOLA, needs API fuzzing methodology, or reviews API authorization.
license: MIT
---

# Bug Bounty API Security

API hunting guides (paths relative to `BugBountySkills/`).

## Guides

- `../../SKILL_FILES/VULNERABILITIES/API/` — `../../SKILL_FILES/VULNERABILITIES/API/rest_api_attacks.md`,
  `../../SKILL_FILES/VULNERABILITIES/API/graphql_introspection_attacks.md`, `../../SKILL_FILES/VULNERABILITIES/API/grpc_attacks.md`,
  `../../SKILL_FILES/VULNERABILITIES/API/api_authentication_attacks.md`, `../../SKILL_FILES/VULNERABILITIES/API/api_authorization_bypass.md`,
  `../../SKILL_FILES/VULNERABILITIES/API/api_mass_assignment.md`, `../../SKILL_FILES/VULNERABILITIES/API/api_rate_limiting_bypass.md`,
  `../../SKILL_FILES/VULNERABILITIES/API/api_versioning_attacks.md`, `../../SKILL_FILES/VULNERABILITIES/API/api_fuzzing_methodology.md`.
- `../../SKILL_FILES/VULNERABILITIES/WEB/graphql_attacks.md` for web-context GraphQL.
- `../../KNOWLEDGE_BASE/API_Security/` — `../../KNOWLEDGE_BASE/ReDoS/theory.md`, `../../KNOWLEDGE_BASE/ReDoS/hunting-methodology.md`,
  `../../KNOWLEDGE_BASE/ReDoS/attack-scenarios.md`, `../../KNOWLEDGE_BASE/ReDoS/bypasses.md`, `../../KNOWLEDGE_BASE/ReDoS/chaining.md`, `../../KNOWLEDGE_BASE/ReDoS/cheatsheet.md`,
  `../../KNOWLEDGE_BASE/ReDoS/payloads.md`, `../../KNOWLEDGE_BASE/ReDoS/tools.md`, `../../KNOWLEDGE_BASE/ReDoS/reports-index.md`.
- `../../CHECKLISTS/api_general.md`, `../../CHECKLISTS/graphql.md`, `../../CHECKLISTS/idor.md`.

## How to work

1. Discover the full API surface (see `bugbounty-recon` API discovery) including
   versions, undocumented endpoints, and GraphQL introspection.
2. Test authorization first (BOLA/BFLA across every object reference), then
   authentication, mass assignment, rate limits, and business logic.
