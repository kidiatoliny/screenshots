# Unified Dev: parallel agents and the Archive safety report

Project: `unified-dev` · Status: scheduled

## Schedule

| Channel | When (Luxembourg) | Buffer post | Link |
|---|---|---|---|
| LinkedIn | Tue 20 Oct, 08:30 | `6aca09ead9cab260a7bc5d6b` | |

## Images

- `overview/01-main-window.png` (original), `overview/01-main-window.jpg` (used in the post)
- `agent/01-turn-running.png` (original), `agent/01-turn-running.jpg` (used in the post)
- `archive/01-safety-report.png` (original), `archive/01-safety-report.jpg` (used in the post)

## Text: LinkedIn

I've been building Unified Dev, a native macOS app for running coding agents in parallel. Each agent gets its own git worktree, so several of them can work on the same repo without stepping on each other.

It's built with SwiftUI. One window: projects and workspaces on the left, the agent transcript in the middle, a terminal, and an inspector with the diff. It works with Claude Code and Codex.

Because a workspace is a real worktree on disk, a lot of the work went into not destroying one. The first version of Archive ran git worktree remove --force and git branch -D with no checks. Uncommitted work, gone. Now it builds a safety report first, refuses by default, and tells you exactly what would be lost before you confirm.

If you run more than one coding agent at a time, how do you keep them from stepping on each other?
