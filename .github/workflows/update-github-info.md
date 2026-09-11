---
name: update-github-info
description: Reads Mona's notes and the GitHub Blog to keep site/content/github-info.md current, proposing changes via pull request.
on:
  schedule: daily
  workflow_dispatch:
permissions:
  contents: read
tools:
  edit: {}
  web-fetch: {}
network:
  allowed:
    - defaults
    - github.blog
    - github.com
    - awesome-copilot.github.com
safe-outputs:
  create-pull-request:
    title-prefix: "[update-github-info] "
    allowed-files:
      - "site/content/github-info.md"
---

# Update GitHub Info

Keep `site/content/github-info.md` current with the latest GitHub news for Mona's website.

## Steps

1. Read `notes/mona-notes.md` for tone, style, and editorial guidance.
2. Fetch `https://github.blog/latest/` for recent GitHub Blog posts.
3. Fetch `https://github.blog/changelog/` for recent GitHub Changelog entries.
4. Fetch `https://awesome-copilot.github.com/workflows/` for notable Awesome Copilot workflows.
5. Update `site/content/github-info.md` with concise, practical summaries of notable new items, following the guidance in `notes/mona-notes.md`. Mention whether each update came from the GitHub Blog, the GitHub Changelog, or Awesome Copilot workflows.
6. Open a pull request proposing the changes so Mona can review before anything goes live.

If there is nothing new to report since the last update, call `noop` with a short reason instead of opening a pull request.
