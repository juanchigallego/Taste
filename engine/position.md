# POSITION

Turn the brief into a point of view. Produce one Creative Thesis capable of governing many decisions, plus 3–5 principles and anti-principles. Avoid adjective soup. Good thesis creates productive constraints. Gate: user recognizes the intended character.

---

## Purpose
Convert discovery into a governing creative point of view. POSITION is where taste becomes actionable—a thesis that can reject options, not just describe preferences. Without this, DIVERGE produces arbitrary "cool" directions.

## Inputs
- Discovery synthesis from DISCOVER
- User feedback on what feels right/wrong (even if vague)
- Productive tensions identified
- Category codes and differentiation opportunities

## Steps

### 1. Draft the creative thesis
One sentence that governs all future decisions. Test it:

| Test | Pass? |
|------|-------|
| Could this thesis reject a plausible direction? | If no, it's too vague |
| Does it create productive constraints? | If no, it's a description not a point of view |
| Would the user recognize the intended character? | If no, iterate with them |
| Is it specific to this brand/product/audience? | If no, it's generic |

**Bad thesis:** "A modern, professional brand that feels trustworthy and innovative"
**Good thesis:** "Accessible scientific expertise for people who work with soil—precise but unpretentious, like a knowledgeable colleague not a lab report"

**Bad thesis:** "Premium luxury for discerning customers"
**Good thesis:** "Quiet confidence through material honesty—luxury expressed by what we leave out, not what we add"

### 2. Extract 3–5 creative principles
Principles are observable behaviors, not adjectives. Each should be testable against a design decision.

**Bad principle:** "Be bold"
**Good principle:** "Use scale contrast to create hierarchy—nothing is medium-sized"

**Bad principle:** "Feel warm and approachable"
**Good principle:** "Lead with accessible language; technical detail available on demand, never forced"

### 3. Define anti-principles
What this brand explicitly rejects. Anti-principles prevent drift and give CRITIQUE clear failure modes.

**Bad anti-principle:** "Don't be boring"
**Good anti-principle:** "Never clinical—no white-room photography, no lab coat aesthetics"

**Bad anti-principle:** "Avoid bad design"
**Good anti-principle:** "Never center everything—tension and asymmetry express our point of view"

### 4. Name productive tensions
How does the brand hold opposing qualities?

| Tension | How we hold it |
|---------|----------------|
| Technical ↔ Accessible | [specific behavior] |
| Premium ↔ Humble | [specific behavior] |

### 5. Validate with the user
Present thesis + principles + anti-principles. Ask: "Does this feel like the character you want?" Iterate until recognized.

## Output shape
```
## Position: [project name]

**Creative thesis:** [one sentence]

**Principles:**
1. [observable behavior]
2. [observable behavior]
3. [observable behavior]

**Anti-principles:**
- [explicit rejection]
- [explicit rejection]

**Productive tensions:**
| Tension | Resolution |
|---------|------------|
| [A ↔ B] | [how held] |

**Gate:** User recognizes intended character? [yes/no + notes]

**Next step:** [REFERENCE to find territory / DIVERGE if references exist]
```

## Quality gates
- [ ] Thesis is one sentence and governs decisions
- [ ] Thesis could reject at least one plausible direction
- [ ] Principles are observable behaviors, not adjectives
- [ ] Anti-principles are explicit and specific
- [ ] User recognizes the intended character
- [ ] No adjective soup ("modern, clean, premium, professional")

## Anti-patterns
- **Adjective soup**: "Modern, clean, premium, innovative, trustworthy"
- **Unfalsifiable thesis**: Can't reject anything because it's too vague
- **Borrowed thesis**: Copying a competitor's positioning
- **Feature-list positioning**: "We're the fastest/cheapest/best" (not creative direction)
- **Premature visual commitment**: Locking colors/fonts before thesis is validated

## Good vs bad positioning one-liners

**Bad:** "We want to feel modern and professional like Stripe"
**Good:** "Technical credibility through restraint—complexity handled calmly, never hidden behind decoration"

**Bad:** "Our brand should be fun and playful"
**Good:** "Serious science, zero pretension—playfulness comes from clarity and directness, not illustration or bright colors"

## When to stop
- User confirms thesis and principles
- Ready to find visual territory (→ REFERENCE) or diverge (→ DIVERGE if references exist)

## When to route elsewhere
- Discovery was insufficient → DISCOVER
- User provides references with clear direction → REFERENCE (validate thesis against them)
- Thesis keeps failing validation → may need more DISCOVER
- Thesis locked but user wants to see options immediately → DIVERGE (with thesis as constraint)

## See also
- `engine/discover.md` — upstream if brief is unclear
- `engine/reference.md` — next step to find visual territory
- `examples/DESIGN.md.partial.md` — example of codified thesis + principles for Terracotta
