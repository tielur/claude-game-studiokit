# claude-game-studiokit

This is a Claude Code plugin marketplace for game design skills. The marketplace name is `claude-game-studiokit`.

Plugins live in the `plugins/` directory. The marketplace catalog is at `.claude-plugin/marketplace.json`.

## Skill structure

Each skill lives in `plugins/<plugin>/skills/<skill-name>/` and contains:

- `SKILL.md` — YAML frontmatter with a `description` field, followed by markdown instructions.
- `references/` — Supporting markdown files (e.g., `framework.md`, `gotchas.md`) that the skill references for detailed guidance.

## Writing skills

- **The `description` field is for triggering, not summarizing.** Claude scans skill descriptions to decide whether a skill matches the user's request. Write it as "use when the user wants X" rather than a generic summary.
- **Gotchas are the highest-signal content.** Build up `references/gotchas.md` from real failure modes Claude hits. Update it over time as new edge cases appear.
- **Use progressive disclosure.** Don't put everything in SKILL.md. Point Claude to reference files and let it read them when relevant. The `references/` folder is context engineering.
- **Don't state the obvious.** Claude already knows a lot about game design. Focus on information that pushes it out of its default thinking — uncommon frameworks, counterintuitive principles, specific gotchas.
- **Avoid railroading.** Give Claude the information it needs but the flexibility to adapt. Skills are reusable across many contexts, so overly specific instructions will break in edge cases.

## README conventions

- Use the exact plugin name (e.g., "game-design" not "Game Design") when referring to plugins.
- Skill descriptions in the table should avoid em dashes. Use ", including" instead.
- Each plugin section includes an intro line: `<plugin-name> plugin includes the following skills:`
