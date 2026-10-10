# Swift: if let vs guard let

Project: `tips` · Status: scheduled

## Schedule

| Channel | When (Luxembourg) | Buffer post | Link |
|---|---|---|---|
| X | Tue 13 Oct, 18:00 | `6aca07b8bba9419ccbf85ddd` | |
| Bluesky | Tue 13 Oct, 18:00 | `6aca07bbbba9419ccbf85e84` | |
| LinkedIn | Fri 23 Oct, 08:30 | `6aca09fdbba9419ccbf8c8df` | |

## Images

None.

## Text: X, Bluesky

Swift: if let vs guard let

if let unwraps only inside its braces.
guard let unwraps for the rest of the function and makes you exit early when it's nil.

I use guard when a missing value means "stop here". #Swift

## Text: LinkedIn

if let or guard let in Swift?

Both unwrap an optional. The difference is scope.

if let user = currentUser { ... }
user only exists inside the braces.

guard let user = currentUser else { return }
user is available for the rest of the function, and the else forces you to leave early when it's nil.

I use guard when a missing value means the function can't continue. It keeps the happy path at the left margin instead of nested three levels deep.

Which one do you reach for by default?
