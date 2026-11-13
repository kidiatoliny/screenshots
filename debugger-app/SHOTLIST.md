# Akira Debugger: shot list

Source: https://github.com/akira-foundation/debugger-app (Tauri: Rust + React), latest release v0.5.0
How to shoot: the app window receiving Ray calls from a demo Laravel app; demo data only, no real emails, tokens or customer data (solid boxes if anything real shows)

Screens to capture and their status. Window-only `screencapture` on Retina, never cropped or edited. The post that uses a feature's shots goes in that feature's folder as `post.md` (written by Claude).

- [x] `overview/01-log-list.png`: the main window with a mix of entries from a demo Laravel app: a dump, an executed query, an Eloquent model, a mailable, a table, an application log and an exception, with labels, and the dump expanded.
- [x] `overview/02-exception.png`: an exception entry expanded as a tree: class, frames, file and line.
- [x] `overview/03-filters.png`: the log type filter in the header showing only queries, with the search field open and a search typed.
- [x] `overview/04-query.png`: an executed query expanded: connection, time and the formatted SQL.
- [x] `overview/05-mailable.png`: a mailable expanded: subject and body.
- [x] `overview/06-eloquent-model.png`: an Eloquent model expanded: class and attributes.
- [x] `overview/07-ai-explain.png`: the "Explain with Claude" drawer open on an exception: what happened, root cause, fix and notes, powered by the Claude Code CLI.
- [x] `overview/08-settings.png`: Settings, Preferences tab: preferred editor, log border style and log display limits.
