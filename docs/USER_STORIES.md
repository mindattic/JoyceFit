---
codex: 1
project: JoyceFit
code: JF
layer: stories
status: living
updated: 2026-10-12
---
<!-- GENERATED from MindAttic.Tickets/data/Tickets.db by `tickets db render`. Do not edit: this file is rewritten from the database; change stories and tickets with the tickets CLI. -->

# JoyceFit — User Stories
> ✅ done (shipped & tested) · 🟡 partial · ⬜ planned. Every ✅ cites the test.

## Priority backlog
_Nothing recorded yet._

## Tickets
> Permanent log of every change and fix — this repo's ticket system. Rows are append-only: never
> delete or reword one; only move its Status (open → closed / wont-do) and fill in Ref. Status is
> a word, not a glyph, so tickets don't count toward the story index. Keep this section last.

| ID | Date | Type | Status | Summary | Ref |
|---|---|---|---|---|---|
| JF-T1 | 2026-10-12 | docs | closed | Start the permanent ticket log in USER_STORIES.md | — |
| JF-T2 | 2026-10-15 | chore | closed | Remove duplicate command copies (/quickload, /quicksave) now centralized at the user level (~/.claude/commands) | M.FLOW-T14 |
| JF-T3 | 2026-10-16 | chore | closed | install.ps1 adds this repo's 9 .prose/commands stubs for the shared global commands, so any LLM client finds them | mindattic-agent-standard/install.ps1 run 2026-10-16 |
| JF-T4 | 2026-10-16 | chore | closed | Bug hunt: run an exhaustive /bughunt over the whole repo and fix every real bug found (each fix under its own fix ticket), then hunt again; close this only when a full pass finds nothing | 2db79d7 |
| JF-T5 | 2026-10-16 | chore | open | Run the full unit test suite and fix every failure (each under its own fix ticket) until it passes; put the passing run in --ref. No test project: close this wont-do saying so | user request 2026-10-16: approved repo sweep |
| JF-T6 | 2026-10-16 | chore | open | Clean up code and docs: remove dead code, stale comments and outdated or duplicated docs, and simplify where behaviour doesn't change (/simplify); tests stay green | user request 2026-10-16: approved repo sweep |
| JF-T7 | 2026-10-16 | docs | open | Bring README.md up to date with the code as it is now (what it is, setup, usage, commands, current state), following codex-standard/README-STYLE.md; README.htm regenerated if the repo has one | user request 2026-10-16: approved repo sweep |
| JF-T8 | 2026-10-16 | docs | closed | Update USER_STORIES.md | — |
| JF-T9 | 2026-10-19 | chore | open | Convert tracked source files to LF line endings via .gitattributes, per HOUSE-LAW-13 (low priority) | — |
| JF-T10 | 2026-10-20 | docs | open | Publish JoyceFit docs to GitHub Pages via the shared Toolkit DocFX pipeline: run adopt-docs-site.ps1 (README.md as home page, docs/*.md as articles, API reference only where the code builds in CI), enable Pages with build_type=workflow, set the repo homepage URL, retire tools/build-readme.ps1 and README.htm, confirm the docs Actions run is green and https://mindattic.github.io/JoyceFit/ returns 200. Depends on MAT-T8. This is a static site: the Pages site is docs only and must not replace or clash with its real hosting (check MindAttic.Deploy first). | — |
| JF-T11 | 2026-10-21 | fix | closed | deck.htm: slides are width:100vw inside a scrolling .deck, so on Windows/classic scrollbars the deck overflows sideways, shows a horizontal scrollbar and snapped slides no longer fit the viewport | eb541ea |
| JF-T12 | 2026-10-21 | fix | closed | deck.htm: screenshot slides (card, flyer; website on phones) are taller than 100vh at 1280x720/1366x768, so overflow:hidden crops the kicker and heading off the top and the image off the bottom | ec0bf63 |
| JF-T13 | 2026-10-21 | fix | closed | frontpage.htm: the phone media query's .ctarow{gap:16px} sits before the base .ctarow rule, so the later gap:22px always wins and the mobile gap never applies | 74b6066 |
| JF-T14 | 2026-10-21 | fix | closed | frontpage.htm: the nav brand link targets header#top, which sits below the sticky nav, so clicking it scrolls the page 65px down and the nav covers the hero eyebrow on phones | 2db79d7 |
| JF-T15 | 2026-10-21 | fix | open | deck.htm: on very small phones (320x568) the fixed 100vh slides with overflow:hidden crop text on slides 6, 8, 11, 12, 13 and 15; fixing it means letting slides grow past one screen (min-height + snap rework), a layout decision left for review | — |
| JF-T16 | 2026-10-21 | docs | closed | Update USER_STORIES.md | — |
