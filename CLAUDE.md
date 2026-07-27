# CLAUDE.md

Guidance for Claude Code working in the `ketqat/.github` repository.

This repository has no `AGENTS.md`. The organization-wide conventions in the `AGENTS.md` files of `ketqat-sdk`, `ketqat-web`, and `ketqat-planning` still apply to how work is proposed and reviewed here.

## What this repository is

`ketqat/.github` owns the **public** organization profile and the shared community health files that GitHub applies as defaults across the organization:

- `profile/README.md` -- the public organization landing page
- `ISSUE_TEMPLATE/` -- shared issue forms (bug report, feature request, documentation, research task) and `config.yml`
- `PULL_REQUEST_TEMPLATE.md` -- default PR template
- `CODE_OF_CONDUCT.md`, `CONTRIBUTING.md`, `GOVERNANCE.md`, `SECURITY.md`, `SUPPORT.md`, `LICENSE`

## Blast radius

Files here are inherited by every repository in the organization that does not define its own. A change to an issue form or the PR template takes effect immediately, everywhere, without a deploy. `profile/README.md` is the first thing an outside visitor reads.

Treat every change as a public, organization-wide change:

- Verify issue form YAML is valid before merging; a malformed form breaks issue creation across all repositories.
- Keep the PR template's required sections aligned with what the repositories' `AGENTS.md` files ask contributors to report.
- Do not add repository-specific instructions here. They belong in that repository.

## Public-safety rules

This repository is public, and `ketqat-web` and `ketqat-planning` are private.

- Do not copy content from private repositories into this one.
- Do not reference private infrastructure, secret names, deployment topology, database hosts, or internal URLs.
- Do not describe features that do not exist yet as though they ship today.
- Security reporting instructions in `SECURITY.md` must stay accurate; a stale contact path is a real vulnerability.

## Scope statement

`README.md` and `profile/README.md` state the project's scope publicly. Per [ADR 0001](https://github.com/ketqat/ketqat-planning/blob/main/docs/architecture/adr/0001-focus-on-qec-and-algorithms.md), KetQat does not provide QPU access aggregation, marketplaces, billing, hardware-provider status monitoring, or credential storage.

ADR 0004 proposes narrowing that clause to permit hardware characterization snapshots and user-initiated BYOC execution. It is **Proposed, not Accepted**. Do not change the public scope statement here until a maintainer accepts it -- this repository is where the project's scope is stated to the outside world, so it must not lead the decision.

## Commands

There is no build or test step. Before committing:

```bash
git diff --check HEAD
```

Validate any changed issue-form YAML, and check that Markdown links resolve.

## Workflow

- Use a feature branch: `chore/...`, `docs/...`, or `fix/...`. Do not commit to `main`.
- `main` has force-push and deletion blocked; there are no required status checks, so review carries the weight.
- Link PRs to an Issue in the repository the change serves, usually `ketqat-planning`.

## Cautions

- Worktrees of this repository exist outside the primary checkout, including under `~/.codex/worktrees/`. Run `git worktree list` before assuming a branch is free.
