# ONESecure — Design System

> **ONESecure** is a Brazilian **Workspace Security Platform** that integrates
> continuous monitoring, threat intelligence and automated response into a single
> environment. The 2026 rebrand reframes cybersecurity from a *tool* into a
> *continuous management process* — connecting protection, governance and
> operational efficiency.
>
> _Tagline (PT-BR):_ **"Segurança como sistema. Gestão como padrão."**
> ("Security as a system. Management as the standard.")

---

## Source material

Reconstructed from a single Figma file the user attached: **`ONESecure.fig`**.

| Page | Frames | Purpose |
|---|---|---|
| `BRAND-BOOK` | 35 | Brand bible — vision, positioning, principles, logo, colour, type |
| `APRESENTACAO` | 28 | Sales / pitch deck templates |
| `SOCIAL-MEDIA` | 14 | Instagram + LinkedIn posts and Stories |
| `WALLPAPER-BACKGROUNDS` | 18 | Desktop + meeting wallpapers |
| `DOCUMENTOS` | 4 | Document covers |
| `EMAIL-MKT` | 4 | Email marketing |
| `Thumb` | 1 | File cover |

No production codebase or live website was attached. This system is therefore
**brand-led**, not product-led: any UI surfaces in `slides/` are recreated
from the brand book and presentation deck, not from running code.

---

## Company at a glance

- **Name:** ONESecure
- **Domain:** `onesecure.com.br`
- **Language:** Brazilian Portuguese (all native copy)
- **Sector:** Cybersecurity — B2B / Enterprise
- **Product:** Workspace Security Platform (WSP)
- **Brand epoch:** Brand Guidelines March 2026 (post-repositioning)
- **Positioning shift:**
  - *From:* modular offer, complex comms, low differentiation, commercial dependency
  - *To:* integrated security **management**, clarity for decision-makers, scale, authority

### Brand architecture — two complementary lines

| Line | Tone | Sub-marks |
| --- | --- | --- |
| **Institutional** *(~80% of touchpoints)* | Credibility, authority, decision-makers | `Corporate`, `Enterprise` |
| **Experiential**  *(~20%)* | Engagement, proximity, memorability | `Comunidade`, `Suri`, `Eventos` |

Both lines share one logo, one type system, one primary palette. They diverge
only in **tone**, **support-color usage**, and **shape rhythm**.

---

## ✦ Content fundamentals

### Voice — Institutional line

> *Linguagem clara, objetiva e técnica, sempre orientada a negócio.*

- Clear, objective, technical, business-oriented.
- Lead with outcomes: governance, decision-making, financial protection.
- First-person plural ("organizamos, estruturamos, sustentamos, protegemos").
- Avoid excess, superficial simplifications, or promotional tone.

### Voice — Experiential line

> *Linguagem mais próxima, dinâmica e acessível, mantendo clareza.*

- Warmer, more rhythmic, still smart. Engaging but never casual.
- Heavier use of support colors and motion.

### Casing & rhythm

- **Tags & CTAs are ALL-CAPS**, Lexend Regular, tracked `+0.08em`.
  Examples: `CALL TO ACTION`, `MARÇO`, `2026`, `ONESECURE.COM.BR`.
- Page chips read mixed-case in an uppercase frame: `Introdução`, `Cores`, `Tipografia`.
- Headlines are **sentence case**, terminated with a period for cadence:
  *"Mudança estratégica."*, *"Construindo uma plataforma de confiança, escala e crescimento."*
- Body retains formal PT-BR punctuation: em-dashes `—`, accented vowels.

### Verbatim examples from the brand book

- *"Estruturando segurança como sistema contínuo"*
- *"A segurança passa a operar como um processo contínuo de gestão."*
- *"A ONESecure evolui com o ambiente, sustenta a maturidade e transforma segurança em processo contínuo."*
- Principle pairs (declarative, twin-line):
  - **Segurança como sistema.** *"Segurança não é evento. É operação."*
  - **Integração real.** *"Ferramentas isoladas não resolvem. Conectamos, organizamos e damos contexto."*
  - **Segurança que acompanha o negócio.** *"Se não acompanha a operação, não serve."*
  - **Evolução com maturidade.** *"Evoluímos com direção."*

### Vocabulary do / don't

