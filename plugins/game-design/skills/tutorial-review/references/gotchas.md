# Gotchas -- Common Mistakes When Evaluating Tutorials

These are failure modes to watch for in your analysis. Avoid them.

## Under-explaining is the default failure mode, not over-explaining

Designers systematically overestimate how obvious their systems are. After months or years of development, the designer has internalized every mechanic to the point where it feels self-evident. This is a structural bias, not a personality flaw -- it affects every designer regardless of experience. When evaluating a tutorial approach, correct for this bias by assuming the game teaches less than the designer thinks it does. When in doubt, recommend more teaching, not less.

## Players forget tutorials by the time mechanics matter

Teaching a mechanic in minute 1 that doesn't become relevant until minute 30 is wasted teaching. The player has no context for why the information matters, no immediate way to practice, and no reason to retain it. By the time the mechanic appears in real gameplay, the tutorial is gone from working memory. The fix: teach just before the mechanic matters. Proximity between instruction and application is the single strongest predictor of tutorial effectiveness.

## "Intuitive" to the designer is not intuitive to the player

The designer has played the game hundreds of times. What feels natural to them is foreign to a first-time player. "This mechanic is intuitive" is never a valid design claim -- it's a hypothesis that only playtesting can confirm. When you see a design that assumes a mechanic is self-explanatory, flag it. The designer's intuition about intuitiveness is the least reliable data point available.

## Text tutorials are not teaching -- they're documentation players skip

A wall of text before gameplay begins is the least effective teaching method. Players skim or dismiss text popups because they want to play, not read. If a design can only teach a mechanic through text, that's a signal the mechanic may need redesigning -- or at minimum, the teaching method needs to change. Text should be a last resort after environmental teaching, contextual prompts, and demonstration have been considered and rejected for specific reasons.

## Teaching one mechanic at a time even when mechanics interact

Players can absorb one new concept per teaching moment. If two mechanics interact, teach each one separately first, then introduce their interaction as a third, distinct teaching moment. The sequence: learn A, learn B, learn A+B. Trying to teach the interaction before both components are understood forces the player to learn three things simultaneously, which reliably produces confusion.

## Accessibility settings are a form of teaching

Making a mechanic adjustable communicates what the game considers core (the parts that can't be adjusted) vs. peripheral (the parts that can). This teaches design philosophy, not just difficulty. When evaluating tutorial design, check whether the assist mode options are consistent with what the game is trying to teach. If the game's identity is built around a mechanic that the assist mode trivializes, the assist mode is undermining the game's own teaching.

## Tutorial necessity scales with information criticality, not complexity

A simple mechanic that's critical to survival needs explicit teaching. A complex mechanic that's optional and discoverable doesn't. The instinct is to tutorial complex things and skip simple things, but complexity is the wrong variable. Criticality is what matters: how much does the player's experience suffer from not knowing this? A one-button mechanic that's invisible and essential is a higher teaching priority than an elaborate system the player can experiment with at leisure.

## Restarting is not a substitute for teaching

If players learn by dying and restarting, they're learning through punishment, not teaching. This is a valid design choice for some genres -- games built around mastery through repetition use death as a core teaching mechanism. But it should be a conscious choice, not an accident. If the game isn't designed around the restart loop, forcing players to learn by failing means the tutorial has failed. Check whether death-as-teaching is intentional and genre-appropriate, or whether it's papering over a gap in onboarding.

## Front-loading tutorials creates the worst first impression

The first minutes of gameplay should be the most compelling. This is when the player is deciding whether to continue. Pausing gameplay for instruction during this window costs disproportionate engagement. Every second spent on a tutorial screen in the first five minutes is a second the player isn't experiencing what makes the game worth playing. Spread teaching across the first hour rather than concentrating it at the start. Drip-feed mechanics as they become relevant rather than dumping everything upfront.

## Confusing "players will figure it out" with "players don't need to know"

These are different claims. "Players will figure it out" means the information is discoverable but not taught -- the player spends time and effort finding the answer. "Players don't need to know" means the information is genuinely unnecessary for a good experience. Designers frequently use the first to justify skipping a tutorial when what they actually mean is "I don't want to build this tutorial." If not knowing a mechanic makes the game less enjoyable while the player figures it out, the designer has offloaded their communication obligation onto the player's time.

## Teaching genre conventions to genre veterans

If the target audience has played similar games, teaching mechanics that conform to genre conventions wastes time and feels patronizing. Genre veterans will assume standard behaviors (dodge rolls have invincibility frames, red barrels explode, glowing objects are interactable) without instruction. Teaching these things signals that the game doesn't trust or understand its audience. Save tutorial effort for mechanics that deviate from convention -- those are the ones that actually need teaching.
