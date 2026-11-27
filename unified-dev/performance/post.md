# Unified Dev: doing less in the background (LinkedIn)

Planned: LinkedIn 21/12 08:30 (Europe/Luxembourg)

## Text: LinkedIn

Unified Dev 1.3 does less work when you're not looking, and most of it came from counting.

Unified Dev is my macOS app for running coding agents in parallel, each in its own git worktree. With a dozen workspaces open, the background work adds up, so I wrote a probe that changes five worktrees every two seconds and reports, for one minute, the git processes started, the reloads and the main thread's CPU time. Then I went after the numbers:

Each diff refresh started six git processes. Now four, and a test counts them.
A diff count change reloaded every project. Now only that count updates.
Three terminal loops each ran ps and listed tmux panes every tick. Now they share one reading, and behind another app they wake every ten seconds.
The pull request bar, the checks tab and the notification each asked GitHub for the same pull request. Now they share one read.
Quotas were asked every minute. Now every five minutes while nobody is looking.
Chats you haven't looked at in a while give their rows back and read them again when you open them.

None of these is clever. They were all found by measuring first.

#Swift #macOS #Performance

## Screenshots

- `unified-dev/workspaces/01-parallel-agents.png`
