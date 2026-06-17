---
name: elite-powerpoint-designer
description: Transform content into world-class presentations with the design quality of Apple keynotes, Microsoft product launches, and Google I/O. Use when the user requests a professional presentation, pitch deck, or wants Apple/Microsoft/Google style slides. Applies 2024-2025 presentation design trends and brand-level consistency.
---

# Elite PowerPoint Designer

Transform content into world-class presentations with the design quality of Apple keynotes, Microsoft product launches, and Google I/O. This skill applies 2024-2025 presentation design trends and brand-level consistency to create stunning, professional slide decks.

## Core Design Philosophy

1. **Minimalism First** - Remove everything that doesn't serve a clear purpose
2. **Bold & Clear** - Large typography, high contrast, confident colors
3. **Visual Hierarchy** - Guide attention through size, color, and spacing
4. **Consistent Branding** - Every element follows the design system
5. **Purposeful Motion** - Animations only where they add clarity or emphasis

## Available Brand Styles

### 1. Tech Keynote (Apple/Tesla Style)
- Colors: Deep blacks (#000000), whites (#FFFFFF), accent blue (#0071E3)
- Typography: SF Pro Display (title 72-96pt), SF Pro Text (body 32-44pt)
- Layout: Extreme whitespace, single focal point per slide
- Transitions: Push, Fade (duration: 0.6s)
- Style: Minimalist, premium, product-focused

### 2. Corporate Professional (Microsoft/IBM Style)
- Colors: Navy (#003366), steel blue (#0078D4), warm gray (#F3F2F1)
- Typography: Segoe UI (title 54-72pt), body (24-32pt)
- Layout: Balanced, grid-based, data-friendly
- Transitions: Morph, Fade (duration: 0.8s)
- Style: Trustworthy, data-driven, enterprise-ready

### 3. Creative Bold (Google/Airbnb Style)
- Colors: Bright primaries, gradients, bold combinations
- Typography: Montserrat (title 64-84pt)
- Layout: Dynamic, asymmetric, playful spacing
- Transitions: Zoom, Reveal (duration: 0.5s)
- Style: Energetic, innovative, design-forward

### 4. Financial Elite (Goldman Sachs/McKinsey Style)
- Colors: Charcoal (#2C3E50), gold accent (#D4AF37), white
- Typography: Georgia (serif, elegant)
- Layout: Traditional hierarchy, centered, balanced
- Transitions: Subtle Fade only (duration: 0.4s)
- Style: Sophisticated, authoritative, premium

### 5. Startup Pitch (Y Combinator Style)
- Colors: High contrast black/white with brand accent
- Typography: Inter or Roboto (modern sans-serif)
- Layout: Problem-solution focused, metric-heavy
- Transitions: Quick Push (duration: 0.3s)
- Style: Energetic, data-driven, founder-friendly

## Typography Hierarchy

```
Hero Title:     72-96pt, Bold, 1.1x line height
Section Title:  54-72pt, Semibold, 1.2x line height
Slide Title:    44-54pt, Semibold, 1.3x line height
Body Large:     32-36pt, Regular, 1.4x line height
Body:           24-28pt, Regular, 1.5x line height
Caption:        18-20pt, Light, 1.6x line height
```

## Spacing System

```
Gutter:              100-120px from edges
Title margin-bottom: 60-80px
Section spacing:     40-60px
Paragraph spacing:   24-32px
Bullet indent:       40px
Element padding:     20-30px
```

## Slide Type Detection

```
# Title      → title_slide (hero treatment)
## Section   → chapter_intro (section divider)
### Points   → key_message_slide (1-3 key points)
* Bullets    → bullet_hierarchy_slide
> Quote      → quote_slide (large, impactful)
| table |    → data_visualization (auto-chart if numeric)
```

## Animation Guidelines

**Tier 1 — Always Safe:**
- Fade (0.6s), Push (0.4s), Morph (0.8s)

**Tier 2 — Use Sparingly:**
- Zoom (0.5s), Reveal (0.6s), Wipe (0.5s)

**Tier 3 — Never Use:**
- Ferris Wheel, Curtains, Dissolve, Origami

**Rules:**
- Max 3 animated elements per slide
- 1-2 transition types per deck
- Text entrance: Fade In (0.4s)
- Stagger bullets: 0.3s delay between items

## Quality Checklist

- [ ] All slides use design system colors (no random colors)
- [ ] Typography follows hierarchy (max 4 font sizes)
- [ ] Consistent spacing (same margins throughout)
- [ ] One main idea per slide
- [ ] No walls of text (max 6 lines body)
- [ ] Transitions consistent (1-2 types only)
- [ ] Emphasis animations only on critical moments
- [ ] 4.5:1 contrast ratio for accessibility

## Implementation with python-pptx

Use python-pptx to implement designs. Key principles:
- Slide dimensions: 18288000 x 10287000 EMU (16:9)
- Use blank layout (index 6) for full design control
- Define color system as RGBColor constants
- Implement typography hierarchy strictly
- Use rbox() for background panels and color blocks
- Never use default PowerPoint themes — build from scratch

## Workflow

1. Analyze content type and audience → select brand style
2. Map each content block to slide type
3. Apply design system (colors, typography, spacing)
4. Build with python-pptx maintaining hierarchy
5. Validate consistency across all slides
6. Apply professional polish (shadows, overlays where needed)

## Tips

- Start with style selection before building
- Less is more: 1 slide per minute of presentation
- One main idea per slide — split if needed
- Test that every slide works without the presenter
- Design for PDF export too (animations become static)
