# CRITIQUE

Diagnose the level of failure: thesis fit, distinctiveness, coherence, specificity, hierarchy/composition, craft, Slop Check. Route local craft→APPLY; system→CODIFY; weak world→DIVERGE/REFERENCE; wrong direction→SELECT/POSITION; misunderstood problem→DISCOVER. Never solve strategic failure with decoration.

---

## Purpose
Evaluate design work against the creative thesis and identify the *earliest* layer where something broke. Critique is forensic, not cosmetic—find the root cause before proposing fixes.

## Inputs
- Artifact(s) to critique: screenshot, URL, code, Figma, deck, video, image generation output
- Creative thesis / DESIGN.md (if exists)
- User's stated concern or "general review" request

## Steps

### 1. Establish evaluation baseline
- Load DESIGN.md if it exists; otherwise use stated thesis/principles
- If no thesis exists, note this—the critique may reveal that POSITION is needed first
- Identify what artifact type this is and what job it's meant to do

### 2. Run the seven-layer diagnostic
Evaluate every layer and record pass/fail for the report. The *earliest* failure is the root cause for routing—everything downstream is likely symptomatic, not causal. Do not stop evaluating after the first failure; complete the full diagnostic, then route based on the earliest broken layer.

| Layer | Question | Failure signal |
|-------|----------|----------------|
| **Thesis fit** | Does this work express the governing idea? | Artifact could belong to a different brand/product with no modification |
| **Distinctiveness** | Would this be recognizable without the logo? | Passes the "cover the logo" test? Or generic? |
| **Coherence** | Do all elements feel like they belong to the same world? | Mixed signals, inconsistent voice, Frankenstein feeling |
| **Specificity** | Are choices tied to this brand/audience/context? | Choices are arbitrary or model-default |
| **Hierarchy/composition** | Does the eye move intentionally? Does tension exist where appropriate? | Everything centered/even, no clear entry point, no rhythm |
| **Craft** | Are details executed cleanly? | Sloppy spacing, bad kerning, misaligned elements, color math issues |
| **Slop signals** | Run `principles/slop-check.md` | Any "yes" answers |

### 3. Diagnose the root layer
Name the *first* broken layer explicitly:
- "This fails at **thesis fit**—the visual language doesn't express 'accessible brutalism,' it looks like generic SaaS"
- "Thesis and distinctiveness are fine; this fails at **craft**—the icon grid is inconsistent and the type is poorly tracked"

### 4. Determine routing
Route backward to the layer that caused the problem:

| Root failure | Route to | Rationale |
|--------------|----------|-----------|
| Thesis fit | SELECT or POSITION | Direction itself is wrong |
| Distinctiveness | DIVERGE or REFERENCE | Need stronger visual world |
| Coherence | CODIFY | Rules aren't clear enough to maintain consistency |
| Specificity | REFERENCE or POSITION | Not grounded in real context |
| Hierarchy/composition | APPLY | Execution problem, not direction problem |
| Craft | APPLY | Local fix, keep iterating |
| Slop signals | Depends on signal source | Trace each signal to its origin layer |

### 5. Provide actionable next step
State one clear action:
- "Return to DIVERGE and create a world that actually embodies 'industrial warmth' instead of 'corporate friendly'"
- "This is a craft issue—fix the baseline grid in the card component and tighten the heading kerning"

## Output shape
```
## Critique: [artifact name/type]

**Evaluation baseline:** [thesis summary or "no thesis—POSITION needed"]

**Layer diagnosis:**
- Thesis fit: [pass/fail + one line]
- Distinctiveness: [pass/fail + one line]
- Coherence: [pass/fail + one line]
- Specificity: [pass/fail + one line]
- Hierarchy/composition: [pass/fail + one line]
- Craft: [pass/fail + one line]
- Slop check: [pass/fail + signals found]

**Root failure:** [layer name]

**Routing:** [phase] — [why]

**Next action:** [one concrete instruction]
```

## Quality gates
- [ ] Named the root layer, not just symptoms
- [ ] Routing matches the layer (don't send craft problems to POSITION)
- [ ] Provided one actionable next step, not a laundry list
- [ ] Did not suggest decoration/polish if the failure is strategic
- [ ] Referenced the thesis in evaluation (or flagged its absence)

## Anti-patterns
- **Cosmetic critique**: "Add more white space" when the problem is thesis fit
- **Polish cascade**: Suggesting refinements at every layer instead of finding the root
- **Vague diagnosis**: "It doesn't feel right" without identifying which layer
- **Premature solutions**: Proposing fixes before completing diagnosis
- **Decoration as fix**: "Add texture/illustration/animation" to mask strategic weakness
- **Skipping layers**: Jumping to craft critique when distinctiveness is the issue

## Good vs bad critique one-liners

**Bad:** "The typography could be more interesting"
**Good:** "Typography fails specificity—nothing ties the type choices to the 'archival science' thesis; these are model defaults"

**Bad:** "It looks too generic"
**Good:** "Fails distinctiveness at the world level—this could be any fintech. Route to DIVERGE with stronger reference territory"

**Bad:** "Needs more visual hierarchy"
**Good:** "Hierarchy/composition failure—the three CTAs compete equally. Primary action unclear. Fix in APPLY"

**Bad:** "Colors feel off"
**Good:** "Color fails coherence—the accent palette was generated without relationship to the core palette. Return to CODIFY to establish color rules"

## When to stop
- You've identified ONE root layer and ONE routing decision
- Further diagnosis would be drilling into symptoms, not causes

## When to route elsewhere
- No thesis exists → must complete POSITION before meaningful critique
- User wants to "just fix it" without diagnosis → explain why that leads to decoration-over-strategy, then offer quick-fix vs proper-fix options
- Critique reveals the brief was misunderstood → route to DISCOVER

## See also
- `principles/slop-check.md` — the slop-signal checklist
- `templates/critique.md` — blank template for structured critique output
- `examples/critique.filled.md` — example of a completed critique (Terracotta dashboard)
