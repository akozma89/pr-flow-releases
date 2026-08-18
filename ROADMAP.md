# PR Flow Roadmap

Welcome to the PR Flow roadmap! This document gives a high-level view of what is
being worked on now, what is planned next, and the longer-term directions we are
exploring.

> **Note:** This roadmap is a living document and is subject to change based on
> user feedback and project priorities. Nothing here is a dated commitment.

**Current phase:** PR Flow is a stable, shipping product (see
[Releases](https://github.com/akozma89/pr-flow-releases/releases)). The
near-term focus is getting it in front of more developers and keeping it solid,
so **Now** is deliberately small and made of things that can land reliably: real
defects and sharp, contained improvements. Bigger bets live in **Later** as
directions, not promises.

## 🚀 Now (In Progress)

_Small, committed work for the next upcoming releases._

- **"Draft with AI" failures say what happened**: when a summary can't be
  drafted, name the reason instead of failing quietly.
- **A fully keyboard-accessible Finish-review sheet**: proper dialog semantics,
  focus management, and reachable controls, including for screen readers.
- **Find any setting by typing its name**: search in Settings that jumps
  straight to the setting you mean.
- **Every tool error tells you the fix**: when a required CLI is missing or
  signed out, say so in plain language and offer the next action.

## 📅 Next (Upcoming)

_Planned and scoped. Order may shift; timing depends on capacity._

- **Know why a PR is next**: a short, plain-language reason for the queue order.
- **Waiting on whom, and for how long**: make a stalled review visible instead
  of quietly ageing.
- **One honest home for local tools**: see what PR Flow can actually do on this
  machine, and what's missing before you connect.
- **Smarter snoozing**: silence a PR until the thing you're waiting for actually
  happens.
- **Stack Journey, part two**: guidance through a stacked review session, not
  just navigation.

## 🔮 Later (Future Explorations)

_Directions we intend to explore. Not scoped, not scheduled, and some will
change or be dropped outright._

- **Review context beyond the diff**
- **Closing the loop from review comments to done**
- **Personal insight, kept personal**
- **Team workflows without surveillance**
- **Deeper parity across providers**

## 🧭 Principles that shape this roadmap

Some things are deliberately _not_ on it, now or later:

- **Your code stays yours.** Source code and pull-request data never pass
  through PR Flow's servers. When AI is enabled, content goes from your machine
  straight to the provider you chose — pick a local one and it never leaves the
  device.
- **AI is advisory.** It can read, summarize, and suggest. It never posts,
  approves, or merges on your behalf; nothing leaves the app until you press
  submit.
- **No bossware.** Personal metrics stay personal. PR Flow will not build
  manager dashboards that rank individuals.

---

## 💡 Have an idea?

We'd love to hear from you! If you have a feature request or an idea to improve
PR Flow, please check our
[Issues](https://github.com/akozma89/pr-flow-releases/issues) to see if it has
already been proposed, or start a new
[Discussion](https://github.com/akozma89/pr-flow-releases/discussions).

This roadmap is founder-driven today. User requests carry more weight than
anything on this page — if something here is in your way, or something missing
matters more, say so and it moves.

## 📦 Recently shipped

A few highlights from recent releases — see the
[Releases](https://github.com/akozma89/pr-flow-releases/releases) page for the
full history.
