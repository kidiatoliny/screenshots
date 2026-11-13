# Spectra Desktop: shot list

Source: https://github.com/akira-foundation/spectra-desktop (Go + Wails + React)
How to shoot: the app window signed in to a demo customer; no real customer names, tokens or emails (solid boxes if anything real shows)

Screens to capture and their status. Build or open it from an up-to-date main, demo data only, window-only `screencapture` on Retina, never cropped or edited. The post that uses a feature's shots goes in that feature's folder as `post.md` (written by Claude).

- [x] `overview/01-main-window.png`: the main window with a demo Laravel project open, its routes grouped in the sidebar and `POST /api/books` open, body generated from the FormRequest rules.
- [x] `overview/02-routes-by-resource.png`: a demo NestJS project with its endpoints grouped by resource, method and path visible, and a body generated from the DTO (PR #22).
- [x] `overview/03-send-request.png`: `GET /api/books` sent, with the 200 response, timing, an account and the `local` environment selected.
- [x] `overview/04-add-project.png`: the Add Project dialog after picking a folder: Laravel detected, API routes filter, login and logout routes found, base URL.
- [x] `overview/05-dashboard.png`: the Dashboard overview: response status, latency, slowest and most used endpoints, failures.
- [x] `overview/06-laravel-exception.png`: a 500 response with the Laravel exception panel: class, message, file and line.
- [x] `overview/07-snapshots.png`: Snapshots after a rescan: three routes added and one removed.
- [x] `overview/08-accounts.png`: the Accounts page with three demo identities, one showing a live TOTP code.
- [x] `overview/09-command-palette.png`: the command palette searching endpoints by name.
- [ ] `routes/01-nestjs.png`: NestJS routes detected in a demo project.
- [ ] `license/01-trial-banner.png`: the trial banner.
