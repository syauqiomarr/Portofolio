# Portfolio Website — Syauqi Omar Nafis

A single-file, self-contained portfolio site (`index.html`) — all images are embedded, so there's nothing else to configure.

## Deploy to GitHub Pages (free hosting)

1. Create a new GitHub repository, e.g. `portfolio` (public).
2. Upload `index.html` to the root of that repo (drag-and-drop on the GitHub web UI works fine, or via git).
3. Go to **Settings → Pages**.
4. Under **Build and deployment → Source**, choose **Deploy from a branch**.
5. Pick branch **main** and folder **/ (root)**, then **Save**.
6. Wait ~1 minute — GitHub will give you a live URL:
   `https://<your-username>.github.io/portfolio/`

That's it — no build step, no dependencies.

## Editing later

Everything — text, colors, layout — lives in the single `index.html` file:
- Colors/fonts: the `:root { --bg-navy: ...; }` block near the top of the `<style>` section.
- Section content: search for the `<section class="sheet" id="...">` blocks — one per "sheet" (Cover, About, Experience, Organization, Projects, Certifications, Contact).
- To swap the profile photo or a chart image: replace the `src="data:image/...;base64,...."` value on the relevant `<img>` tag. If you'd rather use normal image files instead of embedded base64, drop them in an `assets/` folder next to `index.html` and point the `src` at e.g. `assets/profile.jpg`.

## Files

- `index.html` — the site (open directly in a browser to preview locally)
- `assets/` — original image files (profile photo + project charts), kept here for reference/editing; not required by `index.html` itself since images are embedded
