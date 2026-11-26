# my-site

Personal scientific portfolio for Ali Rihani. Plain HTML and CSS: no framework and no build step.

- `index.html` holds all content (intro, current work, experience, education and grants, expertise, publications, talks, contact)
- `style.css` holds the styling (light and dark mode follow the visitor's system setting)
- `.nojekyll` tells GitHub Pages to serve the files as they are

## Deploy to GitHub Pages

Deployment runs through GitHub Actions (`.github/workflows/deploy.yml`) on every push to `main`.

1. Create a repository, for example `<username>.github.io` (for a site at `https://<username>.github.io/`) or any other name (for a site at `https://<username>.github.io/<repo>/`).
2. Put the contents of this folder, including the hidden `.github/` folder, at the root of the repository on the `main` branch.
3. On GitHub, go to **Settings → Pages → Build and deployment** and set **Source** to **GitHub Actions**.
4. Push to `main`. Watch the run under the **Actions** tab; the site URL appears on the run's summary page and under **Settings → Pages**.

## Updating

To add a paper, copy one `<li>` block inside `<ol class="pubs">` in `index.html` and place it at the top of the list. Your name is wrapped in `<span class="me">` so it shows in bold.
