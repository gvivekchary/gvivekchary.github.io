# AGENTS.md

## Cursor Cloud specific instructions

This is a **static HTML/CSS/JS portfolio website** with zero build tools, no package manager, and no backend. All frontend libraries (Bootstrap 5, AOS, Font Awesome, PureCounter, etc.) are vendored as pre-built minified files in `css/` and `scripts/`.

### Running the dev server

Serve the repo root with any static HTTP file server. The README recommends:

```
python3 -m http.server 8080 --directory /workspace
```

Then open `http://localhost:8080/` (or `/vivek-portfolio.html`).

Opening HTML files via `file://` breaks relative asset paths — always use an HTTP server.

### Lint / Test / Build

There are no linting tools, automated tests, or build steps configured in this repository. Changes are validated by visual inspection in a browser.

### Key files

- `index.html` / `vivek-portfolio.html` — main portfolio page (identical content)
- `privacy.html` — privacy policy page
- `css/` — vendored CSS (Bootstrap, AOS, Font Awesome, Bootstrap Icons, custom `main.css`)
- `scripts/` — vendored JS libraries + custom `main.js`
- `images/` — SVG illustrations, service icons, hero photos
- `resume.pdf` — downloadable resume
