# dongxiaw.github.io

Personal academic homepage of **Dongxia Wu** — a lightweight, single-page
[Jekyll](https://jekyllrb.com/) site hosted on GitHub Pages.

## Editing content

Almost everything is data-driven. To update the site, edit **`_data/data.yml`**:

| Key            | What it controls                                                        |
| -------------- | ----------------------------------------------------------------------- |
| `profile`      | Name, title, photo, email, CV link, and social links (GitHub, Scholar…) |
| `bio`          | The introductory paragraph in the header (supports Markdown links)      |
| `news`         | Dated news items (most recent first)                                    |
| `research`     | Research thrusts with taglines and motivation text                      |
| `recruiting`   | Prospective-students section: blurb, topic areas, application note      |
| `publications` | Paper list, grouped automatically by `year` (most recent first)         |

To add a publication, append an entry under `publications.papers` with
`title`, `link`, `authors` (wrap your own name in `<b>…</b>`), `venue`, and `year`.

## Structure

- `index.html` — section order (header → news → research → students → publications)
- `_layouts/default.html` — page shell
- `_includes/*.html` — one file per section (`header`, `news`, `research`, `students`, `publications`, `navbar`, `footer`, `scripts`)
- `assets/css/main.scss` — all styling (teal accent theme, responsive)
- `assets/images/` — `dongxiawu-web.jpg` is the displayed avatar; `dongxiawu.jpeg` is the full-res original

## Local development

Requires Ruby + Jekyll:

```bash
gem install jekyll bundler
jekyll serve         # http://localhost:4000
```

GitHub Pages builds and deploys automatically on push to the default branch.
