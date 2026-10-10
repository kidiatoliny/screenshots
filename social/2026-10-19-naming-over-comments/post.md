# Naming over comments

Project: `tips` · Status: scheduled

## Schedule

| Channel | When (Luxembourg) | Buffer post | Link |
|---|---|---|---|
| LinkedIn | Mon 19 Oct, 08:30 | `6ac248dbd8dbde86e147309f` | |

X and Bluesky version published Wed 7 Oct.

## Images

None.

## Text: LinkedIn

If a variable needs a comment to explain what it holds, rename it first.

// days until the subscription expires
const d = 14;

versus

const daysUntilExpiry = 14;

The second one doesn't need the comment, and it stays clear everywhere the variable is used, not just on the line where it's declared.

Comments are great for explaining why something is done. The name should handle the what.
