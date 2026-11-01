# Scales of Faith

A system-neutral fantasy campaign setting for game masters, published as a wiki at
**https://trak3r.github.io/scales-of-faith/**.

> In a world where dragons are nothing but children's stories, two secret orders race to find
> the stone remains of creatures nobody believes ever lived.

## Layout

| Path | Purpose |
|------|---------|
| `content/` | The wiki itself. Open this folder in Obsidian as a vault. |
| `content/_meta/` | Unpublished working notes: templates, art direction, shot list, map list, open questions. |
| `content/attachments/` | Published art (black-and-white ink style) and finished map previews. |
| `maps/` | Map work in progress (Dungeondraft / Wonderdraft). Never published. |
| `quartz/`, `quartz.config.ts`, `quartz.layout.ts` | [Quartz 4](https://quartz.jzhao.xyz/) site generator and configuration. |

## Working locally

```sh
npm ci
npx quartz build --serve   # preview at http://localhost:8080
```

Pushing to `main` deploys to GitHub Pages via `.github/workflows/deploy.yml`.

## Conventions

- Every page uses a template from `content/_meta/Templates/` and carries `type` and `status` frontmatter.
- GM-only secrets live in collapsed `> [!secret]- GM Only` callouts.
- Unresolved gaps are marked `> [!todo]` and collected in `content/_meta/Open Questions.md`.
- Map placeholders use `> [!map]` until a finished map exists.

## License

Copyright © 2026 Thomas Davis. All rights reserved. See `LICENSE`.

The Quartz engine is MIT licensed and is not covered by that notice. See `LICENSE-QUARTZ.txt`.
