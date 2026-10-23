# Kriol: shot list

Source: https://github.com/kriol-lang/kriol (KriolLang; docs https://docs.kriol.dev). The user contributes; the main author is anaximeno.
How to shoot: terminal window (Ghostty) with the code on top and the output below, plus pages of the docs site; examples live in kriol/examples/*.kriol

Screens to capture and their status. Build or open it from an up-to-date main, demo data only, window-only `screencapture` on Retina, never cropped or edited. The post that uses a feature's shots goes in that feature's folder as `post.md` (written by Claude).

- [x] `hello/01-ola-mundo.png`: The README hello world (`fn ola`, `si` / `sinon`, `mostran`) and its output when run with `kriol`.
- [ ] `errors/01-portuguese-message.png`: a compiler error, which is now written in Portuguese.
- [ ] `molda/01-recursive-field.png`: a molda with a recursive field rejected with a clear error instead of crashing (the user's fix, PR #14).
- [ ] `docs/01-home.png`: the home page of docs.kriol.dev.
- [x] `init-order/01-error.png`: Ghostty window with `tests/fail/fail_global_initializer_names_latest_global.kr` on top (cat) and `kriol` run on it below, showing the Portuguese error that says to declare 'c' before 'a'.
