# GiorginoLab website

Static version of [www.giorginolab.it](https://www.giorginolab.it), built with
[Jekyll](https://jekyllrb.com/) and the [al-folio](https://github.com/alshedivat/al-folio)
theme, published on GitHub Pages at <https://tonigi.github.io/prova1/>.

## Editing

| What             | Where                                                       |
| ---------------- | ----------------------------------------------------------- |
| Pages (navbar)   | `_pages/*.md` (`nav: true`, `nav_order`)                    |
| Blog posts       | `_posts/YYYY-MM-DD-title.md`                                |
| Publication list | `_bibliography/*.bib`, rendered by `_pages/publications.md` |
| Site settings    | `_config.yml`                                               |
| Images           | `assets/img/`                                               |

Push to `master`: the single workflow `.github/workflows/deploy.yml` builds the
site and pushes it to the `gh-pages` branch (Settings → Pages → Deploy from a
branch → `gh-pages`).

## Local preview

```bash
docker compose up        # http://localhost:8080
```

or, with Ruby 3.3:

```bash
bundle install && bundle exec jekyll serve
```
