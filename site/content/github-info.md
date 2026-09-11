# GitHub Info

## Mona's editorial angle

Mona's website focuses on practical GitHub guidance backed by official references from:

- docs.github.com
- github.blog
- github.blog/changelog

## Current homepage themes

- GitHub collaboration basics: repositories, branches, pull requests, and merges.
- GitHub Copilot as an AI coding assistant across the IDE, CLI, and GitHub.
- GitHub Actions as the automation layer behind repository workflows.
- Recent GitHub Blog and Changelog stories worth watching.

## Recent updates worth watching

### From the GitHub Blog

- **Copilot app for beginners series** — A running set of short guides (diff/terminal/browser views, running several agents at once, managing your work, triaging Dependabot PRs) that walk new users through the GitHub Copilot app step by step. Good practical starting point for readers new to Copilot.
- **How canvases make agentic workflows visible, steerable, and cost-efficient** — Explains how "canvases" give developers a visual way to watch and steer AI agents while they work, instead of treating them as a black box.
- **Decoding the new AI lingo: loops, harnesses, squads, hill climbing** — A plain-language glossary for the fast-moving vocabulary around agentic coding, useful for readers who feel lost in AI jargon.

### From the GitHub Changelog

- **Copilot code review can now approve pull requests** (Sept 1) — Copilot's automated review can now formally approve a PR, not just leave comments, tightening the review-to-merge loop.
- **GitHub CLI media in issues, pull requests, and comments** (Sept 1) — The `gh` CLI can attach images/video to issues and PRs directly from the terminal.
- **Content exclusions generally available in Copilot app and CLI** (Sept 2) — Teams can now exclude specific files/paths from Copilot's context across the app and CLI, useful for keeping secrets or generated code out of suggestions.
- **Block pull requests with exposed secrets from merging** (Sept 9) — A new guardrail stops PRs with detected secrets from merging until resolved, strengthening secret-scanning enforcement.
- **Refreshed repository pull requests page in public preview** (Sept 10) — A redesigned PR list view, worth a mention as a UI change readers will notice soon.

### From Awesome Copilot workflows

- **Daily Issues Report** — A scheduled agentic workflow that posts a daily summary of new, closed, and stale issues as a GitHub issue; a simple starter example for teams automating triage.
- **OSPO Organization Health Report** — A weekly workflow that surfaces stale issues/PRs, merge-time trends, and contributor leaderboards for an entire GitHub organization.
- **Weekly Comment Sync** — Finds stale code comments or README snippets and opens a draft pull request with text-only fixes, a good example of safe, low-risk automation.

*Sources: GitHub Blog (github.blog), GitHub Changelog (github.blog/changelog), and Awesome Copilot workflows (github.com/github/awesome-copilot).*
