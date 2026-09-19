# rsjanssen.github.io

Source for my personal website, published with GitHub Pages.

## Structure

- `index.html` — landing page (photo, role, short intro)
- `cv.html` — background / career history
- `research.html` — research interests
- `instrumentation.html` — instrumentation work
- `outreach.html` — outreach activities
- `assets/style.css` — shared styles for every page
- `assets/headshot.jpg` — portrait photo

Every page shares the same header, top navigation, and footer markup (copy
it from any existing page when adding a new one) and all pull styling from
the single `assets/style.css`, so there's no build step — just edit the
HTML directly.

## Editing

Open the relevant page in any editor and change the text directly. To add
a new section within a page, follow the existing `<section>` pattern. The
`.placeholder` class (see `instrumentation.html` / `outreach.html`) is used
for the italic "Content coming soon." lines — replace it with real content
whenever it's ready, and there's no need to keep the class around.

To preview locally, just open `index.html` in a browser, or run a tiny local
server from this folder:

```sh
python3 -m http.server 8000
```

then visit `http://localhost:8000`.

## Publishing

This repo is named `rsjanssen.github.io`, so GitHub Pages serves it
automatically at **https://rsjanssen.github.io** once Pages is enabled
(Settings → Pages → Source: `Deploy from a branch`, branch `main`, folder
`/root`). Pushing to `main` updates the live site within a minute or two
(allow a few extra minutes for CDN caches to catch up on changed images).
