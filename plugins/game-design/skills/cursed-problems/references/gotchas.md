# Gotchas -- Common Mistakes When Evaluating Cursed Problems

These are failure modes to watch for in your analysis. Avoid them.

## Trying to solve instead of work around

This is the defining trap. When a problem is truly cursed, no amount of clever design eliminates the conflict. The solution always seems just one tweak away -- teams can spend months or years searching for answers that structurally cannot exist. Recognize the curse, then shift to workaround strategies. Suggesting "just balance it better" for a cursed problem wastes everyone's time.

## Not mapping promises explicitly before designing

Identify the game's player promises first, both the designer's intended promises and the promises players will infer from the mechanics. Skipping this step means diagnosing symptoms instead of the underlying conflict. Write the promises down as a list before evaluating anything.

## Seeing every design conflict as cursed

Most design problems ARE solvable. A problem is only cursed when two core promises fundamentally contradict each other such that fulfilling one inherently breaks the other. If the conflict can be resolved by tuning numbers, adding content, or improving execution, it's hard, not cursed.

## Confusing "technically possible" with "promise kept"

A promise is broken when the optimal strategy bypasses the promised experience, not when the behavior is technically impossible. If a game promises creative freedom but the optimal path is a solved sequence, the promise is broken even though creative play is "allowed." In a free-for-all brawler, players technically fight -- but if the optimal strategy is politics, the game is a politics game with fighting as decoration. The test is whether the golden path includes the promised experience, not whether a player could theoretically choose it.

## Thinking efficient markets can be tuned into loot systems

When players can trade freely, every item has a known market value. Monsters effectively drop currency, not items. The surprise and delight of loot discovery is structurally incompatible with frictionless trading -- this is a property of efficient markets, not a tuning knob. Adjusting drop rates, adding trade fees, or limiting transaction volume are all attempts to add friction to the market, and friction fights the market promise. The incompatibility is structural. Recognize it as a choice between two promises rather than a balance problem.

## Choosing barriers when gates would preserve more

Barriers are the bluntest instrument. They remove the problematic behavior entirely, but they also remove whatever was fun about that behavior. Before recommending a barrier, check whether a gate could reduce the problem to a tolerable level while preserving more player expression.

## Ignoring that player promises evolve over time

A game's promises aren't fixed at launch. Players develop new expectations as they master systems, as the community develops meta-strategies, and as the game updates. A conflict that didn't exist at launch can become cursed as the player base matures and optimal strategies become dominant patterns. Skill inflation is the clearest example: the promise of a welcoming community only conflicts with the mastery promise after the skill floor rises.

## Treating the sacrifice as failure

Successful cursed problem resolution often means abandoning the original dream for something better. The games that successfully navigate cursed problems did not fail to make the original game -- they made better games by embracing a different set of promises. The frame "we gave up on X and got Y" is more productive than "we failed to make X." The sacrifice is not "the game you couldn't make" but "the constraint that produced the game you did make."

## Not recognizing player-inferred promises

Players infer promises from mechanics whether the designer intended them or not. A leaderboard promises that ranking matters. A character creator promises that expression matters. A co-op mode promises psychological safety. Player promises don't require designer intent -- they just require plausibility. If your mechanics imply a promise, players will hold you to it even if you never stated it. Evaluate the promises the game actually makes through its systems, not just the promises the designer wrote in the design document.

## Missing that the same mechanic can serve conflicting promises in different contexts

A scoring system promises competition in one game and promises personal mastery tracking in another. A trading system promises social interaction in one game and commodifies loot in another. Evaluate promises in context. The same mechanic isn't inherently cursed; it depends on what other promises surround it.

## Adding objectives to a creative game without accounting for extrinsic goal dominance

Any progression system, career track, or achievement layer added to a creative game will tend to subsume the creative experience. The extrinsic goals don't just "add structure" -- they redirect player motivation entirely. If you want a creative game to stay creative, you either remove objectives entirely or use the carrots technique to make creativity itself the objective.

## Assuming transparency always improves games

Showing players' scores, rankings, or performance data helps in many contexts -- but in competitive formats prone to political targeting, it enables players to identify and gang up on the leader. Visible leaderboards in a free-for-all directly incentivize political play against the strongest player. Hiding information is sometimes a feature, not a limitation.
