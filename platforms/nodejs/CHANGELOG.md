# purgatory

## 0.0.8

### Patch Changes

- 1e93743: Bump `@hono/node-server` from `^1.13.8` to `^2.0.12`, clearing GHSA-frvp-7c67-39w9, which has no fix on the 1.x line.

  This is a runtime dependency of the published `purgatory` binary, so consumers pick up the new major on install. The only API used here is `serve({fetch, port})`, which is unchanged in 2.x; the server was started and verified to answer requests. Note that `@hono/node-server` 2.x requires **Node >= 20**.

- Updated dependencies [05846ea]
  - purgatory-core@0.0.7

## 0.0.7

### Patch Changes

- latest deps
- Updated dependencies
  - purgatory-core@0.0.6

## 0.0.6

### Patch Changes

- Updated dependencies [8d6b3ce]
  - purgatory-core@0.0.5

## 0.0.5

### Patch Changes

- Updated dependencies
  - purgatory-core@0.0.4

## 0.0.4

### Patch Changes

- Updated dependencies
  - purgatory-core@0.0.3

## 0.0.3

### Patch Changes

- new style
- Updated dependencies
  - purgatory-core@0.0.2

## 0.0.2

### Patch Changes

- readme

## 0.0.1

### Patch Changes

- first release
- Updated dependencies
  - purgatory-core@0.0.1
