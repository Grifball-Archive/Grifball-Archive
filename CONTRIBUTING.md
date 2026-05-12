# Contributing to the Grifball Archive wiki

**Repository:** [Grifball-Archive/Grifball-Archive](https://github.com/Grifball-Archive/Grifball-Archive) · **Wiki:** [wiki home](https://github.com/Grifball-Archive/Grifball-Archive/wiki)

## Who can edit

This project uses GitHub’s **Wiki** feature. Editing permissions are controlled only in **repository settings** (there is no per-page lock).

- **Open wiki:** any signed-in GitHub user can edit pages live.
- **Collaborators only:** only people with write access to the repository can edit.

You can switch between these at any time; see [Maintainer checklist](#maintainer-checklist).

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

## Content guidelines

- Prefer clear titles, short sections, and links between related pages.
- When stating facts (dates, rules, quotes), cite or link to a source when you can.
- If something is uncertain, say so; avoid presenting guesses as established history.
- Treat other contributors respectfully; disruptive or abusive edits may be reverted and permissions may be tightened.

## Maintainer checklist

Do these in the GitHub UI for **Grifball-Archive/Grifball-Archive**:

1. **Settings** → **General** → **Features** → enable **Wikis**.
2. **Open wiki (your current plan):** under **Features**, ensure **Restrict editing to collaborators only** is **unchecked** so any signed-in user may edit.  
   To restrict later, check that option again.
3. Optionally add trusted people under **Collaborators and teams** (or org teams) so they have **Write** access to the main repo if they should help moderate or revert via history.
4. Create a **Home** page in the wiki with a short intro and links to important topics.

### If the org uses “default repository settings”

Org owners may need to allow wikis for this repo or confirm that non-members can edit public wikis when restriction is off. Check **Organization settings** → **Member privileges** / repository policy if something is unexpectedly blocked.

## Main repository vs wiki

- **Wiki:** community pages, quick updates, open editing (as configured).
- **This `main` branch:** optional “shell” — README, policies, or exported snapshots. Changes here use normal **pull requests** if you add collaborators with write access.
