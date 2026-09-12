# DESIGN.md — Terracotta (Partial Example)

This is a partial but substantive DESIGN.md for a fictional soil-testing platform called Terracotta. It demonstrates how to codify a creative direction with enough specificity to be actionable while leaving appropriate degrees of freedom.

**Note:** This is not a complete DESIGN.md—some sections are marked [TO BE DEVELOPED] to show that codification happens progressively as work advances. Don't invent rules you haven't tested.

---

## Creative thesis

**Accessible scientific expertise for people who work with soil.**

Terracotta translates complex soil science into confident decisions for farmers, agronomists, and land managers. The brand should feel like a knowledgeable colleague—precise but unpretentious, technical but never intimidating.

---

## Creative principles

1. **Precision without sterility** — Every number, chart, and data point should feel exact and trustworthy. But the overall tone is warm earth, not cold lab. Technical ≠ clinical.

2. **Grounded in real soil** — Visual choices connect to actual land, place, and material. Photography shows real conditions. Color comes from actual soil classification. No stock-photo agriculture.

3. **Clarity at every scale** — Data-dense interfaces must be legible and calm. When in doubt, add space, not decoration. The information is the hero.

4. **Expertise earns trust** — The brand demonstrates competence through quality of information, not through marketing language or visual polish. Show, don't claim.

---

## Anti-principles

- **Never clinical** — No white-room photography, no lab coat aesthetics, no blue-and-white medical sterility. We rejected this direction in V1.

- **Never cute/artisanal** — No hand-drawn elements, no kraft paper textures, no "farm-to-table" preciousness. We rejected this direction in V2.

- **Never generic SaaS** — No card-heavy layouts, no generic gradient backgrounds, no system-font-only dashboards. Pass the Slop Check.

---

## Personality & productive tensions

| Tension | How we hold it |
|---------|----------------|
| Technical ↔ Accessible | Lead with accessible language; technical detail available on demand |
| Scientific ↔ Earthy | Color and photography ground the science in real soil |
| Precise ↔ Warm | Precision in data; warmth in typography spacing and photography |
| Expert ↔ Humble | Show competence through work quality, not claims |

---

## Typography

### What
- **Primary:** Söhne (technical grotesque)
- **Data/Monospace:** Söhne Mono for readings, measurements, values
- **Fallback:** system sans-serif (Inter > SF Pro > Segoe)

### Why
Söhne has the technical precision of a grotesque but softer optical qualities than industrial faces like Helvetica. Feels modern and scientific without cold. The mono version matches the aesthetic while serving data readability.

### Rules
- Display type: loose tracking (+2-5% depending on size)
- Body type: default tracking, generous line-height (1.5-1.6)
- All-caps sparingly—labels and micro-UI only
- No script, serif, or decorative faces—they conflict with the thesis

### Anti-patterns
- Tight/default tracking on large display type (feels cramped)
- System fonts where the brand should be visible
- Mixing type families beyond the Söhne family

---

## Color

### What
**Core palette** — Derived from Munsell Soil Color Charts:
- `soil-dark` #3D3129 — organic-rich topsoil
- `soil-mid` #785C45 — clay loam
- `soil-light` #C4A882 — sandy soil
- `soil-pale` #EDE5D8 — limestone-influenced

**Functional palette:**
- `data-blue` #2D5A7B — primary data visualization, interactive elements
- `alert-amber` #C77B1F — warnings, attention states
- `success-green` #3D6B4D — confirmations, healthy ranges

**UI neutrals:**
- `surface` #F7F5F2 — warm off-white backgrounds
- `surface-dark` #2A2622 — dark mode / inverse surfaces

### Why
Using actual soil classification as a color source grounds the brand in its subject matter. This is distinctive (competitors use generic palettes) and defensible (connects to real science). Functional colors are muted to sit alongside the earth tones.

### Rules
- Soil palette dominates brand and marketing contexts
- Functional palette leads in product/UI contexts
- Never pure black or pure white—always slightly warm
- Data visualization uses the blue-amber-green range for accessibility

