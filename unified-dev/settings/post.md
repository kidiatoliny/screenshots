# Unified Dev: don't ask the CLI who it is

## Text: X

Lesson from Unified Dev: to know which account an agent CLI is signed in to, I stopped asking the CLI. In my tests, claude auth status preferred the environment over the config directory, and said loggedIn for a forged token. Now the app reads the account's own directory.

## Text: Bluesky

Lesson from Unified Dev: to know which account an agent CLI is signed in to, I stopped asking the CLI. In my tests, claude auth status preferred the environment over the config directory, and said loggedIn for a forged token. Now the app reads the account's own directory.

#Swift #macOS

## Screenshots

- `01-agents.png`: the Agents settings screen, Claude Code connected to the demo account, with the GitHub account below.

---

# Unified Dev: run commands without asking

Planned: 2026-11-19 08:30 Luxembourg (LinkedIn)

## Text: LinkedIn

Unified Dev has a new per-project switch for the orchestrator: Run commands without asking. It's off by default, and off changes nothing.

On, a shell command that would have stopped for your approval is read in full first: compound commands, substitutions, here documents, and the programs known to run other programs. The answer is one of three: refused, left to you, or allowed once. If any part is refused, the whole command is.

What it doesn't change: file edits, driving a terminal and other MCP servers' tools behave as before, and a command it can't read still comes to you.

The part I cared about most: no agent can turn it on. It lives in the app's own settings, isn't a bridge tool and isn't read from any file in the worktree. A follow-up test calls every bridge tool, in every role, with values naming the switch, and checks it never moves.

Would you let an agent run commands without asking?

#Swift #macOS #AI

## Screenshots

- `02-run-without-asking.png`

---

# Unified Dev: run commands without asking

Planned: 2026-11-19 18:00 Luxembourg (X + Bluesky)

## Text: X

Unified Dev has a new per-project switch: Run commands without asking, for the orchestrator. Off by default. On, each command is read in full, pipes, substitutions and here documents included, then refused, left to you, or allowed once.

## Text: Bluesky

Unified Dev has a new per-project switch: Run commands without asking, for the orchestrator. Off by default. On, each command is read in full, pipes, substitutions and here documents included, then refused, left to you, or allowed once.

#Swift #macOS

## Screenshots

- `02-run-without-asking.png`
