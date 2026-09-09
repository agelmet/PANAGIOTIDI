# ginapanagiotidi.gr — brand & art notes (9 Sept 2026)

## Palette (taken from her logo)
| token | hex | use |
|---|---|---|
| `lux-primary` | `#0F4A55` | deep teal — headings accent, buttons, links |
| `lux-accent`  | `#1B6A78` | mid teal — secondary emphasis |
| `lux-dark`    | `#13272C` | body copy |
| `lux-clay`    | `#7D5C28` | gold, dark enough for small text (AA) |
| `lux-gold`    | `#A47D45` | gold for icons and rules (3:1) |
| `lux-glow`    | `#C9A96A` | light gold, dark grounds only |
| `lux-deep`    | `#0B373F` | footer ground |
| `lux-light`   | `#F7F1E8` | paper |
| `lux-cream`   | `#EDE2D3` | banded sections |
| `lux-sand`    | `#DDD0BC` | borders |

## art/
Logo files are cut from the client's own artwork (transparent WebP).
Everything else is original texture generated for this site — watercolour
washes, bristle brush drags and canvas grain in the palette above. They are
decorative only and sit at 8–34% opacity behind the content.

- `logo.webp` — full lockup, teal + gold, for light grounds
- `logo-cream.webp` — cream wordmark + gold mark, for the dark footer
- `mark-gold.webp` — the lighthouse alone, watermark
- `wash-teal / wash-gold / wash-clay` — watercolour blooms
- `stroke-teal / stroke-gold / band-teal` — brush drags
- `canvas-grain.webp` — 256px tile, whole-page paper tooth
- `favicon.png`, `apple-touch-icon.png`, `doctoranytime.jpg`, `instagram.webp`

The brush / palette / paint-tube / jar drawings are inline SVG `<symbol>`s at
the top of `<body>` (`#ico-brush`, `#ico-palette`, `#ico-tube`, `#ico-jar`),
placed with `.art-line`. Hairline gold, same drawing language as the
lighthouse in the logo.

## Rules for future edits
- Keep the whole page on the tokens above; no colour outside the logo family.
- Art layers go in `.art` / `.art-line` divs inside a `relative overflow-hidden`
  section, never in the content flow.
- `.art-xl` layers are hidden under 640px; art opacity drops on small screens.
- Nothing external is hotlinked any more — every asset is in this repo.
