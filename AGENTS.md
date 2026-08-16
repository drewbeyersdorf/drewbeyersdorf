# AGENTS.md — drewbeyersdorf

**Read this first.** Operating contract for every agent (Cursor, Claude Code, Codex, Kimi, Grok) working in `drewbeyersdorf/drewbeyersdorf`.

Fleet-wide documentation rules: [methodology-agent-os/docs/SAFE_DOCUMENTATION.md](https://github.com/drewbeyersdorf/methodology-agent-os/blob/master/docs/SAFE_DOCUMENTATION.md)

---

## What this repo is

Private repository `drewbeyersdorf/drewbeyersdorf`.

Recent activity: Update character-sheet.svg

---

## Before you change anything

1. Read **`docs/WORK_TO_DATE.md`** for current status and prior milestones.
2. Read **`README.md`** if it exists.
3. Work on a **feature branch** off `main`; never commit directly to the default branch unless this repo's policy says otherwise.
4. Run the **publication gate** from SAFE_DOCUMENTATION.md §4 before every push.
5. **Producer ≠ auditor** — the agent that wrote a change does not mark it verified.

---

## Hard boundaries

- **Only Drew-owned repos.** Never clone or modify third-party repositories.
- **No secrets in git** — no API keys, tokens, `.env` values, webhook URLs with secrets, or connection strings. Use env var *names* only.
- **No raw evidence** — do not commit messages, transcripts, screenshots, recordings, or absolute paths to private evidence bundles unless this repo explicitly exists for that purpose.
- **No outbound sends** — no Slack posts, emails, or webhooks unless repo-specific rules and env gates explicitly allow it. Default: stage drafts only.
- **No merges without human approval** — open a PR; Drew (or named delegate) merges.

---

## Privacy tier for this repo

| Default tier | Notes |
|--------------|-------|
| **T2 — Code-private** | Private repo; still run publication gate before every push. |

When unsure, assume one tier more private. See SAFE_DOCUMENTATION.md §2.

---

## Local rules

<!-- Add repo-specific rules below. Examples: stack, test commands, deploy targets, holds. -->

- Follow conventional commits: `type(scope): imperative summary`.
- Update `docs/WORK_TO_DATE.md` when shipping a milestone.

---

## Work history

All completed work is recorded in **`docs/WORK_TO_DATE.md`**. Update it in the same commit when you ship a milestone or change repo status.

---

## Fleet links

| Resource | Location |
|----------|----------|
| Safe documentation standard | [methodology-agent-os/docs/SAFE_DOCUMENTATION.md](https://github.com/drewbeyersdorf/methodology-agent-os/blob/master/docs/SAFE_DOCUMENTATION.md) |
| Agent OS canon | [methodology-agent-os](https://github.com/drewbeyersdorf/methodology-agent-os) |
| PR triage (yej-io only) | [yej-kimi](https://github.com/drewbeyersdorf/yej-kimi) |

---

*Bootstrapped from fleet template 2026-08-16. Customize § Local rules and § What this repo is before treating as ratified.*
