# Image library

This section is for **catalog pages** about still images: screenshots, posters, UI captures, and photos. Each page should be readable on its own, with tables or lists that describe what the image is and **where to open it** (usually a path in this repo or an external URL).

## Why we keep images small and described

Large binaries make `git clone` slow and can hit host limits. Prefer **compressed** PNG or JPEG under `docs/assets/images/` (or a dedicated folder under `docs/image-library/` for grouped assets), and use this section to **name, date, and credit** what is shown.

## Example catalog layout

Below is an **illustrative** table. Replace the rows as you add real entries.

| Image | Date | What it is | Where to view |
|-------|------|-------------|----------------|
| *(example)* Finals scoreboard | 2019-07-14 | In-game end screen | `../assets/images/example-scoreboard.png` (from a page in this section) |
| *(example)* League banner | 2022-01-08 | Promotional art | `https://example.org/banner.jpg` |

When you add a real topic, create a new page under `docs/image-library/` (for example `docs/image-library/2019-finals-photos.md`), add your table and notes, then register that file in **`mkdocs.yml`** under **Image Library** so it appears in the sidebar.

## Same idea as the video library

Like **[Video Library](../video/overview.md)**, this area is for **metadata and pointers**, not for dumping huge raw files without context.
