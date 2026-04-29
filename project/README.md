# Syrus Construction Group — Design System

## Overview

Syrus Construction Group is a premium construction and development firm with 25+ years of industry experience. The brand conveys authority, precision, and understated luxury — a company that lets its portfolio speak for itself. The design system supports a **marketing website** covering Home, Services, Work, About Us, and Contact surfaces.

**Sources provided:**
- Logo PNG: `uploads/logo-1777413086528.png` (copied to `assets/logo-dark-bg.png`)
- Brand brief: Black, white, and grey palette; luxury/premium vibe; formal professional tone; sans-serif typography; Heroicons (medium stroke) icon system.

---

## CONTENT FUNDAMENTALS

**Tone:** Professional, formal, and authoritative. Syrus speaks with quiet confidence — never boastful, never casual. Copy is terse and declarative. No exclamation points. No emoji.

**Voice:** Third-person brand ("Syrus Construction Group delivers…") for institutional contexts; second-person for CTAs and direct addresses ("Your vision. Our expertise."). Never first-person plural unless quoting a team member.

**Casing:**
- Headlines: ALL CAPS (driven by Bebas Neue display font)
- Navigation, labels, tags: ALL CAPS, tracked wide
- Body copy: Sentence case
- CTAs: Title Case or ALL CAPS — never lowercase

**Copy patterns:**
- Short, punchy hero lines: "Built to Last." / "Precision at Every Scale."
- Subheads as one-line credentials: "25+ Years. 300+ Projects Delivered."
- Service descriptions: formal, benefit-led, ~2–3 sentences max
- No filler adjectives ("innovative," "cutting-edge," "world-class") — let specifics do the work

**Punctuation:** Em dashes (—) used for dramatic pauses. Oxford comma always. Periods at end of fragments for weight.

**Numbers:** Spelled out below ten in body copy; numerals for stats and specifications.

---

## VISUAL FOUNDATIONS

### Color
Strictly black, white, and grey — with warm **stone** (a muted warm off-white/greige) as a single restrained accent to add architectural warmth. No saturated colors.

- **Primary surfaces:** Deep black `#111111` (hero, nav, footer)
- **Secondary surfaces:** `#1a1a1a`, `#242424` (cards on dark)
- **Light sections:** Pure white `#ffffff`, near-white `#f5f5f5`
- **Grey scale:** Full 10-stop scale from `#3d3d3d` → `#ebebeb`
- **Stone accent:** `#ccc4bb` / `#b5aa9e` — used sparingly for borders, dividers, highlights on light sections

### Typography
**Display:** Bebas Neue — condensed, all-caps, architectural. Used for all H1–H3. Wide letter-spacing (0.06em–0.2em). Mirrors the geometric authority of the logo mark.

**Body:** DM Sans — clean, modern, humanist. Weights 300 (large body), 400 (body), 600 (UI labels). Warm and legible without being corporate.

**No italic display type.** DM Sans italic used only for pull quotes or testimonials.

**Type scale:** 11px → 144px. Display type is large and dominant; body text is restrained.

### Spacing
8px base grid. Major sections use 96–128px vertical padding. Component internal spacing uses 4/8/12/16/24/32px.

### Backgrounds
- Hero sections: Full-bleed black with the logo mark or project photography on dark overlay
- Content sections: Alternate between pure black and white — strong contrast shifts create visual rhythm
- No gradients. No textures. No patterns.
- Photography: B&W or desaturated project photography only. High-contrast, architectural.

### Borders & Radius
- **Zero border-radius** on all containers, cards, and buttons — sharp, structural geometry echoes construction precision
- Subtle `1px` hairline borders using `rgba(255,255,255,0.08)` on dark, `rgba(0,0,0,0.08)` on light

### Cards
- On dark: `#1a1a1a` fill, `1px` border `rgba(255,255,255,0.08)`, no shadow
- On light: white fill, `1px` border `rgba(0,0,0,0.10)`, subtle `box-shadow: 0 4px 16px rgba(0,0,0,0.08)`
- **No rounded corners**

### Animation & Transitions
- Fade-in on scroll (opacity + subtle translateY, 40px → 0)
- Duration: 280–450ms, `cubic-bezier(0.25, 0, 0, 1)` ease-out
- Hover states: opacity transitions, no color shifts
- No bounce, spring, or playful easing
- Button hover: slight background lightening or border reveal

### Hover & Press States
- Dark buttons: `rgba(255,255,255,0.08)` overlay on hover, slight darken on press
- Light buttons: `rgba(0,0,0,0.05)` overlay on hover
- Links: underline reveal on hover (no color change)
- Cards: `translateY(-2px)` on hover, no shadow change

### Imagery
- Desaturated / B&W architectural photography
- High contrast, dramatic lighting
- Full-bleed at section level
- Dark overlay (`rgba(0,0,0,0.5)`) when text sits over photography

### Iconography
Heroicons (medium stroke, 24px). See ICONOGRAPHY section below.

### Layout
- Max content width: 1280px
- Section gutter: 24px mobile, 48px desktop
- 12-column grid
- Fixed top navigation on scroll

---

## ICONOGRAPHY

**Icon system:** Heroicons v2 (outline / medium stroke, 24px × 24px).
- Loaded from CDN: `https://unpkg.com/heroicons` (or referenced as inline SVG)
- Stroke width: 1.5px (default outline set)
- Always `currentColor` — inherits text color
- No filled icons except for active/selected states where a filled variant is used

**No emoji.** No unicode substitution icons. No custom icon drawings.

**Common icons in use:**
- Navigation arrow: `arrow-right`, `arrow-long-right`
- Services: `wrench-screwdriver`, `building-office-2`, `cube`, `clipboard-document-check`
- Contact: `envelope`, `phone`, `map-pin`
- UI affordances: `chevron-down`, `bars-3`, `x-mark`, `plus`

**Logo assets:**
- `assets/logo-dark-bg.png` — white wordmark + mark on black (1050×600px)
- Extracted mark only: use as favicon / small lockup

---

## FILE INDEX

```
/
├── README.md                    ← This file
├── SKILL.md                     ← Agent skill descriptor
├── colors_and_type.css          ← All CSS tokens: colors, type, spacing, shadows
├── assets/
│   └── logo-dark-bg.png         ← Primary logo (white on black)
├── preview/
│   ├── colors-dark.html         ← Dark palette swatches
│   ├── colors-light.html        ← Light/grey palette swatches
│   ├── colors-semantic.html     ← Semantic color tokens
│   ├── type-display.html        ← Display (Bebas Neue) type scale
│   ├── type-body.html           ← Body (DM Sans) type scale
│   ├── type-labels.html         ← Label + caption styles
│   ├── spacing-tokens.html      ← Spacing scale
│   ├── borders-radii.html       ← Border styles and radius (sharp)
│   ├── shadows.html             ← Shadow / elevation system
│   ├── components-buttons.html  ← Button variants
│   ├── components-cards.html    ← Card variants
│   ├── components-nav.html      ← Navigation bar
│   ├── components-inputs.html   ← Form inputs
│   └── brand-logo.html          ← Logo lockups
└── ui_kits/
    └── marketing/
        ├── README.md
        └── index.html           ← Full marketing website prototype
```
