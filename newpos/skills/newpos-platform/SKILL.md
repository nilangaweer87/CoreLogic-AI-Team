---
name: newpos-platform
description: Use for database, API, offline synchronization, tenant isolation, migrations and printer integrations.
---

# Reliable transaction engineering

1. Trace the production entry point and identify the transaction boundary. Scope identifiers and authorization to tenant, outlet and role on the server.

2. Use stable operation IDs, a database uniqueness constraint and atomic state changes. Return the original outcome for a matching replay and reject a reused ID carrying different data.

3. Keep external printer work in a durable queue and distinguish delivery, acknowledgment and reprint. Reconcile after reconnect without duplicating a receipt, journal or stock movement.

4. Exercise concurrent writers and interrupted operations on synthetic data. Rehearse schema upgrades and restore an earlier backup in isolation. Report commands, observed outcomes and recovery steps.
