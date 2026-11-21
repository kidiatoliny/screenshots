# Unified Dev 1.3

Planned: LI 30/11 08:30, X 30/11 10:00, Bluesky 30/11 10:00 (Europe/Luxembourg)

## Text: X

Unified Dev 1.3 is out. Six agents now: Claude Code, Codex, Grok, the Antigravity CLI, Cursor and OpenCode. Bitbucket Cloud works beside GitHub: pull requests, Pipelines logs, merge and checkout. And Claude Code can drive Chrome if you switch it on.

## Text: Bluesky

Unified Dev 1.3 is out. Six agents: Claude Code, Codex, Grok, the Antigravity CLI, Cursor and OpenCode. Bitbucket Cloud works beside GitHub: pull requests, Pipelines logs, merge and checkout.

#Swift #macOS

## Text: LinkedIn

Unified Dev 1.3 is out.

Unified Dev is the macOS app I'm building to run coding agents in parallel, each in its own git worktree. This release is about meeting people where they already work.

Six agents: Claude Code, Codex, Grok, the Antigravity CLI, Cursor and OpenCode. Grok and Antigravity both speak the Agent Client Protocol, so they share one client and differ only in a small dialect. A profile can sign in to its own Claude Code, Codex and Grok accounts.

Bitbucket Cloud beside GitHub: the app reads the host from the remote, then shows pull requests and build statuses, merges, checks out, and sends a failed Pipelines log to the agent, the way it already did with GitHub Actions. Each profile keeps its own Bitbucket sign-in, and git gets the token through a credential helper, never in a URL or the environment.

And a switch, off by default, that lets Claude Code agents use Claude in Chrome.

Which agent or host should come next?

#Swift #macOS #AIAgents

## Screenshots

- `01-agents.png`
- `02-git-hosting.png`

---

# AMA: Unified Dev

Planned: X 06/12 18:00, Bluesky 06/12 18:00 (Europe/Luxembourg)

## Text: X

Ask me anything about Unified Dev, the macOS app I'm building to run coding agents in parallel: six agents, git worktrees, profiles, Bitbucket next to GitHub, SwiftUI on the Mac. I'll answer in the replies.

## Text: Bluesky

Ask me anything about Unified Dev, the macOS app I'm building to run coding agents in parallel: six agents, git worktrees, profiles, Bitbucket next to GitHub, SwiftUI on the Mac. I'll answer in the replies.

#Swift #macOS

## Screenshots

- `unified-dev/workspaces/01-parallel-agents.png`
