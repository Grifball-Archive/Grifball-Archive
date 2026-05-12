# Contributing to the Grifball Archive wiki

**Repository:** [Grifball-Archive/Grifball-Archive](https://github.com/Grifball-Archive/Grifball-Archive) · **Wiki:** [wiki home](https://github.com/Grifball-Archive/Grifball-Archive/wiki)

## Who can edit

This project uses GitHub’s **Wiki** feature.

- **Open wiki:** any signed-in GitHub user can edit pages live.

## Editing in the browser

1. Open [the repository on GitHub](https://github.com/Grifball-Archive/Grifball-Archive).
2. Go to the **Wiki** tab.
3. Use **New Page** or open an existing page → **Edit**.
4. Use **Preview** before saving when possible.

Markdown works like elsewhere on GitHub. You can attach images through the editor where supported.

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
