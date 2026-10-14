# gaia-public

**Status:** Proposed architecture component — not implemented.

**Domain:** Public-Facing Frontend and API Surface

**Visibility:** Public

**Source:** [GAIA Super-Intelligent Application Architecture Report](https://github.com/KyleAlexanderSteen/GAIA-Documentation) (2026-10-13)

**Traceability:** GAIA-Documentation issues #1–#6

## Purpose
Consumer product: web/mobile interfaces, public API docs, authentication UI, conversation interface, file upload, memory dashboard, tool marketplace, and subscription management.

## Initial Directory Structure (proposed)
```
gaia-public/
├── web/             # Next.js frontend
├── mobile/          # React Native
├── docs/            # OpenAPI documentation site
├── README.md
└── tests/
```

## Proposed Interfaces and Dependencies
- Calls: gaia-api-gateway (all intelligence), gaia-security (auth)
- Depends on: gaia-core, gaia-sdk
- Does not call internal services directly.

## Security and Access-Control Requirements
- Public auth flows (OAuth, email/password).
- Plan-based feature gates.
- No secrets in repo.

## Tests and Acceptance Criteria
- [ ] UI scaffolding and plan feature matrix placeholders.
- [ ] No live public product claimed.
- [ ] Compliance targets labeled as planned (see #6).
- Linked to GAIA-Documentation #1, #6.

## Development Instructions
Scaffolding only. Do not invent implemented chat UI or billing.

**Unresolved:** Exact plan quotas, UI framework versions, data residency choices.
