# Agent guidelines — GiorginoLab website

Static Jekyll site (al-folio theme, trimmed down) that mirrors www.giorginolab.it,
published on GitHub Pages at https://giorginolab.github.io/
(repository `giorginolab/giorginolab.github.io`).

## Where things live

| What                  | Where                                                          |
| --------------------- | -------------------------------------------------------------- |
| Pages (menu)          | `_pages/*.md` (`nav: true`, `nav_order`, optional `nav_title`) |
| Blog posts            | `_posts/YYYY-MM-DD-title.md`                                   |
| Publication list      | `_bibliography/*.bib`, rendered by `_pages/publications.md`    |
| Site settings         | `_config.yml`                                                  |
| Look (fonts, colours) | `_sass/_giorginolab.scss` (all site-specific styling)          |
| Images                | `assets/img/`                                                  |

Keep page URLs as on the original Google Sites site (`/teaching/`, `/software/`,
`/available-theses/`, `/publications/`).

## Build and deploy

- One workflow only: `.github/workflows/deploy.yml` builds on push to `main` and
  publishes with the GitHub Pages actions. Do not add other workflows.
- Local preview (Ruby 3.3): `bundle install && bundle exec jekyll serve`
  (set `LANG=C.UTF-8` if BibTeX parsing fails with an encoding error).
- Format before committing: `npx prettier . --write`.

## Pitfalls

- The menu is a fixed left sidebar on wide screens; avoid theme scripts that
  measure the navbar height (the progress bar is disabled for this reason).
- `baseurl` is empty (site served at the domain root); still use `{{ '/path/' | relative_url }}` for internal links.
- The build must not need network access (no external feeds or remote JSON).
