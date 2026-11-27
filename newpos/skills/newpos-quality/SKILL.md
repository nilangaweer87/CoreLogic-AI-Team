---
name: newpos-quality
description: Use for independent acceptance, regression and release decisions on POS, accounting, inventory and offline workflows.
---

# Independent QA and release evidence

1. Derive expected results from the approved business rule before reading implementation output. Record build, environment, fixtures and expected balances.

2. Run an end-to-end sale with separate order save and settlement. Inspect receipt, printer jobs, tender, base-unit stock and journal records independently. Reconcile counts and amounts.

3. Test retries before and after commit, two terminals, printer acknowledgment loss, offline reconnection, rounding, split tender, and both cancellation types. Check cashier/manager permissions and cross-tenant isolation using development fixtures.

4. For each failure record reproducible steps, expected versus actual, evidence and severity. Re-run the failing case after the fix and test adjacent flows. Mark unexecuted checks explicitly; base release advice on observed results.
