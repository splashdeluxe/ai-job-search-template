# Changelog

All notable changes to this template, newest first. The format follows Keep a Changelog, and versions match the GitHub releases.

## Unreleased

- Sources: regional boards added to `04-sources.md` (Arbeitsagentur, MyCareersFuture, Jobstreet / SEEK with the bare-host note, Welcome to the Jungle, JustJoin.it, Landing.jobs), plus a note that Glints cannot be used as a feed.
- Apply: on Lever, the agent now attempts the submit itself. The owner steps in only when a human-verification check genuinely blocks it.

## v1.0 - 2026-11-02

First public release.

- The full loop as commands: /setup, /scrape, /rank, /apply, /interview, /outcome, /gmail-sync, /upskill, /html-report.
- The integrity rules in `AGENTS.md`: official careers boards only, submit exactly once, never invent a fact or a number.
- The CV standard (`03-cv-standard.md`), the writing check (`05-writing-check.md`) and the dispatcher (`06-dispatcher.md`).
- A fictional worked example (Alex Rivera) under `examples/`, a dashboard spec, and a one-page site under `docs/`.
