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
- [x] `install-checksum/01-mismatch.png`: Ghostty running install.sh from main against the v1.16.2-alpha+build1 pre-release with the downloaded archive truncated to 1 MB, stopping at "Verifying..." with the checksum mismatch error.
- [x] `install-checksum/02-ok.png`: the same install.sh against the untouched pre-release: Verifying, Extracting, installed.
- [x] `exit-codes/01-sai-256.png`: Ghostty, kriol built from main: `cat` of tests/fail/fail_sai_code_above_255.kr (`sai(256);` in `inisiu`), `kriol` rejecting it with the out-of-range error, exit status 1.
- [x] `exit-codes/02-computed-code.png`: tests/panic/sai_code_negative.kr (`sai(code)` with code -1): compiles, and the program stops with the runtime error and exit status 1.
- [x] `exit-codes/03-release-exits-0.png`: the v1.16.2 release, before the fix: the same `sai(256)` file compiles and the program exits with 0.
- [x] `ci-pinning/01-actions-sha.png`: Ghostty, `grep` of every `uses:` line in .github/workflows on main, each pinned to a full commit SHA with the version as a comment.
- [x] `ci-pinning/02-windows-sha256.png`: windows.yml on main: the pinned LLVM and llvm-mingw SHA256 values and the Download LLVM step comparing Get-FileHash with them.
- [ ] `wasm-check/01-check-fails-without-node.png`: Ghostty, kriol from main configured with KRIOL_ENABLE_WASM=ON: `cmake --build build/release --target check` run with node removed from PATH, ending with `wasm32-wasi tests FAIL (node is not on the PATH)` and the failed summary (the user's fix 13ad757: before, the wasm tests were silently dropped and check passed).
- [ ] `wasm-check/02-standalone-skip.png`: the same machine running `./run_tests.sh build/release/kriol .` on its own: the line `Skipping wasm32-wasi tests: node is not on the PATH` is printed instead of a silent skip.
- [ ] `macos/04-install-sh.png`: Ghostty on the Mac running the README's macOS install command (install.sh now supports macOS, anaximeno, 1.16.2): Verifying the checksum (the user's #21), Extracting, installed, then `kriol --version`.
