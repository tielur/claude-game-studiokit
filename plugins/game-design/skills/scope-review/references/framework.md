# Scope Review Framework

Scope review operates in two phases. Phase 1 asks whether the team is choosing the right scope. Phase 2 asks whether that scope is achievable. Most projects fail Phase 1 -- they pick scope based on ambition rather than capability and constraints.

## Phase 1: Scope Selection (via Constraints)

### The Craftsperson's Three Questions

Before evaluating any game concept, the team should be able to answer:

1. **What can I execute well right now?** Not aspirationally -- what has been demonstrated through finished work.
2. **What do I want to learn that won't obviously weaken this project?** Learning is valid scope, but only if the learning area isn't load-bearing. A first attempt at networked multiplayer shouldn't also be the game's core differentiator.
3. **What should absolutely NOT be in this project?** Skills so underdeveloped that including them guarantees a weak subsystem. Any game concept that requires answering "I'll figure out #3 as I go" is the wrong game to make.

### Constraint-Theme Coupling as Ideation Method

Constraints aren't obstacles to design around. They're the blueprint for what matters.

1. **Identify developer constraints** -- what the team can't or won't do given skills, budget, timeline, and tools
2. **Pick one core mechanical constraint** that limits scope (single screen, no characters, one weapon, one level, no dialogue)
3. **Research how others have worked within it** -- collect games that share the constraint, study their interaction models
4. **Couple the constraint with a theme that justifies it** -- the theme should make the constraint feel intentional rather than limiting
5. **Validate the pairing** -- would the constraint read as a feature on a store page? If you can't describe it as a deliberate design choice in marketing, it will read as a limitation to players

The resulting idea should be small enough to prototype quickly and testable before any content is added.

### Quality Density

Small scope doesn't mean "less game." It means competitive quality in every subsystem.

Every subsystem in a game competes independently against other games. If your UI is worse than another game's UI, if your writing is weaker than another game's writing, players notice each one separately. A smaller game concentrates limited skills and time into fewer systems, making each one more likely to be competitive. The goal is density, not breadth. Scope reduction is a quality strategy, not just a completion strategy.

### Theme as Scope Control

A strong theme constrains what belongs in the game and resets player expectations about content volume.

A creature-collecting game with 50 creatures will disappoint players who expect hundreds -- unless the theme implies a naturally bounded pool. A necromancer game with 50 undead creatures, or a dinosaur game with 50 species, meets expectations because the theme defines the boundaries. The developer constraint (can't make hundreds of creatures) is absorbed by the theme rather than exposed as a shortcoming.

Theme is a scope tool, not flavor. Choosing the right theme can make a hard limitation feel like a deliberate and satisfying design choice.

### Friction Intentionality Check

For every constraint in the design, ask: is this serving the theme (making the game better), or is it just a limitation?

- **If serving theme:** The constraint is scope-defining. It shapes what the game is. A game where everything happens on the water because the team can't animate walking characters -- and the theme makes that feel intentional -- is using the constraint correctly.
- **If just a limitation:** It needs thematic justification or cutting. A constraint that players can't see a reason for reads as laziness or an unfinished game. The constraint itself doesn't change -- only the presence or absence of a player-facing justification changes perception entirely. If the justification isn't visible on the store page, it isn't working.

## Phase 2: Scope Verification (via Simplification)

### The Simplification Algorithm

An iterative process with a concrete stopping condition:

1. **Add mechanics** until the design feels complete
2. **Cut mechanics** until something breaks -- until removing one more thing would compromise the core experience
3. **Add back the last thing you cut** -- you're now at minimum viable complexity
4. **Repeat** until done or out of resources

**Stopping condition:** If you didn't add back at least 10% of what you cut, you probably didn't cut enough. Most designers under-cut. The instinct is to preserve; the discipline is to remove.

### "Here Lies" Pre-Mortem with Reframing

Most teams encounter constraints late and experience them as surprises. The pre-mortem surfaces them early, when you can design with them rather than against them.

1. At project kickoff (or when scope feels uncertain), write: "Here lies this project, killed by..."
2. Brainstorm every realistic cause of death: technical risk, budget, content pipeline, team attrition, market timing, platform constraints
3. **For each cause of death, reframe it as a design constraint or prioritization criterion.** This is the key step -- it converts anxiety into actionable scope decisions. "Killed by too many branching paths" becomes "every branch must earn its existence." "Killed by art volume" becomes "art style must minimize per-asset cost."
4. Use the resulting list as a filter: ideas that can't survive these constraints don't advance
5. Revisit the list when scope creep or new ideas threaten to resurrect killed features

### Feature Dependency Mapping

Which features require other features to function? Map the dependency graph.

- **Cut dependencies first, standalone features last.** If feature B requires feature A, and feature A slips, feature B is blocked. Interconnected features create cascading risk.
- Independent features are structurally safer -- they can be cut, deferred, or simplified without breaking anything else.
- If a feature can't be cut without breaking multiple other features, it's either core (keep it) or a dangerous coupling (redesign it).

### Content Pipeline Reality Check

How many unique assets does each feature require? This is where scope estimates die.

- Count the distinct assets: sprites, animations, sound effects, dialogue lines, level layouts, UI screens
- Multiply by iteration cycles -- first drafts rarely ship. Budget 2-3 passes minimum for any visible asset.
- Art pipelines are the most commonly underscoped system. Each unique visual requires concept, production, iteration, and integration across multiple contexts (menus, gameplay, marketing).
- Code can be refactored and mechanics simplified, but if the game needs 200 hand-painted backgrounds at 8 hours each, that's 1,600 hours of art before iteration.

### Technical Risk Inventory

What has the team never built before?

- Each first-time system costs 3-5x the estimate. This isn't pessimism -- it's the cost of learning while building.
- New engines, frameworks, platforms, or custom tech multiply scope unpredictably. Every unknown technology is a scope risk until prototyped.
- Prototype the riskiest technical element first. If it doesn't work, you want to know before building everything around it.
- Engine or tool upgrades mid-project create invisible maintenance burden. Every downstream system that depends on the upgraded component needs testing, and often fixing. Budget for this explicitly or freeze tools early.
