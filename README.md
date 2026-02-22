# Shuhao Qi - Academic Homepage

Personal academic website for Shuhao Qi, built with Jekyll and hosted via GitHub Pages.

## Live site

- Primary: <https://shuhao-qi.net>
- GitHub Pages: <https://miracle-qi.github.io>

## Tech stack

- Jekyll (Ruby)
- Custom layout based on the `minimal-light` theme structure
- Markdown + HTML sections for page content

## Repository structure

- `_config.yml`: site metadata (name, affiliation, email, links, favicon, domain)
- `index.md`: main homepage content (About, Experience, Publications, Awards, Services)
- `_layouts/homepage.html`: homepage template
- `_sass/minimal-light.scss`: main styles
- `assets/`: static files (images, PDFs, CSS/JS)
- `script/`: helper scripts for build/validation/release

## Local development

### Prerequisites

- Ruby 3.x (2.7+ usually works with this setup)
- Bundler (`gem install bundler`)

### Install dependencies

```bash
bundle install
```

### Run locally

```bash
bundle exec jekyll serve --livereload
```

Open <http://localhost:4000>.

### Build static site

```bash
bundle exec jekyll build
```

Generated output is written to `_site/`.

## Editing guide

- Update profile-level metadata in `_config.yml`.
- Edit homepage sections directly in `index.md`.
- Add papers/slides/media under `assets/pdf` and `assets/img`, then link from `index.md`.
- Adjust layout or typography in `_layouts/homepage.html` and `_sass/minimal-light.scss`.

## Deployment

This repository is configured for GitHub Pages-style deployment.

Typical flow:

```bash
git add .
git commit -m "Update homepage"
git push origin master
```

If your Pages source is the default branch, pushing to `master` updates the site automatically.

## Notes

- `_site/` and `.jekyll-cache/` are generated during local builds.
- Keep large media optimized before committing to keep the repository lightweight.

## Credits

This site is based on the `minimal-light` Jekyll theme and adapted for personal academic use.

## License

See `LICENSE`.
