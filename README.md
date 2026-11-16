# opera-up-close

Website for Opera Up Close, live at www.operaupclose.net (GitHub Pages, see `CNAME`).

The whole site is one file, `index.html`, plus images in `photos/`.

## Adding a new night

1. Add the photos to `photos/` as `.webp` files named `<id>-01.webp`, `<id>-02.webp`, and so on.
2. In `index.html`, find `var NIGHTS = [` and add a new entry at the bottom of the list (the list runs oldest to newest).
3. Update the "Up next" section (`<section id="next">`) for the following event.

## How the Past nights section works

- The home page shows the six most recent nights, plus the "See the whole gallery" card.
- Once there are more than six nights, the oldest one drops off the home page automatically. Nothing is deleted. Every night stays in the full gallery.
- The number of nights shown on the home page is set by `HOME_LIMIT` in `index.html`.
- The date range and photo count on the "Every night" card update on their own.
