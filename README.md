[aidancurtis.github.io](https://aidancurtis.github.io)

Built by GitHub Pages' Jekyll on every push to `main`. Nothing to install to deploy.

## Write a post ("Thoughts")

Create `_posts/YYYY-MM-DD-some-title.md`:

```markdown
---
layout: post
title: My post title
description: One line shown on the Thoughts page (optional)
math: true # only if the post uses LaTeX
---

Post body in Markdown.
```

It appears at `/thoughts/some-title/` and on the Thoughts page. Posts with a future date aren't published until that date.

## Add a paper

Add an entry at the top of `_data/papers.yml`. Only `title` is required:

```yaml
- title: "Paper title"
  authors: "<b>Aidan Curtis</b>, Coauthor Name"
  venue: "arXiv preprint"
  year: 2026
  note: "Optional extra line"
  links:            # each key becomes a [label]
    pdf: "https://..."
    arXiv: "https://..."
    code: "https://..."
```

Papers show on the Research tab (`/research/`).
Put any self-hosted PDFs in `docs/`.

## Add a book

Add an entry under `reading` or `read` in `_data/books.yml`.

## Preview locally (optional)

Needs Ruby 3+ (macOS's built-in Ruby is too old; `brew install ruby` first):

```sh
gem install jekyll
jekyll serve   # http://localhost:4000
```
