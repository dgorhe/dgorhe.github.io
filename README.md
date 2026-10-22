# dgorhe.github.io

Personal website of Darvesh Gorhe, built with [al-folio](https://github.com/alshedivat/al-folio) (a Jekyll academic template) and served at [darveshgorhe.com](https://darveshgorhe.com).

## Editing the site

- Site settings, name, and feature toggles: `_config.yml`
- About page (bio, photo, selected papers): `_pages/about.md`, photo in `assets/img/prof_pic.jpg`
- CV (education, experience, skills): `_data/cv.yml`
- Publications: `_bibliography/papers.bib` (BibTeX)
- Projects: `_projects/*.md`
- Blog posts: `_posts/YYYY-MM-DD-title.md` (see the placeholder post for the format and LaTeX examples)
- Social links: `_data/socials.yml`

## Local preview

```bash
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## Deployment

Pushing to `main` runs `.github/workflows/deploy.yml`, which builds the site and deploys the `_site` output to the `gh-pages` branch (the GitHub Pages source). The `CNAME` file keeps the custom domain.

## Credits

Built on the [al-folio](https://github.com/alshedivat/al-folio) template (MIT).
