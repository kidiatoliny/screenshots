# Spectra: Laravel exceptions (LinkedIn)

Planned: LI 27/11 08:30 (Europe/Luxembourg)

## Text: LinkedIn

When a Laravel endpoint returns a 500, the useful part is buried in a JSON blob: the exception class, the message, the file and the line.

Spectra, the free API client I'm building, reads that response and shows it as an exception panel instead: class, message, file and line at the top, so you know where to look before you open the editor.

It's the same idea as the rest of the app: it starts from your project, reads the routes from artisan, and treats a Laravel response like a Laravel response.

https://spectra-desktop.app

What else should an API client understand about your framework?

#Laravel #PHP #DevTools

## Screenshots

- `spectra-desktop/overview/06-laravel-exception.png`

---

# Spectra: Laravel exceptions

Planned: X 28/11 10:00, Bluesky 28/11 10:00 (Europe/Luxembourg)

## Text: X

When a Laravel endpoint returns a 500, Spectra doesn't just show you the JSON. It reads the exception and shows the class, the message, the file and the line, so you know where to look before you open the editor.

## Text: Bluesky

When a Laravel endpoint returns a 500, Spectra doesn't just show you the JSON. It reads the exception and shows the class, the message, the file and the line, so you know where to look.

#Laravel #PHP #DevTools

## Screenshots

- `spectra-desktop/overview/06-laravel-exception.png`
