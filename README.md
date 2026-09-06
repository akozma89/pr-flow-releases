![PR Flow Logo](https://prflow.app/favicon.ico?v=2)

# PR Flow
**The local-first code review inbox for developers.**

[Website](https://prflow.app) • [Download](https://github.com/akozma89/pr-flow-releases/releases) • [Roadmap](ROADMAP.md) • [Report a Bug](https://github.com/akozma89/pr-flow-releases/issues/new?template=bug_report.md) • [Request a Feature](https://github.com/akozma89/pr-flow-releases/issues/new?template=feature_request.md)

---

## 📌 About this Repository

Welcome to the public releases repository for **PR Flow**.

PR Flow is a commercial desktop application for macOS, Windows, and Linux. The source code is not hosted here. This repository serves three purposes:

1. **Releases:** Hosting official signed binaries and release notes.
2. **Roadmap & Issue Tracking:** Sharing our public roadmap and collecting bug reports and feature requests.
3. **Community:** Discussing code review workflows and sharing feedback on [Discussions](https://github.com/akozma89/pr-flow-releases/discussions).

## 🚀 Download & Install

Download the latest version on the **[Releases page](https://github.com/akozma89/pr-flow-releases/releases/latest)**:

- **macOS:** `.dmg` (Apple Silicon & Intel)
- **Windows:** `.exe` installer
- **Linux:** `.AppImage`

*PR Flow comes with a 14-day free trial. No credit card or account creation required.*

## ⚡ What is PR Flow?

PR Flow organizes your incoming and outgoing code reviews into an explainable queue across multiple providers:

- **Unified git host support:** First-class support for **GitHub**, **GitLab**, **Azure DevOps**, and **Gerrit**.
- **Triage by real effort:** Filter PRs by actual change footprint so you can clear quick single-file checks between tasks and schedule complex reviews when you have uninterrupted focus time.
- **Inspect re-review deltas:** View only the new commits and modified hunks on re-reviews instead of re-reading diffs you already approved.
- **Filter bot chatter:** Isolate human reviewer feedback from automated CI bots and linter comments.
- **Explainable queue state:** One-line status summaries clarify whether a PR is blocked by CI, waiting on your sign-off, or awaiting an author's response.

## 🔒 Privacy & Local-First Architecture

PR Flow is built for engineers working in security-conscious codebases:

- **Zero code ingestion:** Source code, diffs, and pull request metadata never touch PR Flow servers.
- **Ambient CLI authentication:** Integrations leverage your existing local CLI tools and sessions (`gh`, `glab`, or `az`). PR Flow never requests or stores master credentials.
- **Local AI options:** Summaries and review triage can run against local LLMs (via Ollama) or your personal API keys. No code is transmitted to third parties or used for model training.
- **No surveillance:** We don't track typing velocity, PR turnaround metrics, or generate management reports.

Review our **[Security Policy](SECURITY.md)** to report any security concerns privately via GitHub Private Vulnerability Reporting.

## 🐞 Bug Reports & Feature Requests

Have a feature request or ran into a glitch?
- **[Report a Bug](https://github.com/akozma89/pr-flow-releases/issues/new?template=bug_report.md)**
- **[Request a Feature](https://github.com/akozma89/pr-flow-releases/issues/new?template=feature_request.md)**
- Review the [Roadmap](ROADMAP.md) to see what is currently in progress.

## ⚖️ License & Legal

**Copyright (c) 2026 Arpad Kozma. All rights reserved.**

PR Flow is a commercial, proprietary product. Binaries provided in this repository are governed by our **[LICENSE](LICENSE)**.

For questions, licensing details, or enterprise inquiries, visit [prflow.app](https://prflow.app).
