# OrbitX website

Static site (plain HTML and one CSS file; no JavaScript, cookies or external resources).

- `index.html` (English), `de/index.html` (German), `privacy.html`, `impressum.html`
- `style.css`: the only stylesheet (light and dark follow the system)
- `.nojekyll`: tells GitHub Pages to serve the files as they are

## Publishing (GitHub Pages)

GitHub Pages on a free account needs a **public** repository. This app repository is private, so the contents of this folder go into a separate public repository (suggested name `orbitx-site`):

1. Create the public repository `orbitx-site` and copy everything in this `site/` folder to its root (`index.html` at the top).
2. Repository > Settings > Pages > Source: "Deploy from a branch", branch `main`, folder `/ (root)`.
3. The site is then at `https://<user>.github.io/orbitx-site/`. All links are relative, so a sub-path works.

Before going live: replace the placeholder download links in both `index.html` files (the Store address and the direct download are shown as "Coming soon" until they exist) and review `privacy.html` and `impressum.html`.
