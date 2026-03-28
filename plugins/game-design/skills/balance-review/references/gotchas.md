# Gotchas -- Common Mistakes When Evaluating Balance

These are failure modes to watch for in your analysis. Avoid them.

## Vocal minority bias

The loudest feedback comes from the most invested players, who are unrepresentative of the broader playerbase. A highly skilled player calling something "broken" and a casual player calling the same thing "impossible" are both correct for their context. Neither represents the whole. Community channels systematically overweight the most engaged, most vocal segment. If you only optimize for vocal feedback, you systematically underweight the majority of your players.

## Survivorship bias in data

Late-game strategies look strong in aggregate data because only successful players reach the late game. An option that appears powerful may just be correlated with being good at the game, not causing success. Before acting on a metric that shows a late-game option overperforming, ask: is this option strong, or are strong players the only ones who encounter it? These require completely different responses.

## Sampling bias from super-users

Two highly active playtesters generating most of the data can skew metrics dramatically. Always segment data by contributor volume. If removing the top 5% of contributors changes the conclusion, the conclusion was based on outliers, not signal. This is especially dangerous early in development when playtester pools are small -- aggregate averages may just reflect one or two people's experience.

## Passive data beats active feedback for identifying real problems

What players do (behavioral data) is more reliable than what they say (verbal feedback). A player may call a strategy "unfun" while using it every game. Behavior reveals preference; words reveal aspiration. Surveys create cognitive cost that reduces response rate and introduces selection bias. Frictionless data collection that captures every session -- not just sessions from motivated reporters -- produces more representative signal.

## Balance patches can create worse problems than they fix

Weakening one option shifts play to the next strongest. That option may create a worse meta than the original problem. Trace all connected systems before changing one -- the second-order effects are often worse than the original imbalance. The sequence matters: what becomes dominant after your change? If you can't answer that, you're not ready to make the change.

## "Feels unfair" and "is unfair" are both valid but require different solutions

Mathematical unfairness requires tuning numbers. Perceived unfairness may require better communication, more visible feedback, or narrative framing that helps the player understand why they lost. Fixing perception with math (or vice versa) wastes effort. A mathematically fair system that feels unfair will generate the same complaints as an actually unfair one. Diagnose which type of problem you have before choosing a solution.

## Perfect balance can be boring

Asymmetry creates variety and identity. If every character or option performs identically, there's no reason to choose -- and choosing is where engagement lives. Some imbalance creates narratives ("the underdog pick"), preferences ("my main"), and discovery ("I found a strong combo"). The goal is meaningful variety, not mathematical equality. A perfectly flat power curve is a game with no identity.

## Balancing for the top 1% vs. the middle 50%

Changes that create interesting decisions at the highest skill level may destroy fun for average players, and vice versa. A strategy that dominates in expert play may be irrelevant at casual skill levels because it requires execution most players can't deliver. Know which population you're balancing for and be explicit about the tradeoff. If you're not sure, balance for the middle and add difficulty systems that let experts self-sort.

## Confusing "I lost" with "the game is unbalanced"

Players attribute losses to balance problems more readily than to skill gaps. This is human nature, not dishonesty. But loss data alone doesn't indicate imbalance -- only systematic, cross-player, skill-controlled patterns do. If one option shows a high win rate across all skill levels and all contexts, that's a balance signal. If one player lost to it once, that's an anecdote.

## Treating metrics as ground truth without asking why

Metrics show correlations, not causes. An option that appears in winning outcomes at a high rate may be strong, or it may be acquired at a point where winning is already likely. Acting on metrics without investigating the structural reasons behind the numbers leads to nerfing healthy content and buffing content that doesn't need it. Always ask: why is this number what it is?

## Balancing in a vacuum without player data

Theoretical balance analysis has value but sharp limits. Designers cannot simulate the full range of player skill, creativity, and behavior in their heads. An option that looks balanced on paper may be broken in practice because players find uses the designer didn't anticipate. Conversely, an option that looks broken on paper may be fine in practice because it requires setup that most players can't execute. Theory informs hypotheses; data confirms or refutes them.

## Over-tuning based on early data

Early-access or launch-window data reflects a playerbase that hasn't learned the game yet. Options that dominate in week one may be irrelevant by week four as players develop counters and deeper strategies. Resist the urge to patch immediately based on early numbers. Give the meta time to develop unless something is clearly catastrophic.
