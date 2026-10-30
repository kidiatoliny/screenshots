# Orbit: from a raw UNIQUE constraint error to an Overwrite button

## Text: X

Orbit used to show a raw "UNIQUE constraint failed: projects.slug" when you added a folder whose slug was taken. Now adding the same folder again just returns the project you already have, and a different folder with that slug gets a clear notice and an Overwrite button.

## Text: Bluesky

Orbit used to show a raw "UNIQUE constraint failed: projects.slug" when you added a folder whose slug was taken. Now adding the same folder again just returns the project you already have, and a different folder with that slug gets a clear notice and an Overwrite button.

#golang

## Screenshots

- `01-detection.png`
- `02-add-overwrite.png`
- `03-after-overwrite.png`

---

# Orbit: an overwrite in one transaction

## Text: X

Follow-up on Orbit's overwrite: it deleted the old project and created the new one in two separate statements. If the create failed, the old project was gone too, with its domains, scripts and logs. Now both run in one transaction, so a failed overwrite changes nothing.

## Text: Bluesky

Follow-up on Orbit's overwrite: it deleted the old project and created the new one in two separate statements. If the create failed, the old project was gone too, with its domains, scripts and logs. Now both run in one transaction, so a failed overwrite changes nothing.

#golang #SQLite

## Text: LinkedIn

A bug I shipped and then fixed in Orbit, my local dev runtime manager.

When you add a project whose slug is already taken, Orbit offers to overwrite the old one. The first version deleted the old project and created the new one in two separate statements. If the create failed, the old project was already gone, and with it its groups, domains, scripts and logs, because they cascade.

Now Repository.Replace runs the delete and the insert in one transaction. A failed overwrite leaves everything as it was.

The frontend had its own version of the problem: after an overwrite the list showed one project too many until you reopened the app. The store now drops any entry with the same id or slug before inserting.

Two statements that must succeed together belong in one transaction. Obvious once it's written down, easy to miss when the second one lives in another function.

#golang #SQLite #Wails
