---
title: Frontmatter Schema
draft: true
---

Every published page starts with this frontmatter.

```yaml
---
title: The Sage
type: person          # see types below
status: partial       # complete | partial | stub
chapter: 1            # adventures and events only; omit if unplaced
aliases: []           # alternate names; also used for link redirects
banner: the-sage.png  # optional header art in attachments/
tags: []              # optional free-form tags (region, faction, theme)
---
```

## Types

| type | used for | template |
| --- | --- | --- |
| `lore` | world, history, cosmology, introduction pages | (free-form) |
| `faction` | organizations and groups | [[Faction Template]] |
| `place` | settlements, businesses, sites, regions | [[Place Template]] |
| `person` | named NPCs | [[Person Template]] |
| `adventure` | playable scenarios (main or side quest) | [[Adventure Template]] |
| `event` | timed happenings in or around town | [[Event Template]] |
| `encounter` | short road or random encounters | [[Adventure Template]] (trimmed) |
| `creature` | bestiary entries | [[Creature Template]] |
| `item` / `artifact` | magic items and plot artifacts | [[Item Template]] |
| `spell` | spells and prayers | [[Spell Template]] |
| `index` | section landing pages and lists | (free-form) |

## Status

- **complete**: ready to run as written.
- **partial**: usable, but has `> [!todo]` gaps.
- **stub**: an idea with little detail; needs work before play.

## Callouts

```markdown
> [!secret]- GM Only
> Hidden truth, collapsed by default.

> [!prep]
> **Maps**: ... **Tokens**: ...

> [!todo]
> An open question or missing piece. Also list it in [[Open Questions]].

> [!map] Map placeholder: Name
> Battle map / region map, Dungeondraft. See `maps/<slug>/`.
```

## Art

`banner` names a file in `content/attachments/`. Embed it as the first line of the body: `![[the-sage.png]]`. Quartz reserves the `image` field for social previews, so don't use `image` here.
