# Submitting materials

The **library website** is generated from the **`docs/`** folder using [MkDocs Material](https://squidfunk.github.io/mkdocs-material/). Changes merge through **pull requests** on [Grifball-Archive/Grifball-Archive](https://github.com/Grifball-Archive/Grifball-Archive), similar in workflow to GitBook-backed wikis such as [TSG Forge Wiki](https://wiki.thescriptersguild.com/) (which uses GitBook’s GitHub integration).

## Add or edit a page

1. Browse to `docs/…` in the repository.
2. Use the **Edit** (pencil) button, or fork and edit in your fork.
3. Add new `.md` files in the right section (`history/`, `articles/`, etc.).
4. Add an entry under **`nav:`** in **`mkdocs.yml`** so the page appears in the sidebar.
5. Open a **pull request** into `main`.

## Images

Place files under **`docs/assets/images/`**. From a page in `docs/articles/foo.md`, reference:

```markdown
![caption](../assets/images/example.png)
```

Keep images reasonably small (compressed PNG or JPEG).

## Statistics files

Put exports under **`docs/assets/files/`** and describe them in a Markdown page under **`docs/statistics/`**.

## Video

Link only; see [Video library](../video/overview.md).

## Preview locally

```bash
pip install -r requirements.txt
mkdocs serve
```

## GitHub Pages (maintainers)

Workflow: `.github/workflows/deploy-docs.yml` publishes the built site to the **`gh-pages`** branch.

**Settings → Pages:** source **Deploy from a branch** → **`gh-pages`** / **`/`** (root).

## Optional GitHub Wiki tab

The [GitHub Wiki](https://github.com/Grifball-Archive/Grifball-Archive/wiki) is optional scratch space. **Canonical** library content should live under **`docs/`** so it appears in search and the sidebar.
