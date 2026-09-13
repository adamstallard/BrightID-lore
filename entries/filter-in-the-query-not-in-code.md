---
id: filter-in-the-query-not-in-code
claim: Filter and aggregate in the database query rather than fetching a collection and
  searching it in application code.
scope: global
status: provisional
conditions:
  paths:
    - web_services/**/*.js
    - scorer/**/*.py
  prose: When a handler reads a collection to find a subset, or recomputes a value on
    every request.
provenance:
  - url: https://github.com/BrightID/BrightID-Node/pull/242#discussion_r677157739
    author: adamstallard
    at: 2021-07-27
  - url: https://github.com/BrightID/BrightID-Node/pull/145#discussion_r521327674
    author: abramsymons
    at: 2020-11-11
  - url: https://github.com/BrightID/BrightID-Node/pull/145#discussion_r522428028
    author: abramsymons
    at: 2020-11-12
  - url: https://github.com/BrightID/BrightID-Node/pull/304#discussion_r906735992
    author: adamstallard
    at: 2022-06-25
supersedes: []
---

Framed as cost on every call, not as style. Two variants appear: filtering client-side what the query could filter, and recomputing per request what could be computed once and stored.
