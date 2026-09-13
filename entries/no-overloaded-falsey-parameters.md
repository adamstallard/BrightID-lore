---
id: no-overloaded-falsey-parameters
claim: Do not give a parameter a second meaning when it is absent or falsey — add a
  separate function or a separate flag instead.
scope: global
status: active
conditions:
  prose: When a parameter or field would carry a magic value, or one field would encode
    several independent states.
provenance:
  - url: https://github.com/BrightID/BrightID-Node/pull/176#discussion_r550873682
    author: adamstallard
    at: 2021-01-02
  - url: https://github.com/BrightID/BrightID-Node/pull/264#discussion_r762520038
    author: adamstallard
    at: 2021-12-05
supersedes: []
reviewed:
  by: adamstallard
  at: 2026-09-13
---

Both instances argue the same way: the reader needs hidden knowledge to understand the call. Splitting into `removeAllSubkeys`, or into two booleans rather than a three-valued `state`, makes the possibilities visible in the names.
