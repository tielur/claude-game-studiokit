# Mechanics Review Framework -- Reference

## Rules, Mechanics, Systems Hierarchy

These are three distinct layers with a strict build-order dependency:

- **Rules** define the possibility space -- conditional logic that determines what is and isn't allowed. "When X, then Y."
- **Mechanics** are verbs -- the actions players take within the rules. Jump, trade, build, aim, dodge, bluff.
- **Systems** are emergent interactions between mechanics -- economy, combat meta, social dynamics, progression arcs.

Rules are the foundation. Mechanics depend on rules. Systems depend on mechanics. Design bottom-up: get rules right, then mechanics, then systems. Building systems before mechanics (proc-gen engines, progression frameworks, AI directors) means building infrastructure for a product that hasn't been designed yet. The system's requirements can't be specified until the mechanics are known.

## Core Mechanic Isolation Test

Strip everything away -- no progression, no narrative, no polish, no secondary systems. Is this mechanic fun with nothing else around it? If the core verb is satisfying in isolation, the game has a foundation. If it requires external reward to be worth doing, the mechanic is weak.

This is the single most important diagnostic. When a game feels boring, the instinct is to add more content, systems, or features. But if the core mechanic isn't engaging on its own, layering secondary mechanics on top masks the problem without solving it. Players eventually reach the core and the game collapses. Fix the verb first.

## Easy to Learn, Hard to Master Diagnostic

Evaluate three properties:

- **Low floor** -- can a novice engage immediately without instruction?
- **High ceiling** -- does a skill ceiling exist that rewards continued investment?
- **Depth** -- is the gap between floor and ceiling filled with discoverable techniques?

If floor and ceiling are close together, the mechanic is shallow -- it will be mastered quickly and offer no reason to return. If the floor is too high, the mechanic is inaccessible -- players bounce before they experience what makes it interesting. Both are problems.

A mechanic being easy to describe does not mean it lacks mastery potential. Simple verbs (attack, dodge) can produce extraordinary depth when they interact with precise surrounding systems (stamina management, enemy design, timing windows). Depth comes from interaction, not from the complexity of any single action.

## Mechanic Transplant Checklist

When borrowing a mechanic from another game or genre, answer these before implementing:

1. **What hidden dependencies does it carry?** What other systems made it work in its original context? A mechanic that feels great in one game may rely on surrounding systems you didn't copy -- pacing, resource pressure, information flow.
2. **What aesthetics does it imply?** A turn-based system implies deliberation and planning. Real-time implies reflexes and pressure. Deck-building implies strategic accumulation. These emotional expectations come bundled with the mechanic.
3. **What player expectations does it set?** Players who recognize the mechanic will expect its typical context, feedback patterns, and depth level. Violating those expectations requires deliberate compensation.
4. **What did you leave behind?** The mechanic worked because of an ecosystem. Identify what you didn't copy and determine whether your game provides functional equivalents.

A mechanic only has meaning inside a system. Evaluating it in isolation from its original context is incomplete. A bolt isn't a machine part until it's inside a machine -- and transplanting it into a different machine requires verifying it fits.

## Cognitive Verbs as Player Mechanics

Mechanics aren't limited to physical actions mapped to button presses. Cognitive verbs are equally valid player activities: anticipate, deduce, bluff, memorize, prioritize, negotiate, empathize, judge, notice.

These are especially important for narrative and social games where physical interaction is minimal. A game where the player "just walks and reads" may actually be asking them to deduce what happened, judge a character's honesty, or reconstruct a timeline. These are designed activities, not passive consumption.

When evaluating mechanics, ask: what is the player doing in their head? If the answer is "nothing -- they're waiting for the next prompt," the mechanic has a cognitive engagement gap.

## Emergent vs. Designed Mechanic Distinction

- **Designed mechanics** are authored by the developer -- predictable, testable, directly specified.
- **Emergent mechanics** are discovered through play -- they arise from system interaction, often surprising both players and developers.

Emergent mechanics are typically more replayable but harder to balance. The best designs create conditions for emergence rather than trying to author every interaction. A small number of well-connected mechanics produces more emergent situations than a large number of isolated ones.

The key question for emergent behavior is not "did we intend this?" but "does this emergent behavior produce aesthetics consistent with our goals?" Unintended mechanics that serve the vision should be preserved. Those that contradict it must be removed regardless of how technically impressive they are.

## MDA Coherence Check

The Mechanics-Dynamics-Aesthetics chain:

- **Mechanics** produce **Dynamics** -- patterns of play that emerge from the rules
- **Dynamics** produce **Aesthetics** -- the emotional experiences the player has

Work backward from intended aesthetics: what dynamics would produce them? What mechanics would produce those dynamics?

For any mechanic, trace the full chain:
1. Identify the mechanic precisely (the rule, stat, or system)
2. Predict the player behavior it incentivizes or enables (dynamics)
3. Name the specific emotion that behavior produces (aesthetics) -- avoid vague terms like "fun"; use: powerful, fearful, crafty, tense, isolated, curious, flustered, etc.
4. Ask: does that emotion complement or conflict with the game's vision?
5. If it conflicts, change or cut the mechanic regardless of how standard or expected it is

**Incoherence** is the primary failure mode: mechanics that produce dynamics at odds with the intended emotional experience. Two mechanics that individually seem reasonable can produce contradictory aesthetics when combined -- one making the player feel vulnerable while another makes them feel unstoppable. Audit mechanics in combination, not just individually.

## Degenerate Strategy Test

Does optimal play conflict with the intended experience? If the most efficient strategy is boring, repetitive, or bypasses the core fantasy, the mechanics have a degenerate strategy problem. The game is telling players to have fun while the math tells them to grind.

This is not an exploit problem -- it's a design problem. A mechanic that makes a cowardly, tedious, or immersion-breaking approach the rational strategy will undermine emotional design regardless of intent. The fix is not to patch the exploit; it's to redesign the mechanic so that rational play aligns with intended emotion.

Ask: what is the rational, optimal strategy this mechanic creates? If that strategy produces an emotion that conflicts with the vision, the mechanic will undermine the experience even when used "correctly."

## Expressive Mechanics

Interactions that serve identity and self-expression rather than progression: character customization, emotes, building aesthetics, movement style, cosmetic choices, environmental interaction with no gameplay consequence.

These are not frivolous -- they're how players make the game "theirs." Free-form play (messing around, petting the cat, smashing empty boxes) is an expected dimension of experience, not a luxury layer. Games that are mechanically tight but have no room for self-expression consistently feel bare-bones to players even if they can't name why.

After core mechanics are solid, audit for expressive potential:
- Can the player do anything that doesn't help them win?
- Can the player leave a mark on the world the game doesn't formally acknowledge?
- Is there anything cosmetic, silly, or low-stakes the player can engage with?

If all answers are no, the game will likely feel sterile.

## Variable Testing Heuristic

When evaluating a mechanic's parameters, don't make small adjustments. Double the value or halve it first. Small tweaks carry the implicit assumption that you're already close to optimal. Extreme changes reveal the actual effect of the variable and expose whether the rule is doing what you think it is.

Systematically vary one parameter at a time (speed, range, cooldown, cost, duration) and observe how the feel changes. This is more reliable than gut feeling and reveals which variables actually matter versus which are noise.
