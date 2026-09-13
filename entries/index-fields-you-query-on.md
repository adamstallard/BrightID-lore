---
id: index-fields-you-query-on
claim: Any field used to look up or filter documents needs an index, declared in initdb.
scope: global
status: active
conditions:
  paths:
    - web_services/**/*.js
    - "**/initdb.js"
  prose: When adding a collection, a query, or a field that will be searched.
provenance:
  - url: https://github.com/BrightID/BrightID-Node/pull/120#discussion_r487450804
    author: adamstallard
    at: 2020-09-12
  - url: https://github.com/BrightID/BrightID-Node/pull/176#discussion_r550863594
    author: adamstallard
    at: 2021-01-02
  - url: https://github.com/BrightID/BrightID-Node/pull/242#discussion_r677157739
    author: adamstallard
    at: 2021-07-27
  - url: https://github.com/BrightID/BrightID-Node/pull/235#discussion_r635967685
    author: adamstallard
    at: 2021-05-20
  - url: https://github.com/BrightID/BrightID-Node/pull/235#discussion_r635964885
    author: adamstallard
    at: 2021-05-20
  - url: https://github.com/BrightID/BrightID-Node/pull/176#discussion_r550867566
    author: adamstallard
    at: 2021-01-02
supersedes: []
reviewed:
  by: adamstallard
  at: 2026-09-13
---

Raised repeatedly over four years, usually after a query was written against an unindexed field. Indexes live in `initdb.js`, and the list there has drifted from what the code actually queries more than once.
