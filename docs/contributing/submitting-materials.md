# Submitting materials

## Add or edit a page

1. Open the right file under `docs/…` in the repository.
2. Add or change Markdown; add new `.md` files where they belong (`history/`, `articles/`, etc.).
3. For new pages, add a line under **`nav:`** in **`mkdocs.yml`** so they show in the sidebar.
4. Merge to `main` the way you prefer (PR or direct push).

**Not sure which section?** Add your page under **[Misc / Uncategorized](../misc/overview.md)** first; maintainers can relocate it and update `mkdocs.yml` later.

## Images

Place files under **`docs/assets/images/`**

```markdown
![caption](../assets/images/example.png)
```

Keep images reasonably small (compressed PNG or JPEG).

## Statistics files

Put exports under **`docs/assets/files/`** and describe them in a Markdown page under **`docs/statistics/`**.

## Video

Link only; see [Video Library](../video/overview.md).

## Preview locally

```bash
pip install -r requirements.txt
mkdocs serve
```

## GitHub Pages (maintainers)

Workflow: `.github/workflows/deploy-docs.yml` builds MkDocs and deploys with **GitHub Actions**.

**Settings → Pages → Build and deployment** — **Source:** **GitHub Actions**.
