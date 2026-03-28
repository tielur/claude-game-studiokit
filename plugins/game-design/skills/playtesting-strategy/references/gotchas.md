# Gotchas -- Common Mistakes in Playtesting

These are failure modes to watch for when planning, running, or analyzing playtests.

## Memory failure

Players forget friction once overcome. A player who struggled at minute 5 and figured it out by minute 15 will not report the struggle in a post-session questionnaire. They've resolved the frustration internally and it vanishes from their recall. Only live observation captures mid-session stumbling blocks. This is why watched playtests are irreplaceable, not just "nice to have."

## Genre-expert bias

Experienced players in your genre may be frustrated specifically because your game deviates from their mental model of how that genre works, not because of fundamental UX issues. Their frustration may not represent your actual target audience at all. Always ask about their genre experience before the session, and when reviewing their feedback, distinguish between "this doesn't match my expectations from other games" and "this is genuinely confusing."

## Survivorship bias in metrics

Late-game data overweights survivors. A card, item, or strategy that appears powerful in aggregate data may look that way because only skilled players reached the point where they could acquire it. Players who survived to late stages were already likely to win regardless of what they picked up. Segment data by player progression and skill before drawing balance conclusions. Metrics show correlations; causation requires human interpretation.

## Sampling bias from super-playtesters

Two highly active testers generating most of the data can drown out everyone else. If your aggregate averages are essentially just two heavy users' experience, those averages are not representative. Run this check: if removing the top 5% of contributors by volume changes the conclusion, the conclusion was based on outliers, not signal. Either weight data by player or segment analysis by experience level before drawing conclusions.

## Designer playtesters

Some testers treat playtesting as an opportunity to pitch their version of the game. They suggest sweeping redesigns, new features, and alternative mechanics rather than reporting their actual experience. Their observations about what happened are useful; their design prescriptions are not. Don't dismiss everything because of the delivery, but don't be captured by their extended opinions either. Filter for observations vs. prescriptions.

## Structured questions outperform open feedback

Even thoughtful testers give vague answers to open questions. "What did you think?" produces "yeah it was good" or an inarticulate shrug. Structured questions constrain answers into actionable data. This is why the Fast Forward Method (see framework) works better than unstructured conversation. Open-ended questions without scaffolding produce noise, not signal, regardless of the tester's articulateness.

## Reusing Kleenex testers destroys their value

A tester who has played before can never give you first-impression data again. Once they've overcome the learning curve, usability friction becomes invisible to them. They navigate your tutorial differently the second time, not because the design improved, but because they already know it. Reusing them gives you false positive data on whether onboarding works for new players. Fresh testers are a non-renewable resource. Pace your Kleenex tests against your confidence that each iteration is worth burning a tester.

## Recording solutions instead of problems

"Add a minimap" is a solution. "I got lost in level 3" is a problem. Record problems. There may be ten solutions to each problem, and the tester's solution is rarely the best one. If your notes contain design prescriptions instead of raw observations, you lose the ability to diagnose root causes later. The fix you intuit on the fly may address a symptom, not the cause. Always capture the observable symptom first; decide on fixes later with all data in hand.

## Positive feedback doesn't mean the design works

Players are polite. "It was fun!" doesn't mean there aren't serious problems. In-person subjects especially hold back criticism when the developer is present. Look for behavioral signals instead: did they ask to play again? Did sessions run long without prompting? Did they recruit other players? Did they lean forward or disengage? Verbal praise is the weakest signal. Unprompted return behavior is the strongest.

## Devlog and community feedback is not playtesting

Positive reactions to development updates don't predict whether the game is fun to play. Community engagement measures interest, not quality. A thousand wishlist additions say nothing about whether the core loop works. These are marketing signals, not design signals. Running a playtest that validates the feel of the game in someone's hands is categorically different from a community responding enthusiastically to a trailer or devlog post.

## Testing too late in development

If the first playtest happens at beta, you've missed the window to cheaply fix fundamental interaction problems. Test the core mechanic at the prototype stage, even on paper. Early testing is cheap; late redesigns are expensive.

## Playtesting to get validation instead of finding problems

A playtest is an instrument for finding problems. If you're there hoping for praise, you'll unconsciously steer observations away from friction points, dismiss negative data, and walk away with a false picture of the game's state. The test is not for you -- it's for the game.

## Intervening during observation

If you jump in to explain something mid-session, you've contaminated the test. The confusion you interrupted was data. The moment you "help," you lose the information about where the design failed to communicate. Agree on intervention rules before the session starts and stick to them.

## Analyzing data during sessions instead of after

Snap judgments during observation lead to premature fixes. A problem that looks obvious in the moment may resolve itself when you see the full pattern across multiple testers. Watch the full session. Collect all data. Analyze afterward with the complete picture.
