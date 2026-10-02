# Ocado Group: Project Knowledge Base & Initiation

This document serves as the master knowledge base for the Ocado Group project. It bridges the entire pre-employment journey—from the initial application to the final offer—into Day 1 execution. It is designed to give any future AI agents full historical context of the role's mandate, the technical problems discussed, the core business context, and the starting logistics.

## 1. The Core Business Problem & Role Mandate
Ocado Group is a technology platform business, not just an internal retailer. This role sits within the **Ocado Smart Platform (OSP)** division, which provides end-to-end online grocery technology to 15 leading grocery partners globally (including their newest major UK signing, **Asda**). 

**The Mandate:** This is a partner-facing implementation, QA, migration, and governance role. The core challenge is maintaining a **canonical OSP measurement contract** (a core event model) while handling partner-specific extensions and exceptions. An error here isn't isolated to one retailer; it gets copied across markets and affects partner trust. 
*   **Primary Account:** A major focus of this role will be building Asda’s GA4 implementation from scratch (or migrating them to the OSP framework) following their recent signing.
*   **Technical Scope:** Hands-on GA4 and app expertise, GTM/Firebase configuration, BigQuery exports, retail media reporting (e.g., `creative_slot`, `item_promotion`), and legacy migrations.

## 2. Key Stakeholders & Org Chart
*   **Sam Lloyd:** VP Data Analytics and AI. The department head this role ultimately reports up to (interviewed at Stage 3).
*   **Katie Driver:** Interim VP Partner Growth. Works closely with Sam and the Ecom Analysts (interviewed at Stage 3).
*   **Chandni Vaja:** Line Manager. Ran Stage 1 and Stage 2 interviews. Will lead the onboarding and assign a buddy in week one.
*   **Andy [Wicks]:** Product Manager for GA4 in OSP technology. Owned the technical side of the GA4 implementation since 2022. Technical interviewer at Stage 2. He explicitly noted his biggest need is hands-on GA4 and app expertise he can lean on.
*   **Jonathan Trillwood:** Recruitment Business Partner (Technology). Handled the offer, negotiations, and logistics.

## 3. The Interview Journey & Technical Proofs
*   **August 2026:** CV and Covering Letter submitted, heavily tailored around GA4 implementation, data engineering, and governance.
*   **3rd September 2026 - Stage 2 (Technical):** Interviewed with Chandni and Andy. The focus was heavily on hands-on GA4 and app expertise. 
    *   *Technical Proof (FreshCart Demo):* Following this interview, Mehdi built a FreshCart demo build for Ocado to practically demonstrate his technical capability. Specifically, he demonstrated how to fix a `customer_type` sequencing defect (where a first-time buyer was labelled returning by the time the order was measured) by moving the flag out of `placeOrder()` to after the `purchase` event.
*   **14th September 2026 - Stage 3 (Values):** Interviewed with Sam Lloyd and Katie Driver. A warm, low-friction culture and values fit interview focused on commercial impact.
*   **21st-24th September 2026 - Offer & Negotiation:** Successfully held ground during salary negotiations, securing the target £85k. The formal offer and DocuSign were completed on the 24th.

## 4. Essential Links & Resources
*   **Compliance Training (Ocado Learning):** [http://links.ocado.com/learning](http://links.ocado.com/learning)
*   **Equipment Orders (TSS):** [IT Equipment Form](https://docs.google.com/forms/d/e/1FAIpQLSfKYojRxe11sAZHZc0Uk3U8xSDdYHJy5is_dknlAC42QA4sPQ/viewform)
*   **Internal Systems (Accessible post-setup):** Workday, Fuse, Slack, Digital Workplace

## 5. Day 1 Logistics & First Week Objectives
*   **Arrival (Oct 5 @ 10:00 AM):** Report to reception at Trident Place. **Bring a valid physical photo ID** (Passport/Driver's License). A temporary pass will be issued, and a photo taken for the permanent card.
*   **IT Setup:** Meet with Technology Support Services (TSS) at Trident 2, Ground Floor. Face-to-face setup (60–75 mins) + system reset (30 mins). *Action: Securely log all passwords issued by TSS immediately.*
*   **Training:** Complete 4–5 legal compliance modules (Ocado Learning) during the first week.
*   **Induction:** Chandni will schedule meetings once the work email is active. Await invite from the People Team for the New Starter welcome meeting (includes live CFC robotics tour).
*   **Admin:** Await update from Benefits team regarding opting out of pension auto-enrolment for the first few months.
