# Unified Dev: one git worktree per agent

## Text: X, Bluesky

Unified Dev runs every coding agent in its own git worktree. Here one agent is writing a retry with jitter for HTTP 429 on its own branch, while the other workspaces sit in the sidebar with their own changes. No agent ever touches another one's files.
