# Agents

> AI agent configurations, roles, and interaction logs. Each agent has a defined purpose, context window, and set of tools.

#agent

---

## Active Agents

| Agent | Role | Context Source | Status |
|---|---|---|---|
| [[Agent_Senior_Data_Engineer]] | Primary coding & architecture partner | Full vault (Memory + Code) | ✅ Active |
| [[Agent_QA_Validator]] | Validates GA4 event schemas & data quality | Memory + Bugs + Code | 🟡 Planned |
| [[Agent_Research]] | Web research, documentation lookup | Web + Docs | 🟡 Planned |

---

## Agent Design Principles

1. **Context-first** — Every agent reads from `10_Memory/` before acting
2. **Scoped** — Agents only access the folders relevant to their role
3. **Logged** — All significant agent decisions are recorded in `50_Decisions/`
4. **Learnable** — Agent mistakes become entries in `60_Learnings/`
