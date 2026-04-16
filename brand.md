# NDUM Brand Guidelines

> Nexus of Digitized and Unified Markets

This document defines the visual identity, tone, and design system for all NDUM projects. Reference this file to ensure consistency across repositories, publications, presentations, and external communications.

---

## 1. Name & Identity

| Element | Value |
|---------|-------|
| Full name | Nexus of Digitized and Unified Markets |
| Short name | NDUM |
| Entity | NDUM Research Center |
| Domain | ndum.org |
| Pronunciation | "N-dum" (individual letters N-D, then "um") |

**Usage rules:**
- "NDUM" is always uppercase in running text
- First reference in a document should include the full name: "NDUM (Nexus of Digitized and Unified Markets)"
- Do not stylize as "Ndum", "ndum", or "N.D.U.M."

---

## 2. Logo

The NDUM logo consists of two mirrored pairs of vertical panels — one silver/gray, one royal blue — with a luminous glow effect on a dark background. The panels suggest parallel structures converging, representing the nexus of digitized and traditional markets.

**Logo files:**
- `logo.png` — Primary logo (dark background, with glow)
- Use on dark or neutral backgrounds only
- Minimum clear space: equal to the height of one panel on all sides

**Do not:**
- Place the logo on busy or light backgrounds without a dark container
- Rotate, stretch, or recolor the logo
- Add drop shadows or effects beyond the built-in glow
- Use below 32px height for digital or 0.5in for print

---

## 3. Color Palette

### Primary Brand Colors

| Name | Hex | RGB | Usage |
|------|-----|-----|-------|
| NDUM Blue | `#4361EE` | 67, 97, 238 | Primary accent, links, buttons, highlights |
| NDUM Blue Light | `#6580F5` | 101, 128, 245 | Hover states, dark mode primary, gradients |
| NDUM Blue Dark | `#2F4ABF` | 47, 74, 191 | Active states, pressed buttons, emphasis |

### Neutral Palette

| Name | Hex | RGB | Usage |
|------|-----|-----|-------|
| Text Primary | `#1E293B` | 30, 41, 59 | Headings, body text |
| Text Secondary | `#475569` | 71, 85, 105 | Captions, descriptions, metadata |
| Slate | `#64748B` | 100, 116, 139 | Tertiary text, icons |
| Border | `#CBD5E1` | 203, 213, 225 | Dividers, card borders |
| Surface | `#F1F5F9` | 241, 245, 249 | Page backgrounds |
| Surface Elevated | `#FFFFFF` | 255, 255, 255 | Cards, modals, elevated containers |
| Gray Blue | `#E8ECF4` | 232, 236, 244 | Alternate backgrounds, code blocks |

### Dark Mode Palette

| Name | Hex | RGB | Usage |
|------|-----|-----|-------|
| Background | `#0F1720` | 15, 23, 32 | Page background |
| Surface | `#141C27` | 20, 28, 39 | Recessed areas |
| Surface Elevated | `#1E2A3A` | 30, 42, 58 | Cards, modals |
| Text Primary | `#E2E8F0` | 226, 232, 240 | Headings, body text |
| Text Secondary | `#94A3B8` | 148, 163, 184 | Captions, metadata |
| Border | `#334155` | 51, 65, 85 | Dividers, card borders |
| Blue Primary | `#6580F5` | 101, 128, 245 | Accent (brighter for contrast) |
| Glow | `rgba(101, 128, 245, 0.2)` | — | Hover shadows, emphasis |

### Functional Colors

| Name | Hex | Usage |
|------|-----|-------|
| Blue Glow (light) | `rgba(67, 97, 238, 0.15)` | Card hover shadows, icon backgrounds |
| Blue Glow (dark) | `rgba(101, 128, 245, 0.20)` | Card hover shadows in dark mode |
| Blue Soft | `rgba(67, 97, 238, 0.12)` | Badge backgrounds, tag fills |

### Color as CSS Variables

