# Gotchas -- Common Mistakes When Evaluating Randomness

These are failure modes to watch for in your analysis. Avoid them.

## Treating all randomness as bad
Randomness serves real design purposes -- variety, balance, rewards, and information management. The question is never "should this game have randomness?" but "is the randomness well-placed and well-controlled?"

## Ignoring the input/output distinction
Saying "this game has too much RNG" without specifying whether it's input or output randomness is vague and unhelpful. The two types create fundamentally different player experiences and require different fixes.

## Assuming output randomness is always wrong
Output randomness is a valid design tool. It simulates imprecision in abstract systems, forces contingency planning, and creates tension. The problem isn't output randomness itself -- it's output randomness without transparency, guardrails, or player recourse.

## Probability is reliably misperceived -- design around it, not just display it
A displayed 90% hit chance feels like certainty to most players. A miss at 90% feels like betrayal, not statistics. Showing accurate numbers satisfies a transparency requirement but does not fix the psychology problem. Some games display one number and compute a more generous number behind the scenes to match player expectations. Evaluate whether the design accounts for how humans actually perceive probability, not just whether the math is disclosed.

## Binary output randomness is uniquely punishing
A complete miss (zero damage, no effect) feels dramatically worse than a partial hit (reduced damage) even at identical expected values. Binary randomness communicates "nothing happened" rather than "something happened, just less." A total miss after a committed decision tells the player their choice produced no outcome at all, which is a direct attack on perceived agency. Partial-hit systems (grazing shots, reduced effects, diminished returns) preserve the sense that the player's decision mattered even when luck was unfavorable.

## Too much information is a design failure
Complete transparency can be as damaging as too little information. Perfect information games with many options per turn can paralyze players -- they spend excessive time calculating optimal moves because all the data is visible and the "correct" choice is theoretically findable. Strategic hiding of some random information keeps decisions tractable. The goal is managed information flow, not maximum information.

## Overlooking restart-scumming incentives
If input randomness heavily determines success (a powerful early item, a favorable starting map), players will restart repeatedly until they get favorable RNG. This turns a roguelike into a slot machine. Check whether the design inadvertently rewards this behavior.

## Early input randomness can predetermine entire runs
If the first random event has outsized impact -- an extremely powerful early item, a map layout that trivializes the first several challenges -- mediocre starts feel "already lost" even if comeback is theoretically possible. Players disengage because the run already feels decided. This is not fixed by making the powerful outcome more common (that just shifts the restart threshold). It requires either removing outsized early advantages or ensuring that early variance doesn't compound multiplicatively across the rest of the run. Weight early randomness carefully.

## Output randomness that only benefits the player produces zero complaints
Surprise positive events (critical hits, bonus drops, lucky saves) generate excitement. Surprise negative events generate frustration. This asymmetry is reliable and exploitable. Asymmetric randomness -- positive outputs combined with strategic inputs -- is a viable design pattern. When reviewing a design, check whether output randomness is symmetrically applied (positive and negative surprises) or asymmetrically applied (only positive surprises). If the design uses symmetric output randomness and players are frustrated, shifting to asymmetric positive-only outputs is often a higher-leverage fix than removing the randomness entirely.

## Forgetting controlled variance
Pure randomness creates streaks that feel broken. If a design uses randomness without any shaping, that's usually the highest-leverage fix. Point to specific techniques rather than just saying "make it less random." Match the technique to the context: bag systems suit repeated small events, pity timers suit rare high-value events, weighted distributions suit ongoing drop rates, and distributed shuffling suits pacing over time.

## Confusing legibility with simplicity
Making randomness legible doesn't mean dumbing it down. Cards, dice, and displayed percentages help players understand probability without reducing strategic depth. Suggest mechanisms that make odds intuitive, not mechanisms that remove decision-making. Suggesting that a game remove displayed percentages because they're "confusing" is the wrong fix -- the fix is making the percentages more intuitive (visual indicators, familiar mechanisms, contextual framing).

## Ignoring multiplayer dynamics
Randomness in multiplayer games has a fundamentally different character than in single-player. A lucky roll that helps one player directly hurts another -- the emotional impact is doubled. Competitive multiplayer demands tighter variance control and more transparency because the perceived unfairness isn't just "the game screwed me" but "the game gave my opponent an unearned advantage." Analyze multiplayer randomness from all players' perspectives, not just one.

## Suggesting "remove the randomness" as a fix
Removing randomness entirely often makes games worse -- perfectly deterministic games can become solvable puzzles or pure execution tests. The fix is usually better-placed, better-controlled randomness, not less of it.
