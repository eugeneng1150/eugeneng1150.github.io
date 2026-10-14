This is Eugene repo for blogs

## Adding papers

Each paper has its own Markdown file in `_papers/`. The Papers page lists
published papers automatically, alphabetically by title.

1. Copy `_papers/example-paper.md` to `_papers/your-paper-name.md`.
2. Update the title, description, and original paper link in the settings at the top.
3. Remove `published: false` when you are ready to publish.
4. Write your notes below the settings using Markdown, then commit and push.

The file `_papers/your-paper-name.md` becomes `/papers/your-paper-name/`.
The description and `paper_url` are optional. Add `math: true` to the settings
if your notes use LaTeX equations. Keep `published: false` on unfinished papers
to hide both their pages and index entries from the normal site build.

You do not need to edit `papers.md` when adding a paper; it is the automatic index.
