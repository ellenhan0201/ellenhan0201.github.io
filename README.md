# Yanting Han Website

Source for <https://ellenhan0201.github.io>, built with the [al-folio](https://github.com/alshedivat/al-folio) Jekyll theme and deployed with GitHub Pages.

## Local Preview

GitHub Actions builds with Ruby 3.3.5. To preview locally:

```bash
bundle install
bundle exec jekyll serve --host 127.0.0.1 --port 4000 --livereload
```

Then open <http://127.0.0.1:4000>.

## Common Updates

- Homepage: `_pages/about.md`
- Research projects: `_projects/`
- Publications: `_bibliography/papers.bib`
- Resume page: `_pages/cv.md`
- Resume PDFs: `assets/pdf/`

Pushes to `main` trigger the deploy workflow in `.github/workflows/deploy.yml`.
