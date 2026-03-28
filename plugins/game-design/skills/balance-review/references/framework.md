# Balance Framework -- Reference

## What Balance Actually Means

Balance does not mean "everything is equal." It means every piece has a reason to exist and no single option dominates all decisions. A balanced game has meaningful choices -- each option has contexts where it's the best pick. Some options are build-arounds, some are staples, some are situational. Conflating balance with equality leads designers to homogenize content and destroy strategic diversity.

The real balance metric is not mathematical equality -- it's decision-making density. If one path is obviously dominant, decision density drops. If all options have genuine tradeoffs, decision density is high. This is what "balanced" should mean in practice.

## The Warping Effect Test

The primary diagnostic for balance problems:

1. Identify the suspect option (the one that seems too strong or too prevalent).
2. Ask: does choosing this option dominate build/strategy decisions regardless of context?
3. If it's always correct to pick this option no matter the situation, it warps the decision space. Other options stop being real choices.
4. The removal test: mentally remove the suspect option. Do the remaining decisions become more interesting? If yes, the option is warping.

Warping is the specific failure mode to watch for. An option that's strong in specific contexts is fine. An option that's strong in all contexts collapses the decision space.

## When Overpowered Content Is Acceptable

In high-variance genres where discovering powerful combinations IS the game, overpowered combos are features, not bugs. The distinction:

- **Warping** -- the powerful option is easy to access and always correct. Players route all decisions toward it. Strategic diversity collapses. This is a problem.
- **Discovery** -- the powerful option is rare, hard to assemble, or requires specific setup. Finding it rewards skilled play or fortunate circumstances. This is a feature.

The test: can the player reliably pursue this option every time, or does it emerge from specific conditions? If it's reliably pursuable and always optimal, it warps. If it requires active discovery or setup, it rewards.

In single-player or run-based games, the structure itself does balance work that competitive games must do manually. A wildly powerful combo that you can't guarantee assembling is a reward for skilled setup, not an exploitable problem.

## Layered Feedback Architecture

Balance data quality depends on collection method. From most passive (highest volume) to most active (highest per-session insight):

1. **Anonymous aggregate metrics** (win rates, pick rates, completion rates) -- highest volume, lowest bias. Every session contributes data whether the player gives feedback or not. Use for identifying systematic patterns.
2. **Automated feedback tools** (in-game surveys, frictionless feedback bots, rating prompts) -- medium volume, some selection bias. Making submission easy reduces the gap between who plays and who reports. Use for quick sentiment on specific changes.
3. **Community channels** (forums, social media, streamer commentary) -- low volume, high vocal minority bias. Streamers narrate their full internal monologue for an audience, producing rich qualitative signal. But community channels systematically overweight invested, high-skill players. Use for qualitative insight, not representative sentiment.
4. **Direct observation** (watched playtests, developer play, attended events) -- lowest volume, highest insight per session. Subjects often hold back criticism when the developer is present. Use for deep qualitative understanding of specific interactions.

Use all layers. Never rely on one alone. What players do (behavioral data) is more reliable than what they say (verbal feedback). A player may call a strategy "unfun" while using it every game. Behavior reveals preference; words reveal aspiration.

## Interpreting Metric Anomalies

Before acting on any metric, ask: is there a structural reason for this number that isn't about the option's actual power?

- **Survivorship bias.** Late-game options look strong in aggregate because only successful players reach the content where they're available. An option that appears powerful may just be correlated with being good at the game, not causing success.
- **Discoverability masquerading as weakness.** Low pick rate may mean players don't know an option exists or don't understand it, not that it's underpowered. Check whether the option is visible and comprehensible before concluding it needs a buff.
- **Indirect patch effects.** Sudden metric shifts after changes may be second-order effects. You changed option A, but option B depended on A. Always trace connected systems before attributing metric changes to the thing you changed.
- **Correlation without causation.** A strong correlation between an option and success doesn't prove the option causes success. Segment data by player skill, progression stage, and playtime before drawing causal conclusions.
- **Contributor distribution skew.** If a small number of highly active players generate most of the data, aggregate averages reflect their experience, not the broader population. Always check: if you remove the top 5% of contributors, does the conclusion change? If yes, the conclusion was based on outliers.

The investigation sequence: notice the anomaly, check for structural confounds, segment by relevant variables, and only treat the metric as actionable signal if no confounding cause explains it.

## Self-Selecting Difficulty as Design Tool

Players naturally find their challenge level if options exist. Rather than prescribing difficulty tiers, design option sets where some are inherently harder to use effectively. Players self-sort without being told they're on "easy" or "hard."

Incremental, unlockable difficulty systems serve double duty: they're content for players (something to climb toward) and data segmentation tools for designers (natural skill-cohort labels). A standard easy/medium/hard menu doesn't produce this benefit because players don't self-sort cleanly into fixed tiers based on self-perception.

## Decision-Making Density

Decision-making density is the primary driver of player investment. Players become invested proportional to how many meaningful decisions they make, not proportional to production value or narrative quality. "I did that. Your solution was different."

When evaluating balance, ask: are players making interesting choices? If one path is obviously dominant, decision density drops to zero for that choice point -- it's not a real decision anymore. The goal of balance work is to restore decision density by ensuring multiple options have genuine contexts where they shine.

## Small Randomness in Simple AI

Adding slight randomness to simple AI behaviors creates perceived depth. Players read pattern variation as intelligence. A small random factor on top of simple rules achieves the same perceived complexity as over-engineered AI systems. Don't build elaborate behavior trees when a simple system with noise produces richer player interpretations.

This is relevant to balance because AI opponents that feel predictable get "solved" quickly, collapsing decision density. A small random element keeps the decision space alive without requiring complex balance tuning of AI behaviors.

## Simplification with Stopping Condition

When the design feels bloated with options, apply this process:

1. Remove options until something breaks (the game stops being interesting).
2. Add back the last thing you removed.
3. You are now at minimum viable complexity.

Checksum: if you didn't add back at least one option, you probably didn't remove enough. Most designers under-simplify. A bloated option set where half the options are never picked is worse than a tight set where every option sees play -- even if the tight set has fewer total choices.

## Beta/Test Branch as Risk Buffer

For live games: deploy balance changes to a test branch first. Let self-selecting engaged players try changes before the general population sees them. This catches the worst problems before they become community crises.

Maintain separate channels for test and stable populations to prevent spoiler effects and focus feedback. All changes must survive the test branch before hitting the main game. This lets you iterate at high speed without destabilizing the experience for most players.
