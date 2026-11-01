# Maps

Source folders for every map the wiki needs. Each `maps/<slug>/` folder has a `NOTES.md` brief and an `exports/` folder. The full list, with priorities, is in [`content/_meta/Map List.md`](../content/_meta/Map%20List.md).

This folder is outside `content/`, so Quartz never publishes it.

## Conventions

These follow the same setup as `~/personal/authentica`:

- **Battle maps** are built in [Dungeondraft](https://dungeondraft.net/) on the Windows PC, at 5 ft per square.
- **Region maps** (Stonebridge, Shoreside) may suit [Wonderdraft](https://www.wonderdraft.net/) better, Dungeondraft's sister app from the same developer.
- **Exports** for each map: PNG with grid, PNG without grid, and Universal VTT (`.dd2vtt`), saved to `maps/<slug>/exports/`.
- **Never commit** `.dungeondraft` or `.wonderdraft_map` save files, asset packs (especially Patreon-licensed ones), asset libraries or thumbnails. `.gitignore` blocks them, and blocks everything in `exports/` except `.gitkeep` and `README.md`.

## Workflow

1. Pull this repo on the PC.
2. Read the map's `NOTES.md` and the wiki pages it lists.
3. Build the map, then export to `exports/`.
4. Fill in `NOTES.md` (build info, fudges, export checklist).
5. To publish a map on the wiki, save a small web-sized preview to `content/attachments/maps/<slug>.jpg`, then replace the page's `> [!map] Map placeholder` callout with `![[<slug>.jpg]]`. Full-resolution exports stay local, or go in Git LFS if you want them versioned.
