# GiorginoLab website

Static version of [www.giorginolab.it](https://www.giorginolab.it), built with
[Jekyll](https://jekyllrb.com/) and the [al-folio](https://github.com/alshedivat/al-folio)
theme, published on GitHub Pages at <https://giorginolab.github.io/>.

## Editing

| What                  | Where                                                       |
| --------------------- | ----------------------------------------------------------- |
| Pages (navbar)        | `_pages/*.md` (`nav: true`, `nav_order`)                    |
| Blog posts            | `_posts/YYYY-MM-DD-title.md`                                |
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
