# PR Flow Roadmap

Welcome to the PR Flow public roadmap. This document outlines what we are actively building, what is queued next, and longer-term research directions.

> **Note:** This is a living document shaped by user discussions and defect reports. We do not publish artificial calendar deadlines; work moves based on technical validation and community feedback.

**Current state:** PR Flow is shipping across macOS, Windows, and Linux (see [Releases](https://github.com/akozma89/pr-flow-releases/releases)). Because code review sits directly on the team critical path, **Now** contains actively coded features and bug fixes. Exploratory ideas stay in **Later** until their workflows are validated.

## 🚀 Now (In Progress)

_Actively in development for upcoming minor releases._

- **Every AI judgement names its commit**: risk, complexity, findings and change stories are each made against one revision of the code, and the branch moves on without them. The queue and the board started saying so in v1.18.0, alongside the pull request details; the menu-bar glance, the daily digest and notifications are what remains — in the same words on every surface, with re-evaluation offered wherever the marker appears. The same rule then extends to other people's work: *"approved at `abc1234`, 3 commits have landed since"*, read from your own provider, with no review state shared or synced between machines.
- **Stack Journey (part two)**: contextual navigation across stacked branches, tracking parent branch status and warning when an upstream rebase invalidates downstream pull requests.

## 📅 Next (Upcoming)

_Scoped and prioritized. Order adjusts based on user feedback._

- **Stateful review snoozing**: silence a PR until a specific trigger occurs—such as new commits pushed, CI passing, or an assigned co-reviewer submitting their comments.
- **Local CI autopsy**: pull CI failure logs locally through your existing provider credentials (`gh`, `glab`, `az`) to inspect failed assertions without opening multiple browser tabs.
- **Provider-level tool health**: live diagnostics in Settings showing which local CLIs and tokens are ready and which need updates or re-authentication.
- **Add reviewers and mark ready for review**: when PR Flow shows that your pull request needs reviewers, request them from the same place — with the provider's own reviewer and group model — and move a draft to ready for review (or back) without opening the provider.

## 🔮 Later (Future Explorations)

_Research directions and experiments. These may evolve significantly or be shelved._

- **Author feedback workbench**: turn review comments into a live checklist that marks items addressed as you push fixes, then reply and resolve in batch.
- **Review context recovery**: assemble git blame and prior PR genealogy on demand to answer why a piece of code exists before touching it.
- **Ask Repository**: path-scoped, read-only chat grounded in an opt-in local checkout to check call sites and blast radius without opening a second editor.
- **Deeper self-hosted parity**: GitLab Self-Managed and self-hosted Gerrit are supported today; extending that configuration support to GitHub Enterprise Server and Azure DevOps Server.
- **Merge when it's ready, on your say-so**: arm your provider's own auto-merge (GitHub auto-merge, GitLab's merge when the pipeline succeeds, Azure DevOps auto-complete) and join GitLab merge trains — armed by your click, carried out by your provider, cancellable from PR Flow.
- **Landing a stack**: merge a stack of pull requests bottom-up in order, where the provider supports it, with each layer still confirmed against its own state.
- **After the merge**: revert a merged pull request, or delete its branch later, from the same place.

## 🧭 Principles that shape this roadmap

We maintain three non-negotiable boundaries:

1. **Your code stays local.** Source code, diffs, and pull request data never touch PR Flow servers. When optional AI features are enabled, prompts route directly from your local machine to your chosen provider or local model (Ollama).
2. **AI remains strictly advisory.** PR Flow drafts summaries, highlights risk, and tracks threads. It will never auto-submit comments, approve pull requests, or merge code autonomously. You retain final sign-off on every action.
3. **Zero bossware.** PR Flow is built for the engineer doing the work, not for management oversight. We do not build team leaderboards, speed rankings, or surveillance metrics.

---

## 📦 Already shipped

Everything that has landed is in the [release notes](https://github.com/akozma89/pr-flow-releases/releases), with the full changelog for each version — that is the record, and it is generated from the releases themselves rather than restated here.

Most recently, **v1.21.0** closed **Immediate CI actions** and added merge, close and update-branch actions: re-run or cancel CI from the pull request (with a one-click re-run on your own failing GitHub and GitLab pull requests), and merge, close, reopen or update a branch on your own pull requests — each confirmed against your provider first, and merged only when you click. Before that, **v1.19.0** taught PR Flow which checks actually gate a merge, and **v1.20.0** added an optional feedback survey at the end of the trial.

---

## 💡 Have an idea?

Feedback directly guides what lands in **Now** and **Next**.
- Report bugs or propose ideas on [GitHub Issues](https://github.com/akozma89/pr-flow-releases/issues).
- Discuss workflows with other users on [GitHub Discussions](https://github.com/akozma89/pr-flow-releases/discussions).
