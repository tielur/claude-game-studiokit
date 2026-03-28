# Gotchas -- Common Mistakes When Evaluating Feedback Loops

These are failure modes to watch for in your analysis. Avoid them.

## Positive loops aren't inherently bad

The problem isn't amplification itself -- it's whether the amplification involves interesting decisions. A positive loop where each cycle requires new problem-solving is engaging. A positive loop where each cycle is identical repetition is grinding. Don't flag a positive loop as a problem unless you can explain what's missing from the decision-making within it.

## Negative loops that feel like punishment vs. ones that redirect

A negative loop that slows the leader feels like punishment. A negative loop that makes unexplored content more attractive feels like opportunity. The mechanical effect (slow down the leader) can be identical, but the framing changes everything. When evaluating a negative loop, ask whether it closes a door or opens a different one.

## Visibility of negative loops affects player psychology

Hidden rubber-banding feels unfair when discovered because players feel deceived about the rules. Visible catch-up mechanics feel fair because they're part of the known system. If you're recommending a dampening mechanic, consider whether it should be transparent. The default should be visibility unless there's a specific reason to hide it (like dynamic difficulty where transparency would encourage sandbagging).

## Mixed signals are the hardest problem to diagnose

One loop rewards aggression, another rewards caution. Each makes sense in isolation. Together they produce players who feel confused about what the game wants them to do. This failure mode masquerades as "players aren't learning" or "players aren't engaged" -- the real cause is contradictory incentive structures. When a design feels confusing, map all active loops and check for opposing incentives before blaming the player or the tutorialization.

## Feedback loops interact with randomness

A positive loop amplified by lucky RNG creates runaway dynamics much faster than either mechanic alone. A negative loop dampened by unlucky RNG can feel like the game is actively hostile. Don't evaluate loops in isolation from the game's randomness systems. Consider the worst-case interaction: what happens when the positive loop fires on a lucky streak? What happens when the negative loop fires on an unlucky one?

## Early-game loops shape the entire session

Because amplification compounds, the first few turns or minutes disproportionately determine the outcome. If early-game loops are too strong, late-game decisions become irrelevant -- the game was effectively decided before most of the playtime occurred. When evaluating loop strength, weight early-game loops more heavily than late-game ones.

## Removing a loop changes all connected loops

Feedback systems are interconnected. Removing or weakening one loop doesn't just affect that loop -- it changes the balance of every loop it interacts with. A positive loop held in check by a negative loop becomes a runaway problem if you remove the negative loop. Map the full system before recommending changes, and trace the second-order effects of any intervention.

## Confusing "loop exists" with "loop is well-designed"

Identifying that a game has positive and negative feedback loops is not analysis. Every game with persistent state has feedback loops. The analysis is whether those specific loops create the intended pacing, tension, and decision-making -- and if not, why not and what to change. Don't stop at classification.

## Rewarding performance with progression resources creates hidden positive loops

When skilled play earns currency that buys power upgrades, you've built a positive loop into what looks like a neutral reward system. Good players get more resources, buy better tools, need less help. Struggling players get fewer resources, can't buy what they need, fall further behind. Any time performance rewards and progression resources share the same economy, check whether you've accidentally created a compounding advantage for players who already don't need it.

## Assuming the loop resets when the player retries

Positive loops in single-player games often feel fine because death means reloading -- the loop resets. But if the game has persistent progression across attempts (permadeath, carry-over resources, permanent squad loss), the loop doesn't reset on failure. It runs in reverse. Check whether failure actually resets the loop or just flips its direction.
