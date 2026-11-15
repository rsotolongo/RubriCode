# RubriCode

Landing page for [RubriCode](https://rubricode.com), a software development consulting startup.

The page has a terminal-style look. The `/about` and `/contact` links open draggable windows built with the [WinBox](https://github.com/nextapps-de/winbox) library.

## Project structure

```text
.
├── index.html            # Page markup, including the hidden content mounted into the windows
├── css/style.css         # Styles (Roboto Mono, green-on-dark theme)
├── js/main.js            # Opens the About and Contact windows on click
├── js/winbox.bundle.js   # WinBox.js v0.1.8 bundle (vendored)
├── img/favicon.ico
└── CNAME                 # Custom domain for GitHub Pages
```

## Running locally

It's a static site with no build step. Open `index.html` in a browser, or serve the folder:

```bash
python3 -m http.server 8000
```

Then visit <http://localhost:8000>.

## Deployment

The site is published with GitHub Pages from the root of the `main` branch, at the custom domain `rubricode.com` (set in `CNAME`), with HTTPS enforced. Every push to `main` redeploys it.

## Contributing

This repository is public for reference only. It doesn't accept pull requests or outside contributions.

## Third-party code

[WinBox.js](https://github.com/nextapps-de/winbox) © Nextapps GmbH, licensed under Apache-2.0.
