# Spectra: import from curl and HAR

Planned: X 17/12 18:00, Bluesky 17/12 18:00, LinkedIn 17/12 08:30 (Europe/Luxembourg)

## Text: X

Spectra can import a request from curl or from a HAR file. Copy as curl in your browser's DevTools, paste it in, and it becomes a request you can edit and send, kept with the project.

## Text: Bluesky

Spectra can import a request from curl or from a HAR file. Copy as curl in your browser's DevTools, paste it in, and it becomes a request you can edit and send, kept with the project.

#DevTools #Laravel

## Text: LinkedIn

The fastest way to reproduce a bug a user hit is usually the request their browser sent.

Spectra, the free API client I'm building, imports a request from curl or from a HAR file. In Chrome DevTools, Network, right-click the request, Copy as curl, paste it into Spectra, and it becomes a request you can edit and send again, with the body pretty-printed. Scratch requests are saved per project, so they're still there tomorrow.

It sits next to the routes Spectra reads from your Laravel or NestJS code, so you can compare what the browser sent with what the endpoint expects.

https://spectra-desktop.app

#DevTools #Laravel #API

## Screenshots

- `spectra-desktop/import/01-curl.png`
