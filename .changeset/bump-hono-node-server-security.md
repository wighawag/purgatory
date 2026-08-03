---
'purgatory': patch
---

Bump `@hono/node-server` from `^1.13.8` to `^2.0.12`, clearing GHSA-frvp-7c67-39w9, which has no fix on the 1.x line.

This is a runtime dependency of the published `purgatory` binary, so consumers pick up the new major on install. The only API used here is `serve({fetch, port})`, which is unchanged in 2.x; the server was started and verified to answer requests. Note that `@hono/node-server` 2.x requires **Node >= 20**.
