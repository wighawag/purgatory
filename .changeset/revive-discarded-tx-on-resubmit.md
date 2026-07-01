---
'purgatory-core': patch
---

Fix UNIQUE constraint crash when resubmitting a previously discarded transaction. `addTransaction` now uses `ON CONFLICT(hash) DO UPDATE`, so a client resubmitting the same raw transaction revives the existing row back to `pending` (clearing `deleted_at`, `dropped_at`, `drop_reason`, `forwarded_at` and refreshing `created_at`) instead of throwing `SQLITE_CONSTRAINT_PRIMARYKEY`.
