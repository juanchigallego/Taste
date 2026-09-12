# DIVERGE

Create 3–5 genuinely different visual worlds, not cosmetic variants. Each has name, premise, thesis relationship, rules, distinctive idea, risk and artifacts to test. Use image generation as world evidence. Translate feedback into KEEP / REMOVE / PUSH and mutate or branch. Loop with REFERENCE and SELECT.

---

## Purpose
Generate multiple distinct creative directions that could each fulfill the thesis. Diverge is *search*—expanding the possibility space before converging. The goal is genuine alternatives, not variations on a single idea.

## Inputs
- Creative thesis from POSITION
- Reference territory from REFERENCE (if completed)
- Any constraints (timeline, production reality, user aversions)
- Feedback from previous DIVERGE/SELECT cycles (if looping)

## Steps

### 1. Confirm thesis is locked
If there's no clear thesis, stop. Diverging without a thesis creates "cool but arbitrary" directions. Route to POSITION first.

### 2. Define the divergence axes
Before generating, identify 2–3 axes of variation to ensure genuine difference:

**Example axes:**
- Tone: austere ↔ exuberant
- Visual approach: photographic ↔ illustrative ↔ typographic
- Cultural reference: contemporary ↔ historical
- Complexity: minimal ↔ maximal
- Familiarity: category-expected ↔ category-breaking

State your axes before generating worlds.

### 3. Generate 3–5 worlds
For each world, define:

| Element | Description |
|---------|-------------|
| **Name** | Short, evocative handle (e.g., "Industrial Garden", "Quiet Archive") |
| **Premise** | One sentence: what if we expressed the thesis *this* way? |
| **Thesis relationship** | How does this world interpret the creative thesis? |
| **Core visual idea** | The one distinctive move that defines this world |
| **Rules** | 3–5 constraints this world obeys |
| **Risk** | What could go wrong / where this might fail |
| **Test artifacts** | 3–5 artifacts that would prove this world works |

### 4. Generate world evidence
Use image generation to test each world. Generate artifacts that stress-test the direction:
- Something typographic (poster, headline lockup, type specimen)
- Something photographic or image-driven (campaign image, product shot, editorial spread)
- Something functional (UI fragment, card, receipt, email, packaging)
- Something environmental (signage, physical space, merch)

Don't over-polish. These are probes, not finals.

### 5. Evaluate distinctiveness
Check: could someone confuse World A for World B? If yes, they're not different enough. Either merge them or push one further.

### 6. Collect feedback and translate to directives
When user responds, translate their feedback into structured directives:

| Directive | Meaning | Action |
|-----------|---------|--------|
| **KEEP** | This element is working, preserve it | Lock this in for next iteration |
| **REMOVE** | This element is wrong/distracting | Eliminate from all future versions |
| **PUSH** | This is interesting, go further | Intensify, exaggerate, explore more |

Record these in the decision history. Each KEEP/REMOVE/PUSH should be specific:
- **Bad:** "KEEP the vibe"
- **Good:** "KEEP the heavy slab serif paired with large photography"
- **Bad:** "REMOVE the weirdness"
- **Good:** "REMOVE the distressed/degraded texture treatment"

### 7. Mutate or branch
Based on feedback:
- **Mutate**: Take one world and evolve it (apply KEEP/REMOVE/PUSH)
- **Branch**: Combine elements from multiple worlds into a new hypothesis
- **Abandon**: If a world has no KEEPs, let it go
- **Loop**: Return to REFERENCE if the visual territory is too thin

## Output shape
```
## Divergence Round [n]

**Thesis:** [one-liner]
**Divergence axes:** [list 2–3]

### World 1: [Name]
- **Premise:** [one sentence]
- **Thesis relationship:** [how this interprets the thesis]
- **Core idea:** [the distinctive move]
- **Rules:** [3–5 bullets]
- **Risk:** [what could go wrong]
- **Test artifacts:** [list]
- **Generated evidence:** [image descriptions/links]

[Repeat for each world]

---

**Distinctiveness check:** [are these genuinely different?]
**Recommended next step:** [SELECT, more REFERENCE, continue DIVERGE]
```

## Quality gates
- [ ] All worlds connect to the thesis (not arbitrary "cool" directions)
- [ ] Worlds are genuinely different (not font/color variants)
- [ ] Each world has a nameable core idea
- [ ] Risks are identified (not just strengths)
- [ ] Test artifacts stress-test the direction (not just safe applications)
- [ ] Feedback is translated to specific KEEP/REMOVE/PUSH, not vibes

## Anti-patterns
- **Cosmetic variation**: Same world in three color palettes
- **Safe exploration**: All worlds are acceptable but none are interesting
- **Thesis drift**: Worlds that are cool but don't express the thesis
- **Premature polish**: Over-rendering before direction is chosen
- **Feedback hoarding**: Collecting vague "likes" instead of KEEP/REMOVE/PUSH
- **World overload**: 7+ worlds is decision paralysis; 3–5 is enough

## Good vs bad world definitions

**Bad world:**
> "Modern and clean with nice typography"

**Good world:**
> **"Quiet Archive"** — What if we expressed "accessible expertise" through the visual language of institutional archives? Heavy serif type, systematic grids, muted paper colors, photography as specimen documentation. Risk: could feel dusty instead of alive.

**Bad world:**
> "Colorful and playful"

**Good world:**
> **"Schoolyard Physics"** — What if we expressed "serious science, zero pretension" through playground vernacular? Bold primary colors, hand-drawn diagrams, ruled paper textures, rubber stamp typography. Risk: could undermine credibility if pushed too far.

## When to stop
- You have 3–5 worlds that are genuinely distinct
- Each world has enough evidence to evaluate
- User has provided KEEP/REMOVE/PUSH feedback
- Ready for SELECT

## When to route elsewhere
- No thesis → POSITION
- Can't find reference territory for a world → REFERENCE
- Feedback reveals brief was misunderstood → DISCOVER
- All worlds feel weak → may need to challenge the thesis (POSITION) or find better references (REFERENCE)

## See also
- `engine/reference.md` — gathering source material
- `engine/select.md` — choosing between worlds
- `templates/decision-history.md` — recording KEEP/REMOVE/PUSH
- `examples/decision-history.filled.md` — example of structured feedback
