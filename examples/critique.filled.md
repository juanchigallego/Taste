# Critique: Terracotta Soil Health Dashboard (v0.3 implementation)

**Artifact type:** Product UI — primary dashboard screen showing soil test results, field map, and recommendations.

**Evaluation baseline:** Terracotta DESIGN.md — thesis: "Accessible scientific expertise for people who work with soil." Principles: precision without sterility, grounded in real soil, clarity at every scale, expertise earns trust.

---

## Layer diagnosis

- **Thesis fit:** FAIL — Reads as generic ag-tech SaaS, not "accessible scientific expertise." Blue gradient header, stock farm imagery, and marketing-style KPI cards express "modern software" not "knowledgeable colleague who understands soil."
- **Distinctiveness:** FAIL — Cover the logo: could be any farm management or climate dashboard. No Munsell palette, no specimen photography, no soil-core signature artifact.
- **Coherence:** FAIL — Header uses blue gradient (not in palette); cards use white-on-gray (clinical); typography appears system default, not Söhne; photography style doesn't match specimen treatment.
- **Specificity:** FAIL — Color choices are model defaults (blue primary, green success). No connection to soil classification, place, or Terracotta's codified system.
- **Hierarchy/composition:** PARTIAL — Information is legible but every section is an equal-weight card. No asymmetry, no clear primary action. Functional but default.
- **Craft:** PARTIAL — Spacing is consistent within cards but gutters are tight. Type sizes are reasonable. Not broken, but not expressing the brand either.
- **Slop check:** FAIL — Multiple signals: could belong to 50 brands; logo removal = unidentifiable; over-containerized (everything in cards); blue gradient without conceptual reason; no memorable recurring rule.

**Root failure:** Distinctiveness (with thesis fit as co-failure — the world was never applied)

**Routing:** APPLY — but only after re-ingesting DESIGN.md. This is not a craft-only fix. The implementation ignored the codified system. Rebuild the dashboard using Terracotta rules: Munsell palette, Söhne type, specimen photography, wide gutters, asymmetric layout, soil-core graphic as section divider.

**Next action:** Rebuild dashboard hero and data cards following `examples/DESIGN.md.partial.md` color, typography, and composition rules. Remove blue gradient header. Replace stock photo with specimen-style soil photography. Test one asymmetric layout before polishing all sections.

---

## How to use this example

This critique demonstrates:

1. **All layers evaluated** — even when root failure is early, downstream layers are noted for the report
2. **Root vs symptoms** — craft is "partial" but fixing craft won't fix distinctiveness
3. **Routing matches root** — not "tweak the cards" but "rebuild using the codified system"
4. **Thesis referenced** — every failure tied back to governing idea
5. **One next action** — specific, not a laundry list

For the blank template, see `templates/critique.md`. For the DESIGN.md this artifact should follow, see `examples/DESIGN.md.partial.md`.