```css
:root {
  --ndum-blue: #4361ee;
  --ndum-blue-light: #6580f5;
  --ndum-blue-dark: #2f4abf;
  --ndum-gray-blue: #e8ecf4;
  --ndum-slate: #64748b;
  --ndum-surface: #f1f5f9;
  --ndum-surface-elevated: #ffffff;
  --ndum-text-primary: #1e293b;
  --ndum-text-secondary: #475569;
  --ndum-border: #cbd5e1;
  --ndum-glow: rgba(67, 97, 238, 0.15);
}
```

---

## 4. Typography

### Font Stack

| Role | Font | Fallback | Weight |
|------|------|----------|--------|
| Headings (serif) | Georgia | Times New Roman, serif | 700 |
| Body (sans-serif) | System UI stack | -apple-system, Segoe UI, sans-serif | 400, 500, 600 |
| Code / Data | JetBrains Mono | Menlo, Consolas, monospace | 400, 500 |

### Type Scale

| Element | Size | Weight | Line Height | Letter Spacing |
|---------|------|--------|-------------|----------------|
| H1 (page title) | 2.5rem (40px) | 700 | 1.15 | -0.02em |
| H2 (section title) | 1.75rem (28px) | 700 | 1.2 | 0 |
| H3 (card/subsection) | 1.05–1.25rem | 600 | 1.3 | 0 |
| Body | 1rem (16px) | 400 | 1.7 | 0 |
| Small / Captions | 0.85rem (13.6px) | 500 | 1.5 | 0 |
| Section Label | 0.8rem (12.8px) | 600 | 1 | 1.5px |
| Tag / Badge | 0.75rem (12px) | 500-600 | 1 | 0.5px |

### Conventions

- Page titles use **serif** (Georgia) for academic authority
- Body text and UI use **system sans-serif** for readability
- Data, code snippets, and episode numbers use **monospace**
- Section labels are **uppercase, tracked wide** (letter-spacing: 1.5px), colored `--ndum-blue`

---

## 5. Component Patterns

### Cards

```
Border:         1px solid var(--ndum-border)
Border radius:  12px (standard), 16px (featured/CTA), 24px (newsletter)
Background:     var(--ndum-surface-elevated)
Padding:        24-32px
Hover:          border-color shifts to rgba(67, 97, 238, 0.4)
                box-shadow: 0 8px 30px var(--ndum-glow)
                transform: translateY(-2px)
```

### Buttons

**Primary:**
```
Background:     var(--ndum-blue)
Color:          #FFFFFF
Border radius:  8px
Padding:        12px 28px
Hover:          background darkens to var(--ndum-blue-dark)
                box-shadow: 0 4px 14px rgba(67, 97, 238, 0.35)
```

**Outline:**
```
Background:     var(--ndum-surface-elevated)
Color:          var(--ndum-text-primary)
Border:         1px solid var(--ndum-border)
Border radius:  8px
Hover:          border-color and text-color shift to var(--ndum-blue)
```

### Tags / Badges

```
Background:     var(--ndum-glow) or surface-soft
Border radius:  999px (pill)
Padding:        2-4px 10-12px
Font size:      0.75-0.8rem
Font weight:    500-600
```

### Section Headers

```
Label:          0.8rem, uppercase, letter-spacing 1.5px, color: var(--ndum-blue)
Title:          serif, 1.75-2.25rem, font-weight 700
Description:    1rem, color: var(--ndum-text-secondary), max-width 560-640px
```

---

## 6. Iconography

- **Style**: Outline/stroke icons (not filled)
- **Stroke width**: 1.5–2px
- **Size**: 16px (inline), 20px (cards), 24-28px (features), 40px (CTAs)
- **Color**: `var(--ndum-blue)` for accents, `var(--ndum-text-secondary)` for neutral
- **Source**: Lucide Icons (preferred) or equivalent open-source stroke icon set

---

## 7. Spacing & Layout