| Use | Don't use |
| --- | --- |
| Plataforma | Solução, ferramenta, software |
| Gestão de segurança | "Cyberdefense", proteção genérica |
| Operação contínua | "Always-on", "24/7" |
| Governança | Compliance (only when literal) |
| Maturidade | Crescimento, escalada |
| Resposta automatizada | Auto-resposta, robô |

### Vibe

Confident, institutional, blue-suit — with a warm humanist rhythm in the
headlines. **No emoji. No exclamation marks. No ALL CAPS in body. No hype.**

---

## ✦ Visual foundations

### Color

The system is **monochromatic blue by design**. One royal flagship (`#0132A5`)
and one deep indigo (`#211941`) carry 80%+ of every layout. Support colors
(mint, violet, yellow) belong to the experiential line only.

| Token | Hex | Role |
| --- | --- | --- |
| `--os-primary` | `#0132A5` | Royal blue — buttons, brand mark, cover slides |
| `--os-primary-dark` | `#211941` | Deep indigo — section dividers, contrast slides |
| `--os-primary-bright` | `#3280EF` | Bright accent — logo gradient, links |
| `--os-blue-050` | `#E6EDFF` | **Default light page background** |
| `--os-blue-100` | `#EAF0FF` | Light tints, hairline blocks |
| `--os-mint` | `#BDFCE3` | Support — confirmation accents |
| `--os-violet` | `#934DEC` | Support — community / Suri persona |
| `--os-yellow` | `#EEF274` | Support — events |

**Rule:** an institutional layout that introduces yellow or violet has broken
the system. White and royal blue are always allowed; everything else is
contextual.

### Typography

**Lexend, exclusively** (variable font, weights 300–700 in active use).
The user uploaded `fonts/Lexend-VariableFont_wght.ttf`; `colors_and_type.css`
serves it locally via `@font-face`.

- `300 Light` — long-form body on slides (`30 px`+)
- `400 Regular` — UI body, tags, captions
- `700 Bold` — every headline, the wordmark

The METADATA also flags a single stray *League Gothic* glyph and a few *Inter*
runs in the source file. Treat those as **legacy / accidental** — do not
reintroduce them.

Type ramp lives in `colors_and_type.css` (`--os-display-1` → `--os-caption`).
Sizes are calibrated to a **1920 × 1080** artboard; downscale ~0.6 for UI.

### Layout & rhythm

- **1920 × 1080** is the canonical artboard for slides, wallpapers, banners.
  Posts use 1080² (square) or 1080×1920 (story).
- **64-px outer gutters** with a 176-px header band carrying two pill chips
  (left: section name, right: `BRAND GUIDELINES`).
- Three radii: **32 px** for cards & heroes, **16 px** for buttons/badges,
  **999 px** for round chips and logo wells.
- An 8-pt grid drives spacing (`--os-s-1` … `--os-s-9`).

### Backgrounds — five canonical recipes

| Mode | When | Recipe |
| --- | --- | --- |
| **Light page**  | Default content slides | `#E6EDFF` + two giant white circles (~1393 px, opacity 0.6) bleeding off-canvas at opposing 45° |
| **Royal cover** | Title slides, posters | `#0132A5` solid + halftone world map PNG at `mix-blend-mode: screen` |
| **Deep cover**  | Section dividers | `#211941` solid + radial gradient toward `#5540A7` + grain PNG at `mix-blend-mode: overlay` |
| **Mint accent** | Single-statement slides | Light page + one mint circle (`#BDFCE3`) replacing one white |
| **Wallpaper**   | Desktop / Teams backgrounds | Royal blue + bold curved sweep + halftone bleed |

All large background circles are **soft-blurred** (`filter: blur(80px)` or via
Figma "Layer blur") and always bleed off-canvas — never centered, never sharp.

### Motion

The brand book is static, but two motifs imply motion:

- **Soft, opacity-led fades** for slide transitions (no slide-from-side).
- **Halftone & grain** layers suggest **subtle film grain** — never animated,
  never jittered.
- Hover: lighten/darken by ~10% — *not* outline. Buttons darken to `#002A8C`.
- Press: 1 px down + faster easing (`120ms ease`).
- Use easing `cubic-bezier(.22,.61,.36,1)` (institutional-confident, not bouncy).

### Borders, shadows, transparency

