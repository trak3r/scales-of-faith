---
title: Art Direction
draft: true
---

The style guide for every illustration in Scales of Faith. The goal is one consistent set that looks like it came from a single old-school (OSR) or Shadowdark-style book.

## Style

- **Medium:** black ink on off-white paper. Woodcut and engraving feel, with crosshatched shading.
- **Palette:** pure black on paper white. No color, no gray washes, no gradients.
- **Line:** bold, confident outlines with consistent line weight across the set. Shading is built only from hatching, crosshatching and stippling.
- **Composition:** one clear subject with generous negative space. White or near-white edges so images blend into the page.
- **Mood:** grounded, folkloric and a little grim. The world is mundane, and the dragons are a whispered rumor, so stone dragons should look like weathered statues, not monsters.
- **Never:** text, lettering, captions, signatures, watermarks, borders or frames, color, photorealism, glossy digital painting, anime styling.

## Formats

| Use | Aspect ratio | Notes |
| --- | --- | --- |
| Page header (places, world, factions, history) | 16:9 | Wide establishing scene. |
| Portrait (people, creatures) | 3:4 | Head and shoulders or three-quarter figure. |
| Spot art (items, artifacts, symbols) | 1:1 | The object alone on blank paper. |

## Files

- Saved in `content/attachments/`, named after the subject in kebab-case: `the-sage.jpg`, `dragon-reef.jpg`. (The image generator outputs JPEG.)
- Each page sets `banner: <file>.jpg` in its frontmatter and embeds `![[<file>.jpg]]` as the first line of the body.
- **Spoiler art goes inside the secret.** If an image would reveal a GM-only secret (living dragons, the Stoning, the Order's mission), embed it as the first line *inside* the page's `> [!secret]- GM Only` callout instead of at the top of the page. These are marked "in secret" in the [[Shot List]].
- The site stylesheet multiplies images onto the parchment background in light mode and inverts them in dark mode, so pure black-and-white images work best.

## Prompt Recipe

Start every prompt with the style block, then describe the subject:

> Black ink illustration on off-white paper, old-school fantasy RPG book art, woodcut and engraving style, bold outlines, crosshatched shading, pure black and white, no color, no gray wash, no text, no border, generous white negative space.

Then add the subject, taken from the [[Shot List]]. Always pass the locked style reference as a reference image.

## Consistency

- **Locked style reference:** `content/_meta/style-reference.jpg` (unpublished). It's sample C of four tried, a classic 1980s module pen-and-ink look with crosshatching and stippling. The others were a bold woodcut, a fine engraving and a heavy-black linocut, which inverted badly in dark mode.
- Pass the style reference on every generation.
- The old notes' images are inspiration only. They are never used as generation references, and none are copied into this repository.
- Illustrations interpret the text. They don't establish canon. If an image contradicts a page, the page wins.

## Canon Constraints

- **Stone dragons** are weathered stone: lichen, moss, vines, coral, seaweed. One is obsidian ([[Lake of Fire]]).
- **Knights of the Order** wear black-enameled plate, never carry shields, and use two-handed weapons (claymore, warhammer, maul).
- **Living dragons** appear only as blurry silhouettes in [[The Plane of Dreams]], or in history scenes.
- **No dragon imagery should look like proof** in present-day scenes. Present-day "dragons" are statues, fakes, puppets or rumors.