### Anti-patterns
- Bright/saturated accent colors (conflict with earthy grounding)
- Pure #000 or #FFF (feels clinical)
- Using soil colors for interactive affordances (browns don't read as clickable)

---

## Imagery & photography

### What
Specimen-style photography of soil, land, and field conditions:
- Soft, even lighting (no harsh shadows)
- Cream/warm backgrounds or in-situ environmental shots
- Subtle shadow/depth, not flat
- Square or 4:3 crops preferred

### Why
References scientific specimen photography (credible) while the soft light and warm tones keep it accessible. Real soil and real conditions signal authenticity.

### Rules
- No stock photography of generic "happy farmers"
- Soil photography should show actual texture and color variation
- People in photos are working, not posing
- Environmental shots show real weather and conditions

### Anti-patterns
- Blue-sky hero imagery (generic ag-tech)
- Clean-room or lab photography (clinical)
- Over-saturated "look at our beautiful farm" shots (tourism, not science)

---

## Composition & grid

### What
- 12-column grid, large gutters (24-32px)
- Generous white space, especially around data
- Asymmetric layouts preferred over centered
- Clear visual hierarchy: one primary element per view

### Why
References survey maps and technical documents that organize complex data calmly. Large gutters and white space provide the "breathing room" that distinguishes us from cluttered ag-tech dashboards.

### Rules
- Data-dense views still need margin and breathing room
- Asymmetric tension is encouraged—don't default to centering
- Cards used sparingly and only when grouping aids comprehension

### Anti-patterns
- Everything in cards (Slop Check failure)
- Centered/symmetrical-everything layouts
- Wall-to-wall data without spatial organization

---

## When uncertain

- **Color:** Prefer soil palette for brand contexts, functional palette for UI affordances
- **Photography:** Prefer imperfect real conditions over polished perfection
- **Layout:** Prefer asymmetry over centering; prefer white space over filling
- **Typography:** Prefer loose over tight; prefer fewer weights over more
- **Tone:** Prefer confident and direct over hedge-y marketing language

---

## Never

- Clinical white-room aesthetics (violates thesis)
- Hand-drawn or artisanal elements (wrong register)
- Generic stock photography of agriculture
- Pure black or pure white (use warm neutrals)
- Tight typography tracking on display sizes
- Marketing superlatives without evidence ("industry-leading", "revolutionary")

---

## Degrees of freedom

### Invariants (do not change)
- Söhne typography family
- Munsell-derived soil color palette
- Specimen photography treatment
- No clinical or artisanal aesthetics

### Flexible (can evolve)
- Extended illustration style (not yet developed)
- Motion/animation principles (not yet developed)
- Secondary data visualization palettes for specific chart types
- Photography can expand to include more environmental contexts

---

## Signature artifacts

The following elements should be recognizable even without the logo:

1. **Soil core cross-section** — A recurring graphic element showing horizontal soil stratification; used as dividers, loading states, brand marks
2. **Munsell color coding** — Data always color-coded to actual soil classification
3. **Specimen crop** — Square photographs with soft shadow on warm backgrounds

---

## Reference rationale

| Decision | Reference | Principle |
|----------|-----------|-----------|
| Söhne typography | Dieter Rams product manuals | Technical precision with warmth through spacing |
| Munsell palette | USDA Soil Surveys | Ground brand in actual subject matter, not generic palette |
| Specimen photography | Natural history museum displays | Scientific credibility without sterility |
| Wide gutters | Emigre, archival layouts | Breathing room signals considered quality |

---

## Sections still to develop

- [ ] Shape language
- [ ] Iconography
- [ ] Motion principles
- [ ] Interaction patterns
- [ ] Voice & microcopy
- [ ] Accessibility constraints

These should be developed as work advances, not invented before testing.

---

## How to use this example

This partial DESIGN.md demonstrates:

1. **Thesis governs everything** — Every section connects back to "accessible scientific expertise"
2. **Principles are observable** — Not "be professional" but "precision without sterility"
3. **Anti-principles are explicit** — Clear rejections from the Direction History
4. **When uncertain gives defaults** — Prevents decision paralysis
5. **Degrees of freedom** — Not everything is locked down
6. **Reference rationale** — Explains *why*, preventing drift
7. **Incomplete is OK** — Don't invent rules you haven't tested

For the template structure, see `templates/DESIGN.md`.
