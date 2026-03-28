# Design Discovery Framework

## Core Methodology: Fail Fast, Follow the Fun

1. **Prototype** -- build something playable as fast as possible. The starting idea does not need to be good, original, or complete. Many of the most celebrated games began with loose, derivative, or fuzzy premises. The quality came from iteration, not from the seed.
2. **Play** -- test it yourself, watch others play it.
3. **Recognize emergent fun** -- identify what's enjoyable, especially the unintended parts. The most fun mechanic in your prototype is probably not the one you planned.
4. **Redesign around it** -- strip everything that doesn't support the interesting thing. Let the implications of that mechanic generate the next layer of design decisions.

This is bottom-up discovery, not top-down design. The designer's role is curatorial: recognize what the game is telling you, then shape it.

## The Vertical Slice Rule

Build the smallest playable slice. Make it genuinely excellent -- feel, decisions, interactions. THEN add content. Never scale mediocre.

1. Build the smallest possible playable slice (one level, one scene, one mechanic).
2. Make that slice feel genuinely good -- game feel, player decisions, core interactions.
3. Only then add content: more levels, enemies, weapons, story, environments.
4. More content on a mediocre core produces a longer mediocre experience. Content amplifies what's already there -- if what's there isn't fun, more of it doesn't fix the problem.

## The "But" Test for Engagement

Write one sentence describing what the player is trying to do. If "but" appears (competing objectives, opposing forces), you have tension. If not, you likely have pure challenge with narrow appeal.

- **Weak:** "You fight enemies to survive as long as possible."
- **Strong:** "You earn upgrade currency by saving houses, *but* saving houses means leaving your advantageous defensive position."

The presence of a "but" signals interesting decisions. Its absence signals a game that relies on difficulty alone, which appeals to a narrower audience.

## Central Fantasy Question

Before designing mechanics, articulate what the player gets to be or do in real-life-adjacent terms that sound appealing to non-gamers. "I get to look after a cool car in a weird apocalyptic zone." "I get to build and defend an island against an invasion." If you can't answer this in a sentence that sounds appealing to someone who doesn't play games, the premise probably isn't strong enough yet.

This forces appeal clarity before mechanics. It also functions as a constraint that speeds later iteration -- every mechanical decision can be tested against the central fantasy.

## The Funnel Model of Appeal

- **Wide end** (reaches most people): theme, premise, art style, central fantasy.
- **Narrow end** (reaches people already interested): mechanics, systems, challenge structure.

Design the wide end first. The narrow end only matters to people who already came through the wide end. Technically skilled developers systematically underweight the wide end because it's outside their core competency.

## Bugs Become Features

Unintended behaviors are data about what's fun. Ignoring them throws away the most valuable signal a prototype produces.

- Combat bugs that let players juggle enemies in the air have become the central mechanic of entire franchises.
- Physics forces applied to vehicles for boost have produced unintended aerial maneuvers that became a game's signature depth.
- Games intended as exploration sandboxes have accidentally become horror games when the tone that emerged from play was more compelling than the original intent.
- Rhythm-based gameplay has emerged from prototypes where fixed turn timers created an unintended musical quality.
- Player-discovered exploits and unintended strategies have been leaned into rather than patched out, pushing games toward psychological depth.

Before fixing any bug, play it deliberately. Ask: is this interesting? Does it create player agency, depth, or unexpected interaction? If a bug makes the game more fun than the intended mechanic, the bug is the design.

## Emerging Complexity Checklist

Ask of any candidate mechanic or rule:

- Does combining this rule with existing rules produce behaviors or strategies that weren't explicitly designed?
- Does the configuration space grow combinatorially (not linearly) as rules are added?
- Would a human opponent create meaningful variety that the designer couldn't author?

If yes to any of these, the rule likely produces emergent complexity -- the kind that sustains replay indefinitely. Simple intersecting systems that produce rich player behavior last longer than any amount of authored content. Prefer these over rules that add designed complexity.

## Thematic Anchors and Fixed Constraints

Before or during early iteration, identify one thing that cannot change -- a theme, an emotion, a core player fantasy, a constraint. This anchor should be abstract enough to permit many mechanical expressions, but specific enough to rule out a large class of ideas.

Fixed constraints amplify iterative freedom. Anchoring one element narrows the search space. This makes iteration faster, not slower, because every design question filters through the constraint, reducing the option space to a manageable size. When two candidate directions seem equally interesting, ask which one serves the anchor.

A well-chosen theme also functions as scope control. It reduces the design surface area while making the game more distinctive -- you don't need to build systems for everything, only for what the theme demands.

## The White-Hot Magma Phase

Treat early development as a high-malleable period where radical pivots are cheap.

- **Pre-production:** Maximum flexibility. Follow the fun aggressively. This is when the game can still become anything. Biggest changes happen here.
- **Mid-production:** The game's identity is more established. Watch for mechanics that players enjoy more than the intended core. Mid-production pivots are expensive but sometimes necessary -- the cost of ignoring the signal is higher than the cost of the pivot.
- **Late production:** The fundamental design is locked. Follow-the-fun now guides individual content pieces, player-discovered exploits, tonal direction, and feature prioritization rather than core mechanics.

"Follow the fun" applies across the full development arc. Not just early prototyping. The same methodology (play, observe, redirect) is valid for puzzle generation in a mature engine, content design late in production, and tonal refinement near ship.

## Techniques for Faster Iteration

### Game Jams

48-hour forced constraints with no long-term commitment. The time pressure forces rapid prototyping and immediate play -- the ideal conditions for design discovery.

### Rapid Prototyping Tools

Game Maker, Godot, paper prototypes, physical materials. Build simple custom level creation tools so the whole team can experiment with mechanics. Use borrowed sprites or placeholder characters -- the goal is speed, not originality.

### Placeholder Assets

Do not wait for art. Use programmer art, borrowed sprites, or boxes. The goal is to get to the play step as fast as possible. Feel matters; visuals do not -- yet.

### Simplification as Iteration

Find the fun. Add features for depth and variety. Then simplify by cutting mechanics until something breaks. Add back the last thing you removed -- you are now at minimum viable complexity. If you didn't end up adding back at least 10% of what you cut, you didn't cut enough.
