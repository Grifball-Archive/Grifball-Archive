# Video library

This section is for **catalog pages**: each page should be readable on its own, with tables or lists that describe what was recorded and **where to watch** it.

## Why we link instead of uploading

Video files are large. Keeping them in git makes clones slow and hits platform limits. The archive instead stores **metadata on the site** (title, date, teams, event) and a **URL** to YouTube, the Internet Archive, or another host.

## Example catalog layout

Below is an **illustrative** table. Replace the rows with real events as you add them.

| Recording | Date | What it is | Link |
|-----------|------|--------------|------|
| *(example)* Finals — Team A vs Team B | 2019-07-14 | Full series, caster audio | `https://www.youtube.com/watch?v=…` |
| *(example)* Rules clinic / Q&A | 2022-01-08 | Community workshop (unlisted OK) | `https://youtu.be/…` |

When you add a real event, create a new page under `docs/video/` (for example `docs/video/2019-summer-finals.md`). New files in this folder are listed automatically (**`append_unmatched`** in **`docs/video/.nav.yml`**); keep `overview.md` first in that file if you want the overview at the top.

## Embeds (optional)

If a host allows **embedding**, you can paste an `<iframe>` in Markdown (HTML allowed where configured) for an inline player. If you prefer a cleaner archive page, a plain link is enough.
