# Orbit: shot list

Source: https://github.com/akira-foundation/orbit (Go + Wails + React)
How to shoot: the app window with demo projects only

Screens to capture and their status. Build or open it from an up-to-date main, demo data only, window-only `screencapture` on Retina, never cropped or edited. The post that uses a feature's shots goes in that feature's folder as `post.md` (written by Claude).

- [x] `overview/01-dashboard.png`: The dashboard with a few demo projects and their <slug>.test domains.
- [x] `overview/02-project-detail.png`: a demo project's detail view with the detected framework, package manager, port and suggested dev command.
- [x] `projects/01-detection.png`: a project detail view showing the detected package manager, framework and suggested dev command.
- [x] `projects/02-add-overwrite.png`: The Add project dialog for a folder whose slug is already taken, showing the "already registered" notice and the Overwrite button.
- [x] `projects/03-after-overwrite.png`: the same project's detail after Overwrite, now pointing at the new folder.
- [ ] `projects/04-overwrite-fails.png`: Add project dialog, Overwrite on a folder whose slug `shop` is taken, while the domain `shop.orbit.test` belongs to another demo project: the dialog shows the overwrite error (fix d6ad774: delete and insert now run in one transaction).
- [ ] `projects/05-owner-kept.png`: right after that failed Overwrite: the dashboard still lists the original `shop` project with its folder, domain and scripts intact (before the fix it was deleted along with its groups, domains, scripts and logs).
