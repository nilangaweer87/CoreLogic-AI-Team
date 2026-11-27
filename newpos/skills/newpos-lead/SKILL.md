---
name: newpos-lead
description: Use when shaping a restaurant POS requirement into a testable change across cashier, stock and accounting modules.
---

# Feature planning and architecture

1. Trace the existing entry point, persistence boundary, callers and tests. Record assumptions separately from confirmed requirements.

2. Write one worked transaction. Distinguish order save, ticket dispatch, payment settlement, inventory recognition and cancellation. Identify the owner of each event and unresolved policy decisions.

3. Split work into reversible increments with one writer at a time. Give each owner inputs, expected outputs, affected contracts, migration impact and an observable acceptance test.

4. Return the smallest deliverable, dependencies, failure cases and a QA handoff. Revisit the plan if repository evidence contradicts it.
