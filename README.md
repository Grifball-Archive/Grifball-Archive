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

1. Open **Settings → Pages → Build and deployment**.
2. Set **Source** to **GitHub Actions** (not “Deploy from a branch”).
3. Push to `main` (or run the workflow manually) and let **Deploy documentation to GitHub Pages** finish. Approve the workflow if GitHub asks on first run.

Until **Source** is **GitHub Actions**, GitHub may keep serving an **older Jekyll “front door”** from `main` that mostly links back to the repo. After Actions is the source, the **MkDocs** site (everything under `docs/`) is what readers see at the same URL.

## License

Add a `LICENSE` when you decide how text and files may be reused (for example Creative Commons for prose).
