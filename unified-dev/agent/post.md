# Swift concurrency: the Stop button and AsyncStream

## Text: X, Bluesky

Swift concurrency lesson from Unified Dev: cancelling the Task that iterates an AsyncStream ends that stream for good. Our Stop button did exactly that, so every later agent turn ran with nobody listening. The runner now multiplexes its events instead. #Swift

## Text: LinkedIn

A Swift concurrency lesson from building Unified Dev.

Unified Dev streams each agent's events through an AsyncStream, and the Stop button cancelled the Task that was iterating it.

What I didn't know: cancelling the Task that iterates an AsyncStream ends that stream for good. So Stop worked once, and every later agent turn ran with nobody listening.

The fix was to stop tying the events to one consumer. The runner now multiplexes its events, so stopping a turn doesn't kill the stream the next turn needs.

If you use AsyncStream for events that outlive a single task, check what your cancel path actually ends.

Has Swift concurrency cancellation ever surprised you like this?
