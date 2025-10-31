Hugo homework scaffold

This repository contains a Hugo-based personal site scaffold built for a homework assignment. It's styled as a compact academic/business-card personal site with:

- A left sidebar with my name, contact info, and navigation
- A homepage written in first-person voice with contact links and featured projects
- At least two posts (see `content/posts/`) and an `About` and `Projects` page
- A profile SVG in `static/images/cs-logo.svg`
- A GitHub Actions workflow to build and deploy to GitHub Pages

How to run locally (WSL)

1. Install Hugo (if not installed). Example using snapd on WSL:

```bash
sudo snap install hugo --channel=extended
```

2. From the project root run:

```bash
cd /mnt/c/Users/bizim/OneDrive/Desktop/hugo
hugo server -D
```

Open http://localhost:1313 in your browser.

Deploying to GitHub Pages

1. Create a GitHub repository and push this project to it on branch `main`.
2. Update `baseURL` in `config.toml` to the actual GitHub Pages URL (e.g. `https://<username>.github.io/<repo>/`).
3. Pushing to `main` will trigger the GitHub Actions workflow at `.github/workflows/gh-pages.yml` which builds and publishes `public/`.

If you'd like, I can initialize the git repo here and push to GitHub for you — say the word and provide the repo name and whether you want it public or private.
