---
name: newpos-finance
description: Use for sales, settlement, journal mappings, stock valuation, period close and finance regression tests.
---

# Posting and reconciliation

1. Pin down the source event, business date, currency, rounding, approved tax configuration, account mapping and reversal policy.

2. Build expected journals independently of implementation. For a tax-free cash sale of 1,000 costing 600 under perpetual inventory, expect Dr Cash 1,000 / Cr Sales 1,000 and Dr Cost of Sales 600 / Cr Inventory 600.

3. Trace receipts, tenders, returns and credit sales into journals and subledgers. Reconcile by outlet and period. Separate cash collection from revenue recognition where applicable.

4. Replay the same event and reverse a posted example. Verify equal debits and credits, one posting per source and an auditable reversal. Report expected versus actual balances.
