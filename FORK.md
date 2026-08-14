# Fork Notes

This repository is a **personal fork** of the upstream Hermes agent.

## Origin / Upstream

- **Upstream:** `https://github.com/NousResearch/hermes-agent` (remote `upstream`)
- **This fork:** `https://github.com/bhovig/hermes-agent` (remote `origin`)
- The code is originally developed and maintained by Nous Research. Credit and licensing belong to them (see `LICENSE`).

## Purpose of This Fork

A private mirror/working copy used for local development and experimentation. It carries **no product or feature changes** of its own beyond a small set of housekeeping commits (removing oversized committed infographics that violate gitignore policy, and a `package-lock.json` version bump).

## Sync Policy

- The intent is for `main` to track upstream `main`; in practice, this fork is synced from upstream periodically and may lag behind it. This fork is **not** a source of truth for product behavior.
- The canonical, authoritative implementation documentation is owned by upstream and must **not** be rewritten or reformatted here.
- To sync from upstream:
  ```bash
  git fetch upstream
  git checkout main
  git merge upstream/main
  ```
- Do **not** force-push, rewrite history, or alter `origin`/`upstream` remotes.
- Any upstream-owned docs (`README.md`, `CONTRIBUTING.md`, `AGENTS.md`, etc.) are only ever updated by merging upstream changes — never hand-edited with fork-specific content.
