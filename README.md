# OrbitX website

Static site (plain HTML and one CSS file; no JavaScript, cookies or external resources).

- `index.html` (English only), `privacy.html`, `impressum.html`
- `index.html` has its own inline CSS, `img/` (WebP screenshots `hero.webp` and `shot-privacy.webp`, the app icon, Microsoft's official Store badge: never edit that file), `favicon-32.png`, `apple-touch-icon.png` and `qr-store.svg`
- `style.css`: the stylesheet of `privacy.html` and `impressum.html` (light and dark follow the system)
- `.nojekyll`: tells GitHub Pages to serve the files as they are

## Publishing (GitHub Pages)

GitHub Pages on a free account needs a **public** repository. This app repository is private, so the contents of this folder go into a separate public repository (suggested name `orbitx-site`):

1. Create the public repository `orbitx-site` and copy everything in this `site/` folder to its root (`index.html` at the top).
2. Repository > Settings > Pages > Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
3. The site is then at `https://<user>.github.io/orbitx-site/`. All links are relative, so a sub-path works.

Before going live: the Store button and QR code (`qr-store.svg`, black on white, made once with the `qrcodegen` crate; no external service) point at the Microsoft Store page; the direct download is still "Coming soon" and review `privacy.html` and `impressum.html`.
