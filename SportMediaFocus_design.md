# Sport Media Focus — Brand & Visual Design Guide

> Research based on direct inspection of sportmediafocus.com (CSS, computed styles, page screenshots), LinkedIn presence, and their sub-project materials. Last reviewed: April 2026.

---

## Brand Essence

Sport Media Focus positions itself as a serious, premium sports marketing agency — not a fan brand. Their tone is **professional authority with athletic energy**. Visual language leans toward deep teal/navy sophistication broken by high-impact photography. The brand communicates experience (since 1997, 25+ years) and international scale while staying distinctly Slovenian.

Core tagline positioning: *"Communication in Sports"*

---

## Color Palette

All values extracted directly from the site's CSS variables and computed styles.

### Primary Colors

| Role | Name | Hex | RGB | Notes |
|------|------|-----|-----|-------|
| Brand Primary | Deep Teal | `#005F7E` | `rgb(0, 95, 126)` | Dominant accent — buttons, links, labels, footer bg |
| Brand Dark | Midnight Navy | `#013150` | `rgb(1, 49, 80)` | Headings on light bg (h2, h3) |
| Brand Darker | Dark Slate | `#1e293b` | `rgb(30, 41, 59)` | Elementor global color-2, dark sections |

### Secondary & Accent Colors

| Role | Name | Hex | Notes |
|------|------|-----|-------|
| Accent Blue | Electric Blue | `#060097` | Elementor global color-0; used sparingly for emphasis |
| Accent Yellow | Golden Yellow | `#FFCD57` | Elementor global color-7; warm highlight, CTAs |
| Muted Blue-Gray | Body Text | `#67768e` | `rgb(103, 118, 142)` — primary body text color |
| Mid Gray | Secondary Text | `#7a7a7a` | Supporting copy, captions |
| Dark Text | Near-Black | `#333333` | `rgb(51, 51, 51)` |

### Background & Surface Colors

| Role | Hex | Notes |
|------|-----|-------|
| Page Background | `#FFFFFF` | White base |
| Light Surface | `#F9F9F9` | Off-white sections |
| Light Gray | `#F2F5F7` | Card backgrounds, subtle dividers |
| Pale Lavender | `#F9F6FE` | Rare accent surface |
| Teal Overlay | `rgba(0, 95, 126, 0.8)` | Used over hero images |
| Footer BG | `#005F7E` | Full teal footer |

### Color Behavior

- **Hero sections**: Full-bleed sports photography with a dark teal overlay (`rgba(0,95,126,0.8)` or near-black) — white text on top.
- **Content sections**: White or `#F9F9F9` background, teal (`#005F7E`) for accent text, navy (`#013150`) for headings.
- **Section alternation**: Dark-bg hero → light content → dark-bg → light content. High contrast rhythm throughout.
- **The footer** is always solid teal (`#005F7E`) with white type — a strong bookend.
- **Social/share buttons**: Square teal blocks with white icons.
- **Uppercase all-caps accent labels** (e.g. "ABOUT US", "SEE SOME OF OUR PROJECTS") are rendered in teal, small caps, with a short underline rule beneath.

---

## Typography

### Typefaces

| Role | Font | Fallback |
|------|------|---------|
| **Primary (everything)** | **Montserrat** | Helvetica Neue, sans-serif |
| Body secondary | DM Sans | sans-serif |
| Code/mono (rarely) | Courier 10 Pitch | Courier, monospace |

Montserrat is the dominant font across all headings, body, nav, and UI. DM Sans appears in some Elementor widget blocks. **No serif typefaces are used.**

### Type Scale & Weights

| Element | Size | Weight | Transform | Notes |
|---------|------|--------|-----------|-------|
| Hero mega-heading | ~80–100px | 700–800 | Uppercase | e.g., "CONNECT", "We are Sport Media Focus" |
| H2 (section titles) | 48px | 700 | Sentence case | Teal or navy |
| H3 (sub-section) | ~28–32px | 700 | Sentence case | |
| Accent label | ~12–14px | 700 | **ALL CAPS** | Teal, letter-spaced, with underline rule |
| Body text | ~16.4px | 400 | Normal | `#67768e`, line-height ~1.85 |
| Nav items | ~16px | 400–500 | Sentence case | White (on dark) or dark |
| Footer text | ~14–16px | 400 | Normal | White on teal |

### Type Personality Notes

- Heavy use of **weight contrast**: ultra-bold display headings paired with light-weight body text.
- Uppercase all-caps is reserved for **short labels and category tags**, not long headings.
- Some hero overlays use **condensed, tracking-tight caps** (e.g. the project card titles like "GAME GANG SHOW", "SPORTO — SPORTS MARKETING CONFERENCE") — almost editorial.

---

## Logo

### Description

The logo is a **wordmark only** — no icon, no emblem. Three stacked lines of text:

```
Sport
Media
Focus
```

- Set in **Montserrat Bold** (or close variant), white on dark backgrounds.
- Left-aligned, stacked vertically — compact, blocky, strong.
- Used exclusively in **white** against dark/teal/image backgrounds.
- No dark version observed in use; the logo lives on dark surfaces.
- Top-left placement in the header, relatively small (approx 80–100px tall block).

The hamburger menu (three-line icon) sits top-right in a **white square box**, creating a strong rectangular contrast element against the hero image.

---

## Layout & Composition

### Grid & Spacing

- **Max content width**: 1200px (`--ast-normal-container-width: 1200px`)
- **Narrow content**: 750px (`--ast-narrow-container-width: 750px`)
- **Section padding**: 2.4em (mobile) to 3em (desktop)
- Mobile-first responsive, Elementor page builder framework

