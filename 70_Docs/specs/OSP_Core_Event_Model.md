---
tags:
  - docs
  - specs
  - ga4
  - partner/osp
status: ⬜ Awaiting Internal Access
created: 2026-10-02
updated: 2026-10-02
---

# OSP Core Event Model — Canonical Measurement Contract

> [!IMPORTANT]
> This is a **placeholder**. Populate this document the moment you gain access to Ocado's internal event dictionary. This is the single most critical reference in the vault — every partner implementation inherits from it.

---

## Event Schema

> _To be documented from internal sources during Week 1–2 discovery._

### Ecommerce Events (GA4 Standard)

| Event Name | Required Parameters | OSP Custom Parameters | Notes |
|---|---|---|---|
| `page_view` | | | |
| `view_item` | `item_id`, `item_name` | | |
| `view_item_list` | `item_list_id`, `item_list_name` | | |
| `add_to_cart` | `items[]` | | |
| `remove_from_cart` | `items[]` | | |
| `begin_checkout` | `items[]`, `value`, `currency` | | |
| `purchase` | `transaction_id`, `value`, `items[]` | `customer_type`? | ⚠️ Verify sequencing — see [[Learning_001_Customer_Type_Sequencing]] |
| `view_promotion` | `creative_slot`, `item_promotion` | | Retail media |
| `select_promotion` | `creative_slot`, `item_promotion` | | Retail media |

### Custom OSP Events

| Event Name | Parameters | Purpose | Notes |
|---|---|---|---|
| _TBC_ | | | _Discover during onboarding_ |

---

## Item Schema

| Parameter | Type | Required | Description |
|---|---|---|---|
| `item_id` | `string` | ✅ | Product SKU |
| `item_name` | `string` | ✅ | Product display name |
| `item_brand` | `string` | | Brand name |
| `item_category` | `string` | | Primary category |
| `price` | `number` | | Unit price |
| `quantity` | `integer` | | Quantity in cart/order |
| _TBC_ | | | _OSP-specific extensions_ |

---

## Partner Extension Rules

> _How partners can extend the canonical model without breaking it._

1. **Allowed:** Adding new custom parameters to existing events (prefixed with partner namespace)
2. **Allowed:** Adding net-new custom events (must not collide with canonical event names)
3. **Not Allowed:** Modifying required parameter names or types on canonical events
4. **Not Allowed:** Removing required parameters from canonical events
5. **Requires ADR:** Any exception to the above rules → log in [[50_Decisions/Decisions|Decisions]]

---

## Questions to Resolve in Discovery

- [ ] Where is the canonical event model documented internally? (Confluence? Fuse? Code?)
- [ ] Who owns the event model governance process?
- [ ] How are partner extensions currently tracked?
- [ ] Is there an automated schema validation step in the deployment pipeline?
- [ ] What does the Asda-specific extension scope look like?

---

See also: [[Docs]] | [[Memory_Tech_Stack]] | [[Memory_Partner_Map]]
