# Taste v0.1
An agentic creative-direction skill for exploring, selecting, codifying and applying distinctive design.

Start with `SKILL.md`. `INDEX.md` is the human-facing capability map. The skill uses progressive disclosure across `engine/`, `modes/`, `recipes/`, `templates/`, `principles/`, and `tools/`.

Core loop: DISCOVER → POSITION → REFERENCE ↔ DIVERGE ↔ SELECT → CODIFY → APPLY ↔ CRITIQUE → SHIP.

## Install

### OpenAI Codex / Generic Agent Harness (Recommended)

Clone or vendor the repo into your project:

```bash
git clone https://github.com/juanchigallego/Taste.git skills/taste
```

Then add a pointer in your `AGENTS.md` (or project agent instructions):

```markdown
## Creative Direction

For brand, visual design, design systems, or DESIGN.md work:
1. Read `skills/taste/SKILL.md` first
2. Follow progressive disclosure — load only relevant files from `engine/`, `modes/`, `recipes/`, `templates/`, `principles/`, `tools/`
3. Do not paste SKILL.md alone into context; the skill needs its supporting folders
```

**Important:** The skill relies on progressive disclosure across multiple folders. Do not flatten or paste only `SKILL.md` — the agent needs access to the full directory structure.

### Claude Code

**Personal install (available in all projects):**

```bash
git clone https://github.com/juanchigallego/Taste.git ~/.claude/skills/taste
```

**Project install (this repo only):**

```bash
git clone https://github.com/juanchigallego/Taste.git .claude/skills/taste
```

Invoke with `/taste` or let Claude auto-invoke when your request matches the skill description. Verify installation with `/skills`.
