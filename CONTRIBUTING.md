# Contributing to the Grifball Archive wiki

**Repository:** [Grifball-Archive/Grifball-Archive](https://github.com/Grifball-Archive/Grifball-Archive) · **Wiki:** [wiki home](https://github.com/Grifball-Archive/Grifball-Archive/wiki) · **Pages site (orientation only):** [grifball-archive.github.io/Grifball-Archive](https://grifball-archive.github.io/Grifball-Archive/)

The **wiki** is where articles and the archive live. The **Pages** URL is a small Jekyll site with links into the wiki — not a second wiki.

## Who can edit

This project uses GitHub’s **Wiki** feature.

- **Open wiki:** any signed-in GitHub user can edit pages live.

## Editing in the browser

1. Open [the repository on GitHub](https://github.com/Grifball-Archive/Grifball-Archive).
2. Go to the **Wiki** tab.
3. Use **New Page** or open an existing page → **Edit**.
4. Use **Preview** before saving when possible.

Markdown works like elsewhere on GitHub. You can attach images through the editor where supported.

## Articles, images, spreadsheets, and video

The wiki is best for **text articles** (Markdown pages) plus **small supporting files**. Large or heavy media usually belongs as a **link** to a proper host, not inside the wiki git repo.

### Articles

- Add a **new wiki page** (or extend an existing one) with a clear title.
- Use headings, short paragraphs, and links to sources. If the topic is big, split into multiple pages and link between them.

### Images (screenshots, maps, posters)

- **In the browser:** when editing a wiki page, use the editor’s **image upload** (drag-and-drop or attach) if available; GitHub will store the file in the wiki and insert a link.
- **From a clone:** create a folder such as `images/` in the wiki repo, add files with descriptive names (e.g. `2024-h3-tournament-bracket.png`), commit, and reference them in Markdown, e.g. `![bracket](images/2024-h3-tournament-bracket.png)`.
- Prefer **PNG** or **JPEG**, reasonable resolution, and **small file sizes** (large PNGs slow down the page and the repo). Avoid huge originals unless there’s a strong reason.

### Google Sheets (or other spreadsheets)

Pick one approach (you can combine them):

1. **Link (quick):** share the sheet as **view-only** (“Anyone with the link can view”), and paste that URL on the wiki page with a short description of what it contains. *Risk:* the link dies if the file is deleted or permissions change.
2. **Archive in the wiki (durable):** in Google Sheets use **File → Download** and save e.g. **CSV** (great for data), **PDF** (great for “looks like the sheet”), or **XLSX**. Put exports in a folder like `files/` via a **wiki clone**, commit, and link to the file from the article so people can download a snapshot that stays with the archive.

For anything important long-term, prefer **downloaded exports** or a copy the org controls, not only a live Google link.

### Video

GitHub wikis are **git repositories**; they are a poor place for big binary files (slow clones, size limits, no streaming). **Do not** rely on uploading full videos into the wiki.

- **Preferred:** upload to **YouTube** (public or **unlisted**), **Internet Archive**, or another stable host, then on the wiki add a **short article** with context, date, and the **link** (and optionally a thumbnail image).

## Cloning the wiki locally

The wiki is stored in a separate Git repo:

```text
https://github.com/Grifball-Archive/Grifball-Archive.wiki.git
```

On the wiki’s GitHub page, use **Clone this wiki locally** to copy the exact URL. Then:

```bash
git clone https://github.com/Grifball-Archive/Grifball-Archive.wiki.git
cd Grifball-Archive.wiki
# edit .md files, commit, push (push requires permission to edit the wiki)
```

Convention: wiki page `Home` is usually in `Home.md`.

### Sidebar and footer (optional)

In the wiki clone, you can add:

- `_Sidebar.md` — custom sidebar (Markdown + links).
- `_Footer.md` — footer on wiki pages.

Commit and push like any other wiki page.

## GitHub Pages site (maintainers)

The landing page at [grifball-archive.github.io/Grifball-Archive](https://grifball-archive.github.io/Grifball-Archive/) is built with Jekyll from this repo (`index.md`, `_config.yml`). Most contributors never need to touch this.

**Change the theme:** edit `remote_theme` in `_config.yml`. Official options: [pages.github.com/themes](https://pages.github.com/themes/). Push to `main`; Pages rebuilds automatically.

**Preview locally** (Ruby + Bundler):

```bash
bundle install
bundle exec jekyll serve --livereload
```

Open `http://127.0.0.1:4000/Grifball-Archive/` (include the `baseurl` path).
