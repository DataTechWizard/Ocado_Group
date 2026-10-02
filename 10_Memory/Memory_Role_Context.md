---
tags:
  - memory
  - context
created: 2026-10-02
updated: 2026-10-02
---

# Role Context

## Position
- **Title:** Senior Data Engineer (Implementation & Analytics)
- **Division:** Ocado Smart Platform (OSP)
- **Salary:** £85,000
- **Start Date:** 5 October 2026
- **Location:** Trident Place (hybrid)

## Mandate

This is a **partner-facing implementation, QA, migration, and governance role**. The core challenge is maintaining a **canonical OSP measurement contract** (a core event model) while handling partner-specific extensions and exceptions.

> [!IMPORTANT]
> An error here isn't isolated to one retailer — it gets copied across markets and affects partner trust.

## Primary Responsibilities

1. **Asda GA4 Build** — Greenfield implementation from scratch (or migration to OSP framework) following their recent signing as a major UK partner
2. **GA4 & App Expertise** — Hands-on GA4, GTM, Firebase configuration; the capability Andy Wicks explicitly said he needs to lean on
3. **BigQuery Exports** — Managing and validating GA4 BigQuery export pipelines
4. **Retail Media Reporting** — `creative_slot`, `item_promotion`, promotion attribution
5. **Legacy Migrations** — Moving partners from older tracking systems to the canonical OSP event model
6. **Governance** — Ensuring the canonical measurement contract stays consistent across 15+ global partners

## Technical Proof Delivered (Pre-Hire)

**FreshCart Demo:** Demonstrated how to fix a `customer_type` sequencing defect where a first-time buyer was labelled "returning" by the time the order was measured. Solution: move the flag out of `placeOrder()` to fire *after* the `purchase` event.

---

See also: [[Memory_Stakeholders]] | [[Memory_Tech_Stack]] | [[Memory_Partner_Map]]
