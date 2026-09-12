# Monk's Enhanced Journal — UNOFFICIAL v14 Fork (RotFM1)

> **This is NOT an official release. It is not maintained, endorsed, or supported by IronMonk (ironmonk108), the original author.**
> All credit for Monk's Enhanced Journal itself belongs to IronMonk — see https://github.com/ironmonk108/monks-enhanced-journal, the real project, for the genuine, maintained module, support, Discord, and Patreon/Ko-fi links.

## What this is

A private, personal fork built for one specific need: getting Monk's Enhanced Journal working on Foundry VTT v14 for a personal game (RotFM1), ahead of an official v14-compatible release. It is built on top of three real, open, **unmerged** community pull requests against the official repo:

- [#820 — Foundry VTT v14 compatibility](https://github.com/ironmonk108/monks-enhanced-journal/pull/820)
- [#821 — ~65 bug fixes on top of the v14 migration](https://github.com/ironmonk108/monks-enhanced-journal/pull/821)
- [#823 — Extension API](https://github.com/ironmonk108/monks-enhanced-journal/pull/823)

(all by [bularzik](https://github.com/bularzik), not by the maintainer of this fork)

with one additional fix on top: the "Convert to Enhanced Journal" action, when used on a journal entry with zero pages, was creating the new page with an invalid native `type` field, which Foundry v14 rejects outright. This fork creates that page as a valid `"text"` type instead, matching the pattern the rest of the codebase already uses correctly.

## Why this exists / why it's not just using the official module

As of this fork, the official Monk's Enhanced Journal release only declares verified compatibility through Foundry v13, and the above PRs — while real and in progress — are not yet merged or released. This fork exists only to unblock one personal v14 test install in the meantime.

## Status

- Not tested extensively. Built for one specific sandbox world, not for general use.
- No support is offered here. Use entirely at your own risk.
- Once the official module ships real v14 support, **switch back to the official module** and stop using this fork.

## License

Distributed under the same license as the original project (GPLv3) — see `LICENSE`. This fork's own changes are described in the git history; everything else is IronMonk's original work.
