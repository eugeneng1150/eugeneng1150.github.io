# Eugene's website

A personal blog built with Jekyll for GitHub Pages. Write articles in Markdown; Jekyll creates the web pages.

## Files to edit

- `_config.yml`: site name, description, and GitHub link.
- `about.md`: your introduction.
- `papers.md`: papers, links, and related notes.
- `_posts/`: published articles named `YYYY-MM-DD-title.md`.
- `_drafts/`: unfinished articles (not published).
- `assets/css/style.css`: typography, colors, and layout.

The README documents the repository. `index.html` is the website's homepage, showing posts by category. The navigation contains About, Categories, and Papers.

## Write a post

Create `_posts/2026-10-09-my-first-post.md`:

```markdown
---
title: "My first post"
description: "A short summary."
categories: [Notes]
math: false
---

Write your article here using Markdown.
```

The Categories homepage updates automatically. Use a date on or before today; future posts stay hidden until a build after their date. Set `math: true` for equations. See `_drafts/example-math.md` for formatting examples.

## Add papers

Edit `papers.md`, keeping its front matter at the top. Replace the empty message with paper titles, authors, links, and any notes you want to share. You can use Markdown headings to group papers by topic or year.

## Preview locally

Install a current Ruby version (3.3 or newer) and Bundler, then run:

```sh
bundle install
bundle exec jekyll serve
```

Open <http://localhost:4000>. Add `--drafts` to preview unfinished posts. Restart after changing `_config.yml`.

## Publish

1. Commit and push to `eugeneng1150/eugeneng1150.github.io`.
2. Open the repository's **Settings → Pages**.
3. Select **Deploy from a branch**, your default branch, and **/(root)**.

GitHub will build <https://eugeneng1150.github.io>. Later pushes rebuild it. Replace the sample welcome post and expand About when ready.

This original layout takes inspiration from simple academic blogs. MathJax loads from jsDelivr only on pages with `math: true`.
