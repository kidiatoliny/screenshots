# Unified Dev: one git worktree per agent

## Text: X, Bluesky

Unified Dev runs every coding agent in its own git worktree. Here one agent is writing a retry with jitter for HTTP 429 on its own branch, while the other workspaces sit in the sidebar with their own changes. No agent ever touches another one's files.

---

# Unified Dev: nothing is written before Create

## Text: X

In Unified Dev, a new workspace doesn't exist until you press Create. Picking the project and the base branch writes nothing. Create is the moment it cuts a branch from origin/main into its own git worktree. Close the sheet before that and there's nothing to clean up.

## Text: Bluesky

In Unified Dev, a new workspace doesn't exist until you press Create. Picking the project and the base branch writes nothing. Create is the moment it cuts a branch from origin/main into its own git worktree. Close the sheet before that and there's nothing to clean up.

#git #SwiftUI #macOS

## Text: LinkedIn

A rule in Unified Dev that took me a while to get right: nothing touches the disk until you say so.

When you start a new workspace you pick the project, the base branch, and write what the agent should do. None of that creates anything. Only Create does: it cuts a new branch from origin/main into a git worktree of its own. Close the sheet before that and there's nothing to clean up.

The Home screen is the other half. Every workspace from every project sits in one list, with its branch, how much it changed and how long ago it was active. Archived ones stay there, greyed out, next to the branch they left.

When a tool creates branches and folders for you, where do you want it to stop and ask?

#Swift #macOS #git

---

# Unified Dev: starting points

Planned: Bluesky 10/12 18:00, X 10/12 18:00 (Europe/Luxembourg)

## Text: X

A new workspace in Unified Dev used to start from an empty composer. Now it suggests up to four starting points: pull requests waiting on you, issues assigned to you and branches you touched lately. Click an issue and it cuts a branch and adds the issue to the prompt.

## Text: Bluesky

A new workspace in Unified Dev now suggests up to four starting points: pull requests waiting on you, issues assigned to you and branches you touched lately. Click an issue and it cuts a branch and adds it to the prompt.

#Swift #macOS

## Text: LinkedIn

An empty text box is a bad place to start work.

In Unified Dev, my macOS app for running coding agents in parallel, a new workspace opened on an empty composer. Most of the time I already knew what I wanted: the pull request someone asked me to review, the issue assigned to me, the branch I left yesterday.

So the space under the composer now lists up to four starting points the app finds on its own: pull requests waiting on you, issues assigned to you and local branches touched in the last two weeks, one of each kind before a second of any. Click a pull request or a branch and the workspace starts from it. Click an issue and it cuts a new branch from the default one and puts the issue in the prompt.

The reading is reused for two minutes, so opening the sheet again doesn't ask GitHub twice.

#Swift #macOS #DevTools

## Screenshots

- `04-starting-points.png`