- **Borders are rare.** When used, they are 1-px `rgba(103,148,254,.20)` — the
  "blue rain" stroke. Only on dividers between cards on royal blue.
- **Shadows are restrained.** Two recipes:
  - `--os-shadow-pill: 0 4px 8px rgba(0,0,0,.20)` for chips & buttons.
  - `--os-shadow-card: 0 8px 24px rgba(33,25,65,.12)` for elevated cards.
- **Transparency** is a primary tool: `.40` for glass cards on royal blue,
  `.10` for tinted-blue inset wells, `.20` for stronger tinted blocks.
- **Blur** is for *atmosphere* (the giant circles), not for chrome. Avoid
  glassmorphism in UI surfaces.

### The mascot

ONESecure's most distinctive visual element is its **escudo-mascote** — a stylized
ermine/quokka rendered in three-dimensional chrome-blue on a heraldic shield.
It sits **above** or **to the left** of the wordmark in every lockup. The
mascot:

- Carries the brand's authority + warmth duality on its own — security (shield)
  + observance (alert animal). Never split it from the brand without reason.
- Has its own card in `preview/` (`brand-mascot.html`) for use as a standalone
  symbol — favicons, app icons, social avatars.
- **Never recolor it.** The metallic blue gradient is part of the identity.
- Minimum size: **40 px** for the mark alone, **120 px** for the horizontal
  lockup, **160 px** for the principal vertical lockup.

### Imagery vibe

- Color photography is treated **flat, slightly cool, no warm grain**.
- Bug-eye people shots get a **royal-blue tint overlay** at ~30% opacity in
  cover compositions.
- Halftone world map and grain are **textures**, not photos — used at
  `mix-blend-mode: screen` or `overlay`.

### Cards & containers

- 32-px radius, no border, optional `--os-shadow-card`.
- On royal blue: **glassy** — `background: rgba(255,255,255,.40)`.
- On indigo: **tinted** — `background: rgba(50,128,239,.10)`.
- On light page: **solid white** or `--os-blue-100`.

---

## ✦ Iconography

The Figma file does **not** ship a system icon set. Only a handful of glyphs
appear, always as inline SVG strokes:

- **`check.svg`** — checkmark used for principle bullets and feature lists
  (copied to `assets/icons/check.svg`).
- **`verified_user.svg`** — Material-style shield used once in the LinkedIn
  banner (copied to `assets/icons/verified-user.svg`).
- **`exclamation.svg`** — accent glyph from Frame 105 (copied).

Otherwise, **no icon font and no consistent icon system is defined.** When
icons are needed for new work, **substitute Material Symbols (rounded,
weight 300)** — same humanist proportions as Lexend — and flag the
substitution to the brand owner.

**Never use emoji.** **Never use unicode dingbats.** When in doubt, omit.

The "shield" form factor recurs as a visual motif (the `verified-user` glyph,
the swoosh on the LinkedIn banner) — keep this in mind when picking a
substitute icon for a security action.

---

## Repository index

| Path | What's in it |
| --- | --- |
| `README.md` | This file |
| `SKILL.md` | Agent SKILL definition — drop-in for Claude Code |
| `colors_and_type.css` | All design tokens (colors, type, radii, spacing, shadows) + base semantic styles |
| `fonts/` | Lexend variable font (brand-provided) |
| `assets/logo/` | Official ONESecure logo system — horizontal & vertical lockups (positive + negative), wordmark-only, and isolated mascot/shield symbol |
| `assets/textures/` | World halftone, grain overlay |
| `assets/icons/` | The three native icons used in the brand book |
| `assets/shapes/` | Swoosh / curve used in social-media compositions |
| `preview/` | Design-system card files surfaced in the Design System tab |
| `slides/` | Recreations of the pitch-deck templates |
| `ui_kits/` | _Not built_ — no product UI was provided. See Caveats below. |

---

## Caveats

- **No production codebase or website** was attached, so no UI kit was built.
  Any future feature/screen designs should be created from the slide templates
  in `slides/` plus the tokens here.
- **Icon system is undefined** in the brand. Material Symbols Rounded is a
  reasonable default until ONESecure commits to one.
- The brand book references `Inter` and `League Gothic` for legacy fragments —
  the design system **drops** both in favour of Lexend everywhere.
- All copy is **Brazilian Portuguese**; translate carefully (formal register,
  no false cognates with European Portuguese).
