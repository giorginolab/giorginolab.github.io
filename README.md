# GiorginoLab website

Website of the GiorginoLab, <https://www.giorginolab.it/>. Built with
[Jekyll](https://jekyllrb.com/) and the [al-folio](https://github.com/alshedivat/al-folio)
theme and published with GitHub Pages (custom domain of `giorginolab.github.io`).

## Editing

| What                  | Where                                                       |
| --------------------- | ----------------------------------------------------------- |
| Pages (navbar)        | `_pages/*.md` (`nav: true`, `nav_order`)                    |
| News items            | `_news/YYYY-MM-DD-title.md` (shown on the home page)        |
| Publication list      | `_bibliography/*.bib`, rendered by `_pages/publications.md` |
| Site settings         | `_config.yml`                                               |
| Look (fonts, colours) | `_sass/_giorginolab.scss`                                   |
| Images                | `assets/img/`                                               |

Push to `main`: the single workflow `.github/workflows/deploy.yml` builds the
site and publishes it with GitHub Pages (Settings → Pages → Source: GitHub Actions).

## Local preview

With Ruby 3.3:

```bash
bundle install && bundle exec jekyll serve   # http://localhost:4000/
```
