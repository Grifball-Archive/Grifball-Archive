# Grifball Archive

A place for all Grifball archives — a **public library** of **history**: articles, statistics, and video records. This repository is for **browsing and preservation**, not for running a league (no sign-ups, live schedules, or ops tooling here).

**Repository:** [Grifball-Archive/Grifball-Archive](https://github.com/Grifball-Archive/Grifball-Archive)

**Library website (browse):** [grifball-archive.github.io/Grifball-Archive](https://grifball-archive.github.io/Grifball-Archive/)

The site is built with **[MkDocs Material](https://squidfunk.github.io/mkdocs-material/)** on GitHub Pages so it feels like a **GitBook-style** wiki: **sidebar navigation**, **search**, and an **on-page table of contents** — the same *kind* of reading experience as [TSG Forge Wiki](https://wiki.thescriptersguild.com/) (TSG uses GitBook itself; we use MkDocs on a free org for a close match).

## Content location

All library pages and assets live under **`docs/`**. The outline is defined in **`mkdocs.yml`** (like a GitBook summary file).

## Download everything

| Method | What you get |
|--------|----------------|
| **Clone** | Full history + `docs/` and assets: `git clone https://github.com/Grifball-Archive/Grifball-Archive.git` |
| **ZIP** | [Download ZIP](https://github.com/Grifball-Archive/Grifball-Archive/archive/refs/heads/main.zip) |

## Contributing

See **[docs/contributing/submitting-materials.md](docs/contributing/submitting-materials.md)** and the short **[CONTRIBUTING.md](CONTRIBUTING.md)** entry point.

## GitHub Pages setup

The workflow [.github/workflows/deploy-docs.yml](.github/workflows/deploy-docs.yml) publishes the built MkDocs site with **GitHub Actions** (not the raw `main` branch).

1. **Settings → Pages → Build and deployment**
2. Set **Source** to **GitHub Actions** (not “Deploy from a branch”).
3. Merge to `main` and let the **Deploy documentation to GitHub Pages** workflow finish. Approve it if the org/repo asks on first run.

If **Source** is still **Deploy from branch `main`**, GitHub can keep serving an **old Jekyll placeholder** that mostly links back to the repo. Switching to **GitHub Actions** is what makes the **full library pages** appear at the same URL.

## License

Add a `LICENSE` when you decide how text and files may be reused (for example Creative Commons for prose).
