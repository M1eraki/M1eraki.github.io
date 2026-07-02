# Chao Peng Ji Academic Homepage

This repository contains an al-folio academic homepage starter prepared for Chao Peng Ji.

It is based on [al-folio](https://github.com/alshedivat/al-folio), a clean and responsive Jekyll theme for academics.

## What To Edit First

- `_config.yml`: site name, URL, description, search, and theme settings.
- `_pages/about.md`: homepage bio and profile block.
- `_data/socials.yml`: email, GitHub, Google Scholar, ORCID, LinkedIn, and RSS.
- `_bibliography/papers.bib`: publication list.
- `_projects/`: selected project pages.
- `_data/cv.yml`: CV content.
- `PERSONALIZE.md`: checklist for making the draft fully yours.

## Local Preview

With Docker:

```bash
docker compose pull
docker compose up
```

Then open `http://localhost:8080`.

Without Docker:

```bash
bundle install
bundle exec jekyll serve
```

Then open `http://localhost:4000`.

## Publish With GitHub Pages

For a personal site, use a repository named `M1eraki.github.io`, keep `baseurl` blank in `_config.yml`, and push to `main`.

After the first GitHub Actions deployment completes, set GitHub Pages to deploy from the `gh-pages` branch.
