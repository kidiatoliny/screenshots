# Go: wrap errors with %w

Project: `tips` · Status: scheduled

## Schedule

| Channel | When (Luxembourg) | Buffer post | Link |
|---|---|---|---|
| X | Mon 12 Oct, 10:00 | `6aca078aed92ed8fa5c2ff02` | |
| Bluesky | Mon 12 Oct, 10:00 | `6aca0791ed92ed8fa5c2ffc8` | |
| LinkedIn | Wed 21 Oct, 08:30 | `6aca09f4c4de2d2b1220f1cd` | |

## Images

None.

## Text: X, Bluesky

Go tip: when you pass an error up, wrap it with %w:

return fmt.Errorf("load config: %w", err)

The message gets context, and callers can still match the original error with Is and As from the errors package. #golang

## Text: LinkedIn

Small Go habit that makes debugging much easier: wrap errors with %w when you pass them up.

return fmt.Errorf("load config: %w", err)

Without it, you get a log line that just says "no such file or directory" and no idea which call failed. With it, the message reads like a trail: "start server: load config: open config.yaml: no such file or directory".

And because %w keeps the original error, callers can still check for fs.ErrNotExist with the errors package.

How do you handle errors in Go: wrap everything, or only at the boundaries?
