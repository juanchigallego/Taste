# CODIFY

Turn selected intent into transferable rules using DESIGN.md. Encode thesis, principles, concrete behavior, anti-patterns, reference rationale, degrees of freedom and "when uncertain" heuristics. Do not freeze arbitrary values that have not been tested.

---

## Purpose
Formalize the selected direction into transferable rules that enable consistent execution without requiring re-explanation. CODIFY creates the system that allows APPLY to happen correctly.

## Inputs
- Selected world from SELECT (with KEEPs locked)
- Reference territory with extracted principles
- Generated evidence from DIVERGE
- Any existing brand assets or constraints

## Steps

### 1. Start with thesis and principles
Before any tokens or specs, codify the governing ideas:
- **Creative thesis**: One sentence that governs all decisions
- **Principles (3–5)**: Observable behaviors, not vague values
- **Anti-principles**: What this brand explicitly rejects

**Bad principle:** "Be bold"
**Good principle:** "Use scale contrast to create hierarchy—nothing is medium"

**Bad anti-principle:** "Don't be boring"
**Good anti-principle:** "Never center everything—tension and asymmetry express our point of view"

### 2. Define "when uncertain" heuristics
These prevent decision paralysis and model defaults:
- "When uncertain about color: prefer the muted palette, use accent sparingly"
- "When uncertain about type size: go larger—this brand isn't quiet"
- "When uncertain about imagery: real photography over illustration"

### 3. Codify concrete behavior per domain
For each domain in `templates/DESIGN.md`, document:
- **What**: Specific choices (typefaces, colors, grid, etc.)
- **Why**: How this expresses the thesis
- **Rules**: Observable constraints
- **Anti-patterns**: What to avoid

Only codify what's been tested. Don't invent rules that haven't been validated through DIVERGE/APPLY.

### 4. Define degrees of freedom
Not everything should be locked:

| Invariant (locked) | Flexible (can vary) |
|--------------------|---------------------|
| Primary typeface | Supporting faces for specific contexts |
| Core palette | Extended palette for illustrations |
| Logo usage rules | Photography treatment can evolve |
| Thesis | Specific artifacts can experiment |

State what can flex and what cannot.

### 5. Document signature artifacts
What recurring elements identify this brand?
- A specific typographic lockup pattern
- A color interaction rule
- A recurring shape or device
- A photography treatment
- A motion behavior

These should pass the "cover the logo" test—recognizable without the logo.

### 6. Add reference rationale
For major decisions, link back to references:
- "Slab serif choice references trade manuals—expertise without pretension"
- "4-column grid with wide gutters references archival layouts"

This prevents future drift by explaining *why*, not just *what*.

## Output shape
Use `templates/DESIGN.md` structure. Key sections:

```markdown
## Creative thesis
[One sentence]

## Creative principles
1. [Principle: observable behavior]
2. [Principle]
3. [Principle]

## Anti-principles
- [What we explicitly reject]
- [What we explicitly reject]

## When uncertain
- Prefer X over Y because [thesis reason]
- Prefer A over B because [thesis reason]

## Never
- [Hard constraint with rationale]
- [Hard constraint with rationale]

## [Domain: Typography/Color/Composition/etc.]
### What
[Specific choices]
### Why
[Thesis connection]
### Rules
[Observable constraints]
### Anti-patterns
[What to avoid]

## Degrees of freedom
### Invariants
[What's locked and why]
### Flexible
[What can vary and within what bounds]

## Signature artifacts
[What makes this recognizable without the logo]

## Reference rationale
[Why major decisions were made, linked to references]
```

## Quality gates
- [ ] Thesis is present and governs everything
- [ ] Principles are observable behaviors, not adjectives
- [ ] "When uncertain" heuristics exist
- [ ] Anti-patterns are explicit
- [ ] Only tested decisions are codified (no invented rules)
- [ ] Degrees of freedom are clear
- [ ] Reference rationale explains major choices

## Anti-patterns
- **Premature codification**: Locking rules that haven't been tested
- **Token-only documentation**: Colors and fonts but no principles
- **Vague principles**: "Be authentic" (not observable)
- **Over-specification**: No room for appropriate flexibility
- **Missing anti-patterns**: Only says what to do, not what to avoid
- **Orphan decisions**: Rules without thesis connection

## When to route elsewhere
- Rules don't feel right in practice → APPLY to test, then revise
- Realize direction is wrong → SELECT or DIVERGE
- Missing territory to codify → REFERENCE
- Can't articulate principles → thesis may be unclear (POSITION)

## See also
- `templates/DESIGN.md` — the full template
- `examples/DESIGN.md.partial.md` — example of a partial but good DESIGN.md
