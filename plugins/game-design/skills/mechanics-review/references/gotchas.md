# Gotchas -- Common Mistakes When Evaluating Mechanics

These are failure modes to watch for in your analysis. Avoid them.

## Genre doesn't determine mechanics

Starting from genre constrains design prematurely. "It's a platformer so it needs double jump" is backward thinking. Genre is a communication tool -- a promise to the audience about what kind of experience to expect -- not a creative constraint that dictates which verbs to include. Start from the desired experience and let mechanics follow. If you remove a genre-standard mechanic, you need to provide something of equal value to the player, but you are not obligated to include it by default.

## Mechanics carry hidden aesthetics from their origin

Borrowing a mechanic imports its emotional weight, pacing expectations, and implied complexity. A deck-building mechanic implies strategic planning even in a casual game. A checkpoint save system implies safety and low-stakes risk even in a horror game. A turn-based structure implies deliberation even in an action-oriented context. You are not just copying a rule -- you are importing an entire causal chain of player behavior and emotion. Trace the MDA chain of any borrowed mechanic before committing to it.

## Simplicity is not shallowness

Few rules with high interaction depth beats many rules with low interaction. A game with 3 mechanics that interact richly is deeper than a game with 30 mechanics that don't. Adding more rules, stats, or systems is not the same as adding mastery potential. Complexity without purposeful interaction creates noise, not depth. When a design feels thin, the fix is usually better-connected mechanics, not more mechanics.

## Mechanics-first thinking is a trap

"What if you could [mechanic]?" produces unfocused prototypes. "What should the player feel?" produces focused designs. The more reliable design path is to name the emotional output first, then work backward: which mechanics and interactions are likely to produce that output? Every design decision should be evaluated against the intended emotional experience, not against whether the mechanic is clever in isolation.

## "Realism" is not a valid design input

"That's not how it works in real life" is never a sufficient reason to include or exclude a mechanic. Systems serve play, not simulation. Setting a jump height because "that's how high a human could jump" has no bearing on whether the mechanic feels good or serves the character fantasy. Realism is only valuable when it improves the play experience. Stylized games succeed precisely because every decision is made in service of the feel, not the physics.

## Non-mechanic elements are direct emotional channels

Music, lighting, camera movement, visual effects, and animation bypass the mechanics-dynamics chain entirely to create emotional states. A mechanic isn't solely responsible for the feeling it produces -- context does much of the work. A heroic soundtrack can make a player feel powerful regardless of what the mechanics are doing. This means a single incoherent non-mechanic element can neutralize carefully designed mechanics. Evaluate every element that produces an emotional signal, not just the rules.

## Aesthetics are non-universal

The same mechanic produces different emotions depending on player skill, context, and preference. What feels like exciting challenge to one player feels like frustrating difficulty to another. Time pressure feels exhilarating to skilled players and anxiety-inducing to struggling ones. This is not a fixable bug -- it's a structural property of emotional design. Define your target audience's skill and context profile early, design for that profile specifically, and accept that the experience will diverge for players outside it.

## Lock mechanic feel before building systems on top

Once systems depend on a mechanic's specific behavior (progression tuned to it, levels designed around it, AI responding to it), changing the mechanic's feel becomes extremely expensive. The feel of the core verb is part of the character of the game. Treating it as polish to address later means reworking foundational design decisions when you discover the feel is wrong. Get the core verb right first, then build systems that depend on it.

## Variable testing reveals more than intuition

When evaluating a mechanic, systematically vary one parameter at a time (speed, range, cooldown, cost) and observe how the feel changes. This is more reliable than gut feeling. Double the value or halve it rather than making small adjustments -- small tweaks assume you're near optimal and mask whether the variable is doing what you think it is. Premature fine-tuning during prototyping wastes iteration cycles converging on a local optimum when a completely different direction would produce better results.
