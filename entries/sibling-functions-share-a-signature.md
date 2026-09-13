---
id: sibling-functions-share-a-signature
claim: Functions in the same family should take the same leading arguments, so callers
  do not have to remember which one is different.
scope: global
status: provisional
conditions:
  paths:
    - web_services/**/*.js
  prose: When adding a function alongside existing ones that operate on the same entity.
provenance:
  - url: https://github.com/BrightID/BrightID-Node/pull/147#discussion_r529254912
    author: abramsymons
    at: 2020-11-24
  - url: https://github.com/BrightID/BrightID-Node/pull/353#discussion_r1468855048
    author: abramsymons
    at: 2024-01-28
supersedes: []
---

The 2024 instance opens with "as asked before", which is the tell: the same correction had already been made and had not stuck.
