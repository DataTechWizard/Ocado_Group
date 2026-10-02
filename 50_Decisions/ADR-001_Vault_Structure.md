---
tags:
  - decision
  - accepted
created: 2026-10-02
updated: 2026-10-02
---

# ADR-001: Adopt Obsidian Vault as Primary Knowledge Base

## Status

✅ **Accepted** — 2026-10-02

## Context

Starting a new Data Implementation Engineer (DE2) role at Ocado Group (OSP division). Need a system that:
- Serves as both a **knowledge base** and a **codebase** reference
- Is **AI-agent friendly** (markdown, structured, file-based)
- Supports **bidirectional linking** between concepts (stakeholders ↔ tech ↔ partners ↔ bugs)
- Works **offline** and is **version-controlled** via Git
- Scales from onboarding through long-term institutional memory

## Decision

Adopt an **Obsidian vault** with a numbered folder structure (`00_Inbox` through `90_Templates`) as the primary knowledge base. All documentation, decisions, learnings, and agent context will live here alongside the codebase.

## Consequences

### Positive
- Wikilinks enable fast cross-referencing between any two concepts
- YAML frontmatter enables Dataview queries and structured metadata
- Git-backed = full audit trail, branching, collaboration
- AI agents can read/write plain markdown files natively
- Zero vendor lock-in — it's just folders and `.md` files

### Negative
- Requires discipline to maintain folder conventions
- Obsidian-specific plugins (Dataview, Templater) add convenience but are optional
- Binary assets (screenshots, diagrams) need to be stored thoughtfully

## Alternatives Considered

| Option | Why Not |
|---|---|
| Notion | Not file-based, poor Git integration, vendor lock-in |
| Confluence | Ocado's internal tool may differ; this is personal KB |
| Plain markdown (no vault) | Loses bidirectional linking and graph view |

---

See also: [[Decisions]]
