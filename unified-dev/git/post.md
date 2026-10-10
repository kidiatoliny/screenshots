# Favourite bug: a branch called --mirror

## Text: X, Bluesky

Favourite bug from building Unified Dev: a branch called --mirror made our git push run as git push --mirror, which deletes remote-only branches. Now every ref goes through a validator and an explicit refspec. Branch names are user input too.

## Text: LinkedIn

Favourite bug from building Unified Dev:

A branch called --mirror turned our git push into git push --mirror. That flag pushes every ref and deletes remote branches that don't exist locally. One badly named branch, and a remote-only branch was gone.

The fix wasn't a special case for that one name. Every ref now goes through a validator, and every push uses an explicit refspec, so a branch name can never be read as an option.

Branch names are user input too. So are file names, tags and commit messages, and anything you pass to a CLI deserves the same suspicion as a form field.

What's the strangest input that ever broke something of yours?
