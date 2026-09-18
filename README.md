# rsjanssen.github.io

Source for my personal website, published with GitHub Pages.

## Structure

- `index.html` — the whole site (single page, styles inlined, no build step)
- `assets/headshot.jpg` — portrait photo

## Editing

Open `index.html` in any editor and change the text directly — bio is in the
`#about` section, career history in `#background`, and links in `#links`.
There's a `<!-- TODO -->` comment next to the ORCID link marking where to
drop in the real profile URL.

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
`/root`). Pushing to `main` updates the live site within a minute or two.
