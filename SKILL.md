---
name: onesecure-design
description: Use this skill to generate well-branded interfaces and assets for ONESecure (a Brazilian Workspace Security Platform), either for production or throwaway prototypes / decks / mocks / social posts / wallpapers. Contains essential design guidelines, colors, type, fonts, assets, slide templates, and tone-of-voice rules for prototyping in PT-BR.
user-invocable: true
---

# ONESecure — brand kit

Read **README.md** first for the full brand bible (positioning, two-line
architecture, content fundamentals, visual foundations, iconography). Then
explore the other files in this skill:

| Path | What it gives you |
| --- | --- |
| `colors_and_type.css` | All design tokens — colors, type ramp, radii, spacing, shadows. Import this in any prototype or production code. |
| `fonts/Lexend-VariableFont_wght.ttf` | The brand font. Self-host it; do not load Lexend from a CDN. |
| `assets/logo/` | Wordmark (light + dark), tagline lock-up, mark-only. |
| `assets/textures/` | World halftone, grain overlay. Used at `mix-blend-mode: screen` / `overlay`. |
| `assets/icons/` | The three native icons (check, shield, exclamation). Substitute Material Symbols Rounded weight 300 if more icons are needed; flag the substitution. |
| `assets/shapes/` | Curved swoosh from the LinkedIn banner. |
| `preview/` | Stand-alone HTML cards for every token & component — copy patterns straight from these. |
| `slides/` | Working slide-deck shell (`index.html`) with 7 canonical slide types — cover, intro, statement, principles, color palette, dark section divider, closing. Use as a starting point for any pitch / brand / sales deck. |

## When invoked

If creating **visual artifacts** (slides, mocks, throwaway prototypes,
posters, social posts): copy the needed assets out of this skill, import
`colors_and_type.css`, and produce static HTML files for the user to view.

If working on **production code**: pull the design tokens from
`colors_and_type.css`, copy the brand assets you need, and treat the rules in
`README.md` (especially *Content Fundamentals* and *Visual Foundations*) as
non-negotiable.

If the user invokes the skill without further guidance, **ask what they want
to build** (deck / wallpaper / social post / web page / app screen), what
**audience** (institutional vs experiential — the tone diverges sharply), and
whether they want copy in **PT-BR (default)** or English. Then act as an
expert ONESecure designer.

## Hard rules

- **PT-BR by default.** Brazilian Portuguese punctuation, accents, em-dashes.
- **Lexend only.** Three weights: 300 / 400 / 700.
- **Royal blue + deep indigo** carry 80%+ of every layout. Support colors
  (mint, violet, yellow) only appear on the **experiential line**.
- **Tags & CTAs are UPPERCASE** with `letter-spacing: 0.08em`.
- Headlines are **sentence case** with a closing period. End-period rhythm
  is a brand signature: *"Mudança estratégica."*
- **No emoji. No exclamation marks. No marketing fluff.**
- Page chrome on every deck slide except true covers: two pill chips at top
  (left = section name, right = "Brand Guidelines"), wordmark bottom-left,
  URL bottom-right.
- Card radius **32 px**, button/pill radius **16 px**, full pill **999 px**.
- Backgrounds: light page (`#E6EDFF` + two soft white circles), royal cover
  (`#0132A5` + halftone screen), deep cover (`#211941` + radial violet +
  grain overlay). Always blurred, always bleeding off-canvas.

See `README.md` § Visual Foundations for the complete recipe set.
