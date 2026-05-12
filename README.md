# Grifball Archive

A place for all Grifball archives — community-maintained rules, events, and resources.

**Repository:** [Grifball-Archive/Grifball-Archive](https://github.com/Grifball-Archive/Grifball-Archive)

**GitHub Pages site:** [grifball-archive.github.io/Grifball-Archive](https://grifball-archive.github.io/Grifball-Archive/) (Jekyll + theme from `_config.yml`)

## Wiki (main content)

The living documentation is in this repository’s **GitHub Wiki** tab (not in this `main` branch by default).

- **Read:** [Wiki](https://github.com/Grifball-Archive/Grifball-Archive/wiki) on GitHub.
- **Edit:** sign in to GitHub → open a page → **Edit** (when the wiki is configured for open editing, any signed-in user can edit; see [CONTRIBUTING.md](CONTRIBUTING.md)).

To work locally, clone the wiki’s Git repository:

```bash
git clone https://github.com/Grifball-Archive/Grifball-Archive.wiki.git
```

## Downloading this archive

| What | How |
|------|-----|
| Main repo (this README, future non-wiki files) | [**Code** → **Download ZIP**](https://github.com/Grifball-Archive/Grifball-Archive/archive/refs/heads/main.zip), or `git clone https://github.com/Grifball-Archive/Grifball-Archive.git` |
| Wiki only | Clone `https://github.com/Grifball-Archive/Grifball-Archive.wiki.git` or use the wiki’s history and **Clone this wiki locally** on GitHub |

## Contributing

See **[CONTRIBUTING.md](CONTRIBUTING.md)** for editing norms, sidebar/footer pages, and maintainer settings (enabling the wiki and open vs collaborator-only editing).

## Jekyll theme (Pages)

Themes supported on GitHub Pages are listed at [pages.github.com/themes](https://pages.github.com/themes/). In **`_config.yml`**, set `remote_theme` to `pages-themes/<name>@v0.2.0` (use the tag from that theme’s repo if needed). Commit and push; Pages rebuilds automatically.

**Preview locally** (Ruby + Bundler required):

```bash
bundle install
bundle exec jekyll serve --livereload
```

Open `http://127.0.0.1:4000/Grifball-Archive/` (include `baseurl` path).

## License

Add a `LICENSE` file when you choose how you want text and media reused (for example a Creative Commons license for wiki content).
