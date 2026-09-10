# rezashkv.github.io

Personal academic site, built with [Jekyll](https://jekyllrb.com) and served by GitHub Pages.

## Editing content

| What                | Where                                  |
| ------------------- | -------------------------------------- |
| Bio, intro, blurb   | `_pages/about.html` (front matter + body) |
| News items          | `_data/news.yml` (newest first)         |
| Papers              | `_publications/*.md` (one file each)    |
| Navigation          | `_data/navigation.yml`                  |
| Name, links, avatar | `_config.yml` (`author:` block)          |
| CV                  | `files/CV.pdf`                          |

### Adding a paper

Create `_publications/<slug>.md`:

```yaml
---
title: "Paper title"
collection: publications
permalink: /publications/<slug>/
date: 2026-06-18          # drives the year grouping and ordering
venue: "ECCV 2026"        # append " Spotlight" or " Oral" to flag it
venueurl: "https://..."
paperurl: "https://arxiv.org/abs/..."
githuburl: "https://github.com/..."   # labelled Code / Data / Project automatically
authors: "First Author, Reza Shirkavand, Last Author"
figure: "/images/<slug>.png"
---
Optional abstract. If present, an "Abstract" chip links to the paper's own page.
```

Then generate the list thumbnail, so the home page doesn't load the full figure:

```sh
sips -Z 560 --setProperty format jpeg --setProperty formatOptions 78 \
  images/<slug>.png --out images/thumbs/<slug>.jpg
```

The name must match the figure's (`images/foo.png` -> `images/thumbs/foo.jpg`).
If the thumbnail is missing the page falls back to the full figure, so the site
still builds -- it just downloads more.

## Theme

Custom, in three files:

- `assets/css/main.scss` — all styling, driven by the tokens in `:root`
- `_layouts/` — `default`, `home`, `page`, `publication`
- `_includes/` — `masthead`, `footer`, `contacts`, `publication-item`, `head`, `scripts`

Originally forked from [academicpages](https://github.com/academicpages/academicpages.github.io) (MIT); the theme layer has since been replaced.

## Local preview

```sh
jekyll build            # or: jekyll serve --config _config.yml,_config.dev.yml
```
