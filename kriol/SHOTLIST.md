# Kriol: shot list

Source: https://github.com/kriol-lang/kriol (KriolLang; docs https://docs.kriol.dev). The user contributes; the main author is anaximeno.
How to shoot: terminal window (Ghostty) with the code on top and the output below, plus pages of the docs site; examples live in kriol/examples/*.kriol

Screens to capture and their status. Build or open it from an up-to-date main, demo data only, window-only `screencapture` on Retina, never cropped or edited. The post that uses a feature's shots goes in that feature's folder as `post.md` (written by Claude).

- [x] `hello/01-ola-mundo.png`: The README hello world (`fn ola`, `si` / `sinon`, `mostran`) and its output when run with `kriol`.
- [ ] `errors/01-portuguese-message.png`: a compiler error, which is now written in Portuguese.
- [ ] `molda/01-recursive-field.png`: a molda with a recursive field rejected with a clear error instead of crashing (the user's fix, PR #14).
- [ ] `docs/01-home.png`: the home page of docs.kriol.dev.
- [x] `init-order/01-error.png`: Ghostty window with `tests/fail/fail_global_initializer_names_latest_global.kr` on top (cat) and `kriol` run on it below, showing the Portuguese error that says to declare 'c' before 'a'.
- [ ] `macos/01-check-passes.png`: macOS build (the user's PR #20, then macOS added to the release). Ghostty on the Mac, from an up-to-date main: `head -1 run_tests.sh` showing `#!/usr/bin/env bash` (it was `#!/usr/bin/bash`, which does not exist on macOS), then `cmake --build build/release --target check` ending with the PASS summary on arm64.
- [ ] `macos/02-otool-no-homebrew.png`: Ghostty with `otool -L build/release/kriol` listing only `/usr/lib` and `/System` libraries, no `/opt/homebrew` path (the release checks this so the binary runs on a Mac without Homebrew).
- [ ] `macos/03-hello-arm64.png`: Ghostty with `uname -m` (arm64), `cat examples/hello_world.kriol` and its output "Kualeh Mundu!" when run with the macOS-built `kriol`.
- [ ] `install-checksum/01-mismatch.png`: NEEDED BY Sun 01/11 20:00. Ghostty running install.sh against a truncated or swapped release archive (a local test release is fine), stopping before extracting with the checksum mismatch message. Optional `02-ok.png`: a normal install that prints the verified checksum.
- [ ] `exit-codes/01-sai-256.png`: NEEDED BY Tue 03/11 20:00. Ghostty: `cat` of a .kriol file with `sai(256);` in `inisiu`, then `kriol` rejecting it with the out-of-range error.
- [ ] `ci-pinning/01-actions-sha.png`: NEEDED BY Wed 04/11 20:00. Editor or terminal showing a workflow file with `uses: <action>@<full sha> # vX` lines and the Windows step that compares Get-FileHash with the pinned SHA256.
