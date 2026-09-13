---
id: api-errors-carry-an-errornum
claim: An error that can reach the API must carry an ErrorNum, and callers should catch
  a specific error type rather than catching everything and comparing.
scope: global
status: active
conditions:
  paths:
    - web_services/**/*.js
  prose: When throwing from code reachable by a request handler, or when catching.
provenance:
  - url: https://github.com/BrightID/BrightID-Node/pull/176#discussion_r550916108
    author: adamstallard
    at: 2021-01-02
supersedes: []
reviewed:
  by: adamstallard
  at: 2026-09-13
---

Single occurrence, kept because it is architectural rather than local and was filed as an issue rather than fixed inline. Verify it still reflects how errors are handled before relying on it.
