# Unified Dev: Bitbucket Cloud

Planned: Bluesky 03/12 18:00, X 03/12 18:00, LI 11/12 08:30 (Europe/Luxembourg)

## Text: X

Unified Dev now works with Bitbucket Cloud. It reads the host from the remote, then shows the pull request and its builds, merges, checks out, and hands a failed Pipelines log to the agent. Each profile signs in on its own.

## Text: Bluesky

Unified Dev now works with Bitbucket Cloud. It reads the host from the remote, then shows the pull request and its builds, merges, checks out, and hands a failed Pipelines log to the agent.

#Swift #macOS #git

## Text: LinkedIn

Adding Bitbucket Cloud to Unified Dev taught me how much a git app assumes GitHub.

Unified Dev, my macOS app for running coding agents in parallel, now reads the host from the remote: bitbucket.org, including ssh.bitbucket.org addresses, is Bitbucket, everything else stays GitHub. A Bitbucket workspace shows its pull request and build statuses, merges with a strategy, checks out a pull request into a new workspace, and sends a failed Pipelines log to the agent like a GitHub Actions log.

The part I spent the most time on was the sign-in. Each profile keeps its own Bitbucket login, and git asks for the token through a credential helper scoped to bitbucket.org. No token goes in the environment, on a command line or in a URL.

And when a clone fails, the alert now shows the line that says why, not git's first line, which is always "Cloning into".

GitHub, Bitbucket or GitLab at work?

#Swift #macOS #git

## Screenshots

- `01-pr-bar.png`
