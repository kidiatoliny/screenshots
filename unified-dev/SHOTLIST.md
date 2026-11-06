# Unified Dev: shot list

Screens to capture and their status. Where a shot is used lives in `posts/<post>/post.md`; search for the file name to find it.

- [x] `overview/01-main-window.png`: the whole window with a project open: sidebar with projects and workspaces, a transcript, the terminal and the changed files.
- [x] `git/01-diff-inspector.png`: a real diff an agent just produced, open in the inspector.
- [x] `agent/01-turn-running.png`: an agent mid-turn, with the Stop button visible.
- [x] `workspaces/01-parallel-agents.png`: 3 or 4 workspaces visibly running agents at the same time, with the sidebar as the focus.
- [x] `archive/01-safety-report.png`: the Archive confirmation listing what would be lost.
- [x] `settings/01-agents.png`: the Agents settings screen with the detected CLIs and the account each one is signed in to.
- [x] `workspaces/02-create-sheet.png`: the sheet for creating a new workspace, with the source picker.
- [ ] `agent/02-subagents.png`: RETAKE: a subagent summary line was painted over in the image. Needs a transcript where the agent spawned subagents and every line, subagent output included, is in English.
- [x] `archive/02-archived-list.png`: Home, Archived tab, with an archived workspace and its branch.
- [x] `archive/03-home-all.png`: Home, All tab, every workspace with its project and branch, one of them archived.
- [x] `git/02-branch-and-push.png`: a workspace with its branch bar (branch, pull request status, Create pull request) and the Push button.
- [x] `updates/01-update-alert.png`: Preview opened with `Tools/scenarios/software-update.json`: the update alert with the release notes, the Skip button, and Later as the default button.
- [x] `spend/01-spend-screen.png`: The spend screen in light appearance: the grouped form, columns ranked by cost, a month of bars with day labels.
- [x] `spend/02-by-account.png`: the spend screen with the By account section showing the Claude Code account and the Codex account, each with its own cost.
- [ ] `agent/03-provider-switch.png`: a demo chat that started on Claude Code and continued on Codex, with the divider between the two visible in the transcript and the model menu showing the new provider. NEEDED BY Tue 10/11 16:00
- [ ] `transcript/01-reply-card.png`: a passage of an agent's answer selected, with the reply card open next to it (quote and reply field), and one quote card already held above the composer. Demo project. NEEDED BY Wed 11/11 16:00
- [ ] `transcript/02-selection.png`: an agent's answer with a selection running from a paragraph through a list and into a code block. Demo project. NEEDED BY Fri 13/11 08:00
- [ ] `profiles/01-switcher.png`: the sidebar profile switcher open with two demo profiles (e.g. Unified and Work), each showing its own projects. NEEDED BY Mon 16/11 08:00
- [ ] `composer/01-account-menu.png`: the composer's model menu open with its Account section (demo accounts only, e.g. ada@lovelace.dev) and Change… NEEDED BY Tue 17/11 16:00
- [ ] `canvas/01-editor.png`: a workspace's canvas tab with the floating toolbar, a few shapes, notes and a frame, and one comment pinned on the canvas. Demo project. NEEDED BY Wed 18/11 16:00
- [ ] `settings/02-run-without-asking.png`: a demo project's settings, Workspaces pane, with the Run commands without asking switch for the orchestrator visible (off). NEEDED BY Thu 19/11 08:00
- [ ] `transcript/03-tasks-sheet.png`: the background tasks list with Running and Finished sections and the Clear button, and a finished command's sheet open with status, type, duration, command and output. Demo project. NEEDED BY Sat 21/11 08:00
- [ ] `workspaces/03-orchestrator-sidebar.png`: a demo project in the sidebar with its orchestrator as the first row (accent connected-points glyph) and the workspaces it started indented under it (68a72b2).
- [ ] `agent/04-orchestrator-read-list.png`: an orchestrator workspace's transcript where a listed read (e.g. `git status`) was answered by Unified Dev on its own, and a command off the closed read list (e.g. `perl -0pi -e ...`) is waiting for the owner's approval. Demo project (8aad2f4, f93bb26).
- [ ] `settings/03-workspaces-tab.png`: Settings, the new Workspaces tab, with "archive a workspace once its pull request merges" on and the archived-workspace limits (age and total size) visible (77c9a0b, 6dd62c8, 024d312).
- [ ] `git/03-image-diff.png`: the diff inspector on a modified PNG, showing the before and after images side by side instead of "Binary content is not shown". Demo project (4dc900f).
- [ ] `updates/02-unsaved-edits.png`: Install and Restart asking first because of unsaved edits, naming the demo files with edits (1412ea0).
- [ ] `transcript/04-run-shell-block.png`: an agent's reply with a bash code block, its run button, and the output shown under the block after it ran. Demo project (c42638d).
- [ ] `quota/01-grok-usage.png`: the menu bar usage panel showing Grok's quota for the current period and its plan, next to the other agents. Demo account only (dd37550).
- [ ] `quota/02-other-account.png`: the menu bar limits panel for an agent whose allowance ran out, offering the agent's other demo account, with the note about what switching costs (f809fd5).
- [ ] `profiles/02-profile-accounts.png`: Profile Settings for a demo profile choosing between its own agent accounts and Unified's, with the profile's default account (#437).
