---
tags:
  - memory
  - tech-stack
created: 2026-10-02
updated: 2026-10-02
---

# Tech Stack

> [!NOTE]
> This is the **known** tech stack from the interview context. Update as access is granted and real systems are discovered.

## Analytics & Measurement

| Technology | Purpose | Status |
|---|---|---|
| **Google Analytics 4 (GA4)** | Core web/app analytics | Primary — canonical OSP implementation |
| **Google Tag Manager (GTM)** | Tag deployment & management | Server-side + client-side containers |
| **Firebase Analytics** | Mobile app analytics | App-side event collection |
| **BigQuery** | GA4 export & data warehouse | Raw event export + reporting queries |

## Retail Media & Reporting

| Technology | Purpose | Notes |
|---|---|---|
| GA4 Ecommerce Events | `creative_slot`, `item_promotion` | Retail media attribution |
| BigQuery | Reporting pipelines | Partner-facing dashboards |

## Internal Platforms

| Platform | Purpose | Notes |
|---|---|---|
| Workday | HR & People management | Post-onboarding access |
| Fuse | Internal knowledge base | TBC |
| Slack | Communication | Primary comms channel |
| Digital Workplace | IT & productivity tools | TBC |
| Ocado Learning | Compliance training | [Link](http://links.ocado.com/learning) |

## Key Concepts

- **OSP Event Model** — The canonical measurement contract that all partners inherit
- **Partner Extensions** — Custom events/parameters specific to a partner's vertical needs
- **Partner Exceptions** — Deviations from the canonical model (governed, documented)

---

See also: [[Memory_Role_Context]] | [[Memory_Partner_Map]]
