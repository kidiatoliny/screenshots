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
