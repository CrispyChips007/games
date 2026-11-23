# Games

Small browser games, served as a static site. No build step: every folder is plain HTML, CSS and JavaScript.

| Folder | Game |
| --- | --- |
| [`snake-cubed/`](snake-cubed/) | **Snake³**: snake on the six faces of a cube, in isometric view. |
| [`crunch/`](crunch/) | **Crunch**: a five-dice score challenge inspired by Farkle. Moved from the `Crunch-Game` repo. |

The root `index.html` is a landing page linking to each game. All links are relative, so the site works at any address.

## Hosting

Deployed with Cloudflare Pages from this repo: no framework preset, no build command, output directory `/`.

## Play locally

Serve the repo root with any static server (Crunch uses ES modules, which don't load from `file://`):

```sh
python -m http.server 8080
```

Then open `http://localhost:8080`.

## Tests

Crunch has a test suite: `cd crunch && npm test` (Node.js 20+).
