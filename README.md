# Meridian Academic Theme

A small Jekyll theme for an academic reading room.

## Structure

- `_config.yml` — site metadata and the author block
- `_pages/about.md` — the landing page, currently a biography placeholder
- `_pages/publications.md` — renders every document in the `publications` collection
- `_publications/` — one Markdown document per publication
- `_data/navigation.yml` — top navigation

## Adding a publication

Create `_publications/<slug>.md` with front matter:

    ---
    title: "Paper title"
    authors: "Author One, Author Two"
    category: "cs.LG"
    date: 2024-05-31
    arxiv: "2405.21060"
    paperurl: "https://arxiv.org/abs/2405.21060"
    ---

Then write a sentence or two about the paper in the body. The Publications page
renders the collection automatically.
