# purgatory-core

## 0.0.7

### Patch Changes

- 05846ea: Fix UNIQUE constraint crash when resubmitting a previously discarded transaction. `addTransaction` now uses `ON CONFLICT(hash) DO UPDATE`, so a client resubmitting the same raw transaction revives the existing row back to `pending` (clearing `deleted_at`, `dropped_at`, `drop_reason`, `forwarded_at` and refreshing `created_at`) instead of throwing `SQLITE_CONSTRAINT_PRIMARYKEY`.

## 0.0.6

### Patch Changes

- latest deps

## 0.0.5

### Patch Changes

- 8d6b3ce: memory leak prevention

## 0.0.4

### Patch Changes

- hidden tx

## 0.0.3

### Patch Changes

- fix nonce when gap

## 0.0.2

### Patch Changes

- new style

## 0.0.1

### Patch Changes

- first release
