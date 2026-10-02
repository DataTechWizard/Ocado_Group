---
tags:
  - learning
  - ga4
  - event-sequencing
created: 2026-10-02
updated: 2026-10-02
---

# Learning 001: GA4 Event Sequencing — `customer_type` Defect

## TL;DR

When a state-mutating operation (like `placeOrder()`) runs **before** the analytics event that should capture the pre-mutation state, you get incorrect attribute values in your data.

## The Problem

In the FreshCart demo scenario:
1. User is a **first-time buyer** (`customer_type = "new"`)
2. `placeOrder()` executes and flips `customer_type` to `"returning"`
3. The `purchase` GA4 event fires and reads `customer_type`
4. Result: The purchase event records `"returning"` for what was actually a first purchase

## The Fix

Move the state mutation (`customer_type` flag update) to **after** the `purchase` event fires. The analytics event should always capture the state **at the time of the user action**, not after server-side processing.

```
❌ placeOrder() → mutate customer_type → fire purchase event
✅ fire purchase event → placeOrder() → mutate customer_type
```

## Why It Matters

- This is a **class of bug**, not a one-off. Any time you have mutation-before-measurement, you'll get stale or incorrect data.
- In OSP, this pattern could affect **every partner** if it exists in the canonical event model.
- Always audit the sequencing of state mutations relative to analytics event dispatch.

## Related

- [[40_Bugs/Bugs|Bugs]] — BUG-000 (FreshCart demo)

---

See also: [[Learnings]]
