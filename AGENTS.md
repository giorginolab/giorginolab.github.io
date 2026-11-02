# Agent guidelines — GiorginoLab website

Static Jekyll site (al-folio theme, trimmed down) for the GiorginoLab, served at
https://www.giorginolab.it/ via GitHub Pages (repository
`giorginolab/giorginolab.github.io`; custom domain set in Settings → Pages,
`giorginolab.github.io` and `giorginolab.it` redirect to it).

## Where things live

| What                  | Where                                                          |
| --------------------- | -------------------------------------------------------------- |
| Pages (menu)          | `_pages/*.md` (`nav: true`, `nav_order`, optional `nav_title`) |
| News items            | `_news/YYYY-MM-DD-title.md` (shown on the home page)           |
| Publication list      | `_bibliography/*.bib`, rendered by `_pages/publications.md`    |
| Site settings         | `_config.yml`                                                  |
| Look (fonts, colours) | `_sass/_giorginolab.scss` (all site-specific styling)          |
| Images                | `assets/img/`                                                  |

Each page's file name matches its URL (`_pages/group.md` → `/group/`, `join.md` →
`/join/`, …; `home.md` is `/`). Menu labels are the page titles (only `home.md` sets
`nav_title: Home`). There is no blog.

## Build and deploy

- One workflow only: `.github/workflows/deploy.yml` builds on push to `main` and
  publishes with the GitHub Pages actions. Do not add other workflows.
- Local preview (Ruby 3.3): `bundle install && bundle exec jekyll serve`
  (set `LANG=C.UTF-8` if BibTeX parsing fails with an encoding error).
- Format before committing: `npx prettier . --write`.

## Pitfalls

- The menu is a sticky top bar with pill links (hamburger on phones). Colours
  are CSS variables at the top of `_sass/_giorginolab.scss`, with an automatic
  dark mode (`enable_darkmode: true`). Avoid theme scripts that measure the
  navbar height (the progress bar is disabled for this reason).
- `baseurl` is empty (site served at the domain root); still use `{{ '/path/' | relative_url }}` for internal links.
- The build must not need network access (no external feeds or remote JSON).