| Token | Value | Usage |
|-------|-------|-------|
| Container max-width | 1200px | Page content wrapper |
| Section padding | 96px vertical | Between major sections |
| Card gap | 16–24px | Grid spacing |
| Content max-width | 640–720px | Prose/paragraph blocks |

### Grid Patterns

- **3-column**: Feature cards, datasets, tools
- **2-column**: Research areas, team cards, mission + stats
- **2/3 + 1/3**: Blog + sidebar, featured research
- Responsive: collapse to single column at 768px

---

## 8. Motion & Interaction

| Property | Value |
|----------|-------|
| Default transition | 0.2s ease |
| Card hover lift | translateY(-2px) |
| Button hover lift | translateY(-1px) |
| Link arrow slide | translateX(4px) on hover |
| Glow pulse | 3s ease-in-out infinite (hero badge dot) |
| Flowing lines | 3s ease-in-out infinite pulse opacity |

**Rules:**
- Transitions apply to color, background-color, border-color, transform, box-shadow
- No motion on page load — interactions only
- Respect `prefers-reduced-motion` for accessibility

---

## 9. Voice & Tone

### Writing Style

| Attribute | Guideline |
|-----------|-----------|
| Register | Academic but accessible — think working paper abstract, not textbook |
| Sentence length | Vary. Short for impact. Longer for nuance. |
| Jargon | Use precise financial/technical terms, but define on first use |
| Point of view | First person plural ("our research", "we examine") in institutional context; third person for formal publications |
| Tense | Present tense for descriptions ("This paper examines..."), past for findings ("Results indicated...") |

### Content Hierarchy

| Format | Tone | Length |
|--------|------|--------|
| Blog post | Conversational, opinionated | 800–1500 words |
| Newsletter | Curated, brief summaries | 500–800 words |
| Essay | Analytical, thorough | 2000–4000 words |
| Dataset description | Factual, precise | 200–400 words |
| Research paper | Formal academic | 8000+ words |

---

## 10. Research Areas

All content should map to one of the four research pillars:

1. **Innovation & Technology** — Patents, trademarks, blockchain, smart contracts, and cryptographic assets reshaping ownership and digital exchange
2. **Economics of Punishment** — Effectiveness of punitive measures against financial misconduct, deterrence, rehabilitation, and governance
3. **Market Participation** — Behavior of parties and counterparties within transactions, market entry and exit, price formation, and liquidity
4. **Market Microstructure** — Formation of networks within markets, trading relationships and institutional linkages across established and emerging economies

---

## 11. Social & External Presence

| Platform | Handle / URL |
|----------|-------------|
| Website | ndum.org |
| GitHub | github.com/NDUM-ORG |
| LinkedIn | linkedin.com/company/ndum-org |

**Social image defaults:**
- Use logo on dark background (`#0F1720`)
- Include "NDUM" text in Georgia serif if logo is too small to read
- Minimum contrast ratio: 4.5:1 for all text over backgrounds

---

## 12. File Naming Conventions

| Type | Pattern | Example |
|------|---------|---------|
| Blog posts | Numeric in `/blog/posts/` | `5.md` |
| Newsletters | `nl_MMDDYYYY.pdf` | `nl_04152026.pdf` |
| Datasets | `snake_case` descriptive | `federal_penalties_2000_2025.csv` |
| Images (people) | `YYYY_firstname.png` | `2025_rodney.png` |
| Images (general) | `snake_case` descriptive | `dex_volume_chart.png` |

---

## Quick Reference Card

```
Primary Blue:       #4361EE
Blue Light:         #6580F5
Blue Dark:          #2F4ABF
Background (light): #F1F5F9
Background (dark):  #0F1720
Text:               #1E293B / #E2E8F0
Headings:           Georgia, serif, 700
Body:               System sans-serif, 400
Cards:              12px radius, 1px border, hover glow
Buttons:            8px radius, blue or outline
```
