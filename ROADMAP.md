# PR Flow Roadmap

Welcome to the PR Flow public roadmap. This document outlines what we are actively building, what is queued next, and longer-term research directions.

> **Note:** This is a living document shaped by user discussions and defect reports. We do not publish artificial calendar deadlines; work moves based on technical validation and community feedback.

**Current state:** PR Flow is shipping across macOS, Windows, and Linux (see [Releases](https://github.com/akozma89/pr-flow-releases/releases)). Because code review sits directly on the team critical path, **Now** contains actively coded features and bug fixes. Exploratory ideas stay in **Later** until their workflows are validated.

## 🚀 Now (In Progress)

_Actively in development for upcoming minor releases._

- **Re-review delta inspector**: when an author pushes updates after your initial pass, inspect only the commits and diff hunks added since your last review stamp instead of re-reading the full change.
- **Review effort triage**: categorize incoming PRs by actual review size (quick single-file adjustments vs multi-file architectural changes) to help knock out small reviews between focus blocks.
- **Explainable queue ordering**: a clear, single-line explanation in the UI showing why each PR is placed where it is in your review queue (e.g. unblocked CI, waiting on your approval, or author replied to your thread).
- **Commit-stamped comment findings**: ensure inline review remarks stay anchored to exact historical commit hashes, even when authors rebase or force-push branches.

## 📅 Next (Upcoming)

_Scoped and prioritized. Order adjusts based on user feedback._

- **Stateful review snoozing**: silence a PR until a specific trigger occurs—such as new commits pushed, CI passing, or an assigned co-reviewer submitting their comments.
- **Stack Journey (part two)**: contextual navigation across stacked branches, tracking parent branch status and warning when an upstream rebase invalidates downstream pull requests.
- **Local CI autopsy**: pull CI failure logs locally through your existing provider credentials (`gh`, `glab`, `az`) to inspect failed assertions without opening multiple browser tabs.
- **Provider-level tool health**: live diagnostics in Settings showing which local CLIs and tokens are ready and which need updates or re-authentication.

## 🔮 Later (Future Explorations)

_Research directions and experiments. These may evolve significantly or be shelved._

- **Author feedback workbench**: turn review comments into a live checklist that marks items addressed as you push fixes, then reply and resolve in batch.
- **Review context recovery**: assemble git blame and prior PR genealogy on demand to answer why a piece of code exists before touching it.
- **Ask Repository**: path-scoped, read-only chat grounded in an opt-in local checkout to check call sites and blast radius without opening a second editor.
- **Deeper self-hosted parity**: expanding configuration support for enterprise on-premises instances (GitLab Self-Managed, GitHub Enterprise Server, Azure DevOps Server, and self-hosted Gerrit).

## 🧭 Principles that shape this roadmap

We maintain three non-negotiable boundaries:

1. **Your code stays local.** Source code, diffs, and pull request data never touch PR Flow servers. When optional AI features are enabled, prompts route directly from your local machine to your chosen provider or local model (Ollama).
2. **AI remains strictly advisory.** PR Flow drafts summaries, highlights risk, and tracks threads. It will never auto-submit comments, approve pull requests, or merge code autonomously. You retain final sign-off on every action.
3. **Zero bossware.** PR Flow is built for the engineer doing the work, not for management oversight. We do not build team leaderboards, speed rankings, or surveillance metrics.

---

## 📦 Already shipped

Everything that has landed is in the [release notes](https://github.com/akozma89/pr-flow-releases/releases), with the full changelog for each version — that is the record, and it is generated from the releases themselves rather than restated here.

---

## 💡 Have an idea?

Feedback directly guides what lands in **Now** and **Next**.
- Report bugs or propose ideas on [GitHub Issues](https://github.com/akozma89/pr-flow-releases/issues).
- Discuss workflows with other users on [GitHub Discussions](https://github.com/akozma89/pr-flow-releases/discussions).
