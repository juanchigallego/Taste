# Recipe — Slop Rescue

CRITIQUE first. Identify whether genericness comes from thesis, references, system or local execution. Route to the earliest broken layer, then move forward again. Never just add decoration.

---

## Purpose
Take existing work that feels generic, default, or AI-generated and rebuild it into something specific and distinctive. Slop Rescue is not "add texture until it looks designed"—it's forensic diagnosis followed by reconstruction at the right level.

## When to use this recipe
- User says "this looks AI-generated" or "too generic"
- Work passed through AI tools and lost distinctiveness
- Design feels like it could belong to any brand
- Slop Check returns multiple failures
- User asks to "make it more interesting" without specific direction

## Inputs
- The sloppy artifact(s): screenshot, URL, code, Figma, image
- Any existing brand direction, thesis, or DESIGN.md (may not exist)
- User's sense of what's wrong (even vague "it feels generic")

## Steps

### 1. Run Slop Check
Load `principles/slop-check.md` and evaluate the artifact against each question. Document every "yes" answer.

Common slop signals and their typical sources:

| Slop signal | Typical source layer |
|-------------|---------------------|
| Could belong to 50 brands | Thesis / distinctiveness |
| Logo removal = unidentifiable | No signature artifacts in CODIFY |
| Choices not tied to thesis/audience | POSITION never done |
| Model defaults everywhere | APPLY executed without CODIFY |
| Surfaces copied, not principles | REFERENCE done superficially |
| Over-containerized (everything in cards) | Default component library, no CODIFY |
| Glow/glass/gradient without reason | Model aesthetic bias, no CODIFY |
| No tension in composition | APPLY didn't consider hierarchy |
| Decoration compensating for weak direction | Skipped POSITION/DIVERGE |

### 2. Run CRITIQUE diagnostic
Load `engine/critique.md` and identify the root failure layer:
- Thesis fit
- Distinctiveness
- Coherence
- Specificity
- Hierarchy/composition
- Craft

Name the *earliest* broken layer—everything downstream is symptomatic.

### 3. Determine rescue scope
Based on the root layer, scope the rescue:

| Root failure | Rescue scope | What you're rebuilding |
|--------------|--------------|------------------------|
| Thesis fit | Full rebuild | Need POSITION → REFERENCE → DIVERGE → SELECT → CODIFY → APPLY |
| Distinctiveness | World rebuild | Need REFERENCE → DIVERGE → SELECT → CODIFY → APPLY |
| Coherence | System rebuild | Need CODIFY → APPLY |
| Specificity | Grounding | Need REFERENCE (real context) → partial CODIFY |
| Hierarchy/composition | Execution fix | APPLY with intention |
| Craft | Local fix | APPLY polish pass |

**Be honest about scope.** If thesis fit is broken, you cannot rescue this with better typography.

### 4. Execute the rescue
Route to the appropriate phase and work forward:

**If thesis is broken:**
1. POSITION: Create a real creative thesis
2. REFERENCE: Find territory that supports it
3. DIVERGE: Create genuinely different worlds
4. SELECT: Choose a direction
5. CODIFY: Lock rules into DESIGN.md
6. APPLY: Rebuild the artifact from the new system
7. CRITIQUE: Verify the rebuild

**If distinctiveness is broken (thesis exists but world is generic):**
1. REFERENCE: Expand territory beyond category norms
2. DIVERGE: Create bolder worlds (push harder)
3. SELECT: Choose the most distinctive direction that fits thesis
4. CODIFY: Update DESIGN.md with distinctive rules
5. APPLY: Rebuild
6. CRITIQUE: Verify

**If coherence is broken (direction exists but not systematized):**
1. CODIFY: Formalize rules, find the inconsistencies
2. APPLY: Rebuild with consistent rules
3. CRITIQUE: Verify

**If only craft is broken:**
1. APPLY: Fix spacing, alignment, typography, color math
2. CRITIQUE: Verify

### 5. Verify rescue success
Re-run Slop Check. All previous "yes" answers should now be "no" or have explicit conceptual justification.

## Output shape
```
## Slop Rescue: [artifact name]

### Slop Check results
- [List each "yes" signal with its source layer]

### CRITIQUE diagnosis
- **Root failure:** [layer name]
- **Evidence:** [why this is the root, not symptoms]

### Rescue scope
- **Starting phase:** [POSITION/REFERENCE/DIVERGE/CODIFY/APPLY]
- **Rebuild path:** [list phases to execute]
- **What we're preserving:** [anything worth keeping, if any]
- **Estimated intensity:** [full rebuild / world rebuild / system fix / craft pass]

### Rescue execution
[Execute each phase, document decisions]

### Verification
- Slop Check: [re-run results]
- Distinctive signal: [what now identifies this work?]
- Thesis expression: [how does this now express the thesis?]
```

## Quality gates
- [ ] Slop Check run before any changes
- [ ] Root layer identified, not just symptoms
- [ ] Rescue scope matches root layer (no under-scoping)
- [ ] Not adding decoration to mask strategic failure
- [ ] Re-ran Slop Check after rescue
- [ ] Can articulate what makes the rescued version distinctive

## Anti-patterns
- **Decoration rescue**: "Add texture/gradients/illustrations" when thesis is broken
- **Surface rescue**: Copying a reference's surface instead of learning its principle
- **Speed rescue**: "Just make it look better" without diagnosis
- **Polish trap**: Spending hours on craft when distinctiveness is the problem
- **Vibe rescue**: "Make it feel more premium" without specific moves
- **Partial rescue**: Fixing one artifact without fixing the system that created it

## Good vs bad rescue decisions

**Bad:** "Add custom illustrations to make it feel less generic"
**Good:** "Distinctiveness is broken—before adding any assets, we need to REFERENCE non-category territory and DIVERGE to create a specific visual world"

**Bad:** "Change the font to something more interesting"
**Good:** "Typography is generic because CODIFY was skipped. First define: what role does type play in this thesis? Then select type that fulfills that role"

**Bad:** "Add more color"
**Good:** "Color is failing Slop Check (model defaults). Route to CODIFY: define a color logic tied to the thesis, not just 'nice palette'"

**Bad:** "This just needs polish"
**Good:** "No—the root failure is thesis fit. This SaaS dashboard could be any SaaS dashboard. No amount of polish fixes that. Start at POSITION"

## When to stop
- Slop Check passes (or all remaining signals have conceptual justification)
- Work is recognizable without the logo
- Choices are traceable to the thesis
- User confirms the intended character is present

## When to reject the rescue
Sometimes the rescue reveals the original brief was wrong:
- "Make a generic, professional logo" → no rescue possible, need new brief
- Artifact type doesn't serve the real need → recommend different artifact
- Constraints make distinctiveness impossible → name the constraint and escalate

## See also
- `principles/slop-check.md` — the slop signal checklist
- `engine/critique.md` — the seven-layer diagnostic
- `engine/diverge.md` — creating distinctive worlds
- `engine/codify.md` — systematizing distinctiveness
- `examples/decision-history.filled.md` — Direction History example for rescue decisions
