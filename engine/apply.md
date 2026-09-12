# APPLY

Prove the direction in a real, demanding artifact with real content/constraints when possible. Separate structural/pattern research from art direction. In code, prevent framework/component-library defaults from taking over. Always route through CRITIQUE.

---

## Purpose
Execute the codified direction in a real artifact that stress-tests the system. APPLY is where principles meet reality—bad rules reveal themselves here. Never ship APPLY output without CRITIQUE.

## Inputs
- DESIGN.md (or thesis + principles if CODIFY is partial)
- Direction History with locked KEEPs
- Real content when possible (actual copy, data, images—not lorem ipsum)
- Target artifact type (landing page, dashboard, logo lockup, email, deck slide, etc.)
- Technical constraints (framework, component library, platform)

## Steps

### 1. Choose a demanding artifact
Pick something that stress-tests the direction, not a safe application:
- **Too easy:** Logo on white background, hero with headline only
- **Right difficulty:** Dashboard with real data, landing page with 5+ sections, email with mixed content types
- **Best:** The artifact the user actually needs, with real content

### 2. Separate structure from art direction
Before making, distinguish:
- **Structural patterns**: layout logic, information hierarchy, interaction flows (can borrow from pattern libraries)
- **Art direction**: color, type, imagery, spacing, signature artifacts (must come from DESIGN.md)

Pattern libraries solve structure. They do not solve taste. Never let a component library's default aesthetic become the brand.

### 3. Load the system
Before executing, confirm you have:
- Creative thesis (governing idea)
- Principles and anti-principles (decision filters)
- "When uncertain" heuristics (defaults to prevent model drift)
- Specific rules for relevant domains (type, color, composition, imagery)
- Signature artifacts to include

If any of these are missing, route to CODIFY first.

### 4. Execute with anti-default vigilance
Common default takeovers to actively resist:

| Default source | What it does | Counter |
|----------------|--------------|---------|
| Component library | Card-heavy, rounded, blue-primary UI | Override tokens; challenge every card wrapper |
| Model aesthetic | Gradients, glow, glass, centered layouts | Check against anti-principles and Slop Check |
| Framework conventions | System fonts, default spacing, Bootstrap grid | Apply DESIGN.md type and spacing rules |
| Stock content | Generic photos, placeholder copy | Use real content or clearly marked stand-ins |
| "Safe" composition | Everything centered, equal-weight sections | Apply composition rules (asymmetry, hierarchy) |

### 5. Include signature artifacts
Every APPLY output should include at least one element that passes the "cover the logo" test—a recurring behavior, typographic pattern, color interaction, or graphic device from DESIGN.md.

### 6. Route through CRITIQUE
Never present APPLY output as final. Always run `engine/critique.md` before showing the user. APPLY without CRITIQUE is how slop ships.

## Output shape
```
## Applied: [artifact name/type]

**System used:** [DESIGN.md version or thesis summary]
**Artifact:** [what was built]
**Content:** [real or stand-in — note which]
**Signature artifacts included:** [list]
**Defaults resisted:** [what you actively overrode]
**Known gaps:** [sections not yet codified in DESIGN.md]

→ Proceed to CRITIQUE
```

## Quality gates
- [ ] Artifact type is demanding enough to stress-test the system
- [ ] Real content used when possible
- [ ] DESIGN.md rules applied, not just referenced
- [ ] Component library defaults overridden where they conflict
- [ ] At least one signature artifact present
- [ ] CRITIQUE run before presenting to user

## Anti-patterns
- **Logo-on-white**: Applying direction to the easiest possible artifact
- **Lorem ipsum execution**: Fake content hides hierarchy and content problems
- **Library-as-brand**: Shadcn/Tailwind/MUI defaults become the aesthetic
- **Skip critique**: Presenting APPLY output as done
- **Invent rules**: Making design decisions not in DESIGN.md without flagging
- **Decoration pass**: Adding polish to compensate for missing art direction

## Good vs bad apply one-liners

**Bad:** "Here's the landing page using our component library"
**Good:** "Landing page built with real product copy. Overrode card defaults—used asymmetric 12-col grid with wide gutters per DESIGN.md. Soil-core divider included as signature artifact"

**Bad:** "I made a logo, what do you think?"
**Good:** "Logo lockup in context: business card + app icon + favicon at 16px. Tests whether the mark survives the 'cover the logo' test at small sizes"

## When to stop
- Artifact is built and CRITIQUE has been run
- CRITIQUE passes or routing decision is made
- User confirms the artifact expresses the intended character

## When to route elsewhere
- DESIGN.md is missing or too thin → CODIFY
- APPLY reveals direction is wrong → CRITIQUE → SELECT/DIVERGE
- Rules don't work in practice → CODIFY (revise rules, then re-APPLY)
- Brief was wrong → DISCOVER
- Implementation in code → `tools/implementation.md` for coding-agent handoff

## See also
- `engine/critique.md` — mandatory next step after APPLY
- `engine/codify.md` — upstream if system is incomplete
- `tools/implementation.md` — handoff to coding agents
- `examples/critique.filled.md` — example of critiquing an APPLY output that failed