### Section Structure Pattern

The homepage follows a deliberate rhythm:

1. **Full-bleed video/image hero** — cycling imagery (sport action, VR, basketball, handball) with large overlaid typography. Dark overlay, white text.
2. **Social media cards strip** — tiled Instagram-card style layout showing active sports content.
3. **"We are Sport Media Focus"** — light section, left-aligned body copy, teal accent heading.
4. **Service category blocks** — alternating dark/light full-width image sections, each with: category label + bold heading + body copy + client list in teal all-caps.
5. **Stats callout** — large bold text ("More than 25 years of experience...") in teal on off-white.
6. **Client logo strip** — horizontal scroll/carousel of partner brand logos.
7. **Project thumbnail grid** — image cards with overlaid white text (project name + category label).
8. **Full teal footer** — logo, nav links, full contact/legal details, all white.

### Image Treatment

- **Hero photography**: high-action sports photography (crowd events, athletes mid-play, conference speakers). Always full-width.
- **Dark teal overlay** on most imagery — creates brand-consistent color wash.
- **Project cards**: rectangular image thumbnails with title overlay on hover/always-visible white text.
- **No illustrations or icons** (beyond FontAwesome social icons).
- **Instagram card mockups** on homepage — framed social posts shown in device-like rounded cards.

---

## UI Components & Patterns

### Buttons / CTAs

- No pill shapes — buttons tend to be **rectangular or lightly rounded**.
- Background: teal (`#005F7E`) — white text.
- Social sharing buttons: solid teal squares with white platform icons (LinkedIn, Facebook, Twitter).
- Cookie banner "Save" button: full-width teal rounded rectangle.

### Navigation

- **Full-screen overlay nav** — hamburger triggers a full-page menu with large centered navigation links.
- Nav is minimal on-screen: only logo (top-left) + hamburger (top-right white box).
- Navigation links in the overlay are large, white, center-aligned.

### Section Accent Elements

- Short **horizontal teal underline** rule beneath uppercase category labels.
- Teal bullet separators between listed items (e.g., "EUROBASKET 2013 • UEFA FUTSAL EURO 2018 • ...").
- **Two-weight heading trick**: e.g., "More than **25 years of experience**" — regular weight intro + bold teal callout.

### Dividers

- Color-block section changes serve as visual dividers rather than rules or borders.
- Thin horizontal line separates some content areas.

---

## Tone & Communication Style

- **Confident, authoritative**: "We are unstoppable in ensuring quality..."
- **Experience-forward**: numbers featured prominently (25+ years, 60+ clients, 150+ projects).
- **Pan-European ambition**: highlights international events (FIVB, EHF, UEFA, NBA).
- **B2B language**: clients, partners, sponsorship activations — not fan-facing.
- No playful or casual visual elements — this is agency-to-brand communication.

---

## Must-Have Visuals (For Any SMF Project)

These are the visual assets and references that are *essential* to match or align with the Sport Media Focus identity:

### 1. The Logo (Wordmark)
- White stacked Montserrat wordmark: "Sport / Media / Focus"
- Always on dark or teal backgrounds. Request or recreate exactly.
- **Source**: Top-left of every page on sportmediafocus.com

### 2. The Teal Color `#005F7E`
- The single most identifying brand color. Every design must use this prominently.
- It appears as: footer bg, button fill, link color, accent label color, overlay wash.

### 3. High-Action Sports Photography with Teal Overlay
- Their entire visual identity is built on this pattern: athlete/event photo + `rgba(0,95,126,0.8)` dark teal overlay.
- Any design without this risks feeling off-brand.

### 4. Montserrat Bold at Large Scale
- The all-caps hero text ("CONNECT", section titles, project card labels) in Montserrat 700+ at large sizes is a signature visual pattern.
- Especially the uppercase tracking-tight card title style.

### 5. The Footer
- Full teal background, white Montserrat text, stacked logo top-left — this footer is visually iconic and immediately recognizable.

### 6. SPORTO Conference Branding
- The SPORTO conference is SMF's flagship sub-brand. If the project touches SPORTO, their visual identity includes: dark stadium imagery, bold white type, speaker/panel photography.
- Instagram: @sportoconference (470 followers, 255 posts)

### 7. Client Logo Strip
- SMF always displays their client/partner logos (Garmin, Fructal, Dallas Mavericks, NLB, Continental, etc.) in a horizontal carousel.
- Having the right client logos is essential for credibility visuals.

### 8. Stats in Bold Teal Type
- The "25+ years / 60+ clients / 150+ projects" stat block in large Montserrat Bold teal is a recurring element across the site and LinkedIn posts.

### 9. Project Card Grid Style
- Dark overlay image cards with white Montserrat Bold title + all-caps gray category label — this grid is the primary way projects are displayed.

### 10. Hamburger Menu Block (White Square on Dark)
- The white square enclosing the hamburger icon is an unusual, distinctive UI choice. On any reimagined navigation, this detail signals the brand.

---

## Summary: Brand Personality at a Glance

| Attribute | Value |
|-----------|-------|
| Color feel | Deep teal + navy. Professional, trustworthy, athletic. |
| Type feel | Heavy Montserrat. Bold, clean, no-nonsense. |
| Photo style | High-action sports. Dark overlays. No illustrations. |
| Layout | Full-bleed sections, alternating light/dark, generous whitespace. |
| Agency positioning | Premium B2B sports marketing. International scale. |
| National identity | Subtly Slovenian (Ljubljana Marathon, Luka Dončić, I Feel Slovenia) but internationally ambitioned. |
