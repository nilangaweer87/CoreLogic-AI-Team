---
name: newpos-stock
description: Use when building receiving, stock transfers, batch production, counts, recipe costing or inventory reconciliation.
---

# Inventory and production controls

1. Identify item, base unit, pack conversion, location, batch, quantity, unit cost and the movement’s source ID. Use exact decimal quantities and explicit rounding.

2. Build a movement table with opening units and value. Exercise purchase, transfer, recipe consumption, actual output, waste and closing count as applicable. Account for both sides of transfers.

3. Retry a receipt and simulate competing issues against the last available unit. Verify the configured negative-stock policy, transaction atomicity and movement uniqueness.

4. For cancellations distinguish prepared, served, wasted and physically returned stock. Reconcile movement totals and valuation to approved accounting policy and produce a worked example.
