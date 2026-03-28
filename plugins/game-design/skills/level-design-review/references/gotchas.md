# Gotchas -- Common Mistakes When Evaluating Level Design

These are failure modes to watch for in your analysis. Avoid them.

## Intuitive navigation is not the same as fun navigation
Clarity (following visual cues to the goal) and depth (hidden paths, speedrun routes, secret areas) are separate layers. A level can be confusing to first-timers but deeply rewarding for explorers. Both layers serve different purposes and different players. Don't flatten navigation quality into a single "is this easy to follow?" question. The hidden layer is what makes a level worth returning to.

## Empowerment means delivering on the fantasy, not necessarily power fantasy
A meditative exploration game empowers emotionally. A horror game empowers through survival. A comedy game empowers through creative absurdity. "Empowerment" in level design means the level delivers on whatever the game's central promise is. Don't evaluate every game through the lens of making the player feel powerful.

## Constraint-driven design is legitimate and often better than planned design
Some of the most memorable level moments emerge from working around limitations rather than executing a plan. When a good design idea is blocked, the forced workaround may be more memorable than the original. Don't dismiss constraint-driven solutions as compromises -- they are a valid and often superior design method. Deliberately constraining yourself can force innovation.

## Grey-box before full art
Investing in art for an unvalidated level design is the most common waste. If the level doesn't play well in grey-box (minimal art, basic geometry), art won't fix it. Any risky or novel level idea must be grey-boxed and tested before committing to production art. A good idea that is never proved out in grey-box is a cut idea waiting to happen.

## Difficulty select screens are often a design failure
They ask players to evaluate difficulty before they've played -- an uninformed, irrevocable choice. Embedding difficulty through risk/reward pathways is richer because players discover their comfort level through play, making continuous contextualized decisions rather than one upfront abstraction. When reviewing a level, check whether difficulty is embedded in the environment or outsourced to a menu.

## Empty space is not breathing room -- it is dead time
Space between encounters should contain discovery, narrative, or environmental interest. "Rest" is not the absence of content; it is lower-intensity content. Every room, corridor, and transition needs a reason to exist. Emptiness can work as a pacing tool when the absence of enemies IS the tension, but emptiness without purpose is boredom. If a space has no gameplay, no narrative, and no emotional purpose, flag it.

## Linear levels pretending to be open feel worse than honestly linear levels
If there's only one path, don't dress it up with fake branching. Players feel manipulated when they discover the illusion. A level that looks open but funnels through a single path sets the expectation of choice and then betrays it. Check for genuine decision points: can the player approach objectives in different orders, use different routes, or choose different strategies? A single corridor with branching visuals is not open design.

## Non-linear content requires narrative integration
Optional side content that exists purely for completionism -- collectibles with no context, hidden items with no narrative stakes -- is padding. Players recognize mechanically inert content and resent it. The fix requires two things: clear reward signaling before the player commits to the detour, and narrative integration that ties the optional content into the world or story. Optional content that adds to the world is exploration; optional content that just adds time is busywork.

## Puzzle ordering is a distinct skill from puzzle creation
A well-designed puzzle in the wrong position teaches nothing. Sequence puzzles to build on previous knowledge: introduce a concept, test it, combine it with a prior concept, test the combination. Key operations: insert bridging puzzles where players struggle, optionalize hard gates instead of deleting them, provide multiple available puzzles at any given point so no single puzzle blocks all progress. If you evaluate individual puzzles without evaluating their sequence, you miss half the design.

## Frontloading tutorials with text instead of teaching through play
If a level needs a text box to explain what the player should do, the level has failed at its job. The best tutorials disguise themselves as gameplay: intensity without real danger, each section teaching a new mechanic through structure rather than prompts. Evaluate whether the level teaches through play or relies on explicit instructions.

## Rollercoaster pacing applied uniformly becomes predictable
The crescendo/trough model is so widely used it becomes its own meta-pattern. Players learn the rhythm and anticipate the beats, so no individual peak lands as hard as it should. The fix is not to abandon pacing but to periodically violate the pattern deliberately -- use absence, sudden reversal, or subverted expectation to reset the player's predictions.

## Backtracking is not the same as bi-directional design
Reusing level art by making the player retrace the exact same path is perceived as laziness. Bi-directional design reuses the same space but changes the gameplay logic -- different enemies, mechanics, objectives, or environmental state -- so the space feels different on the return. When reviewing a level that sends the player back through familiar territory, check whether the return trip offers meaningfully different gameplay.

## Making every space equally important
Not every room needs to be a setpiece. Levels need rhythm: high-intensity moments need low-intensity spaces around them to land. If every space is turned up to maximum, nothing stands out. Peak moments only work because of the quieter buildup before them.

## Ignoring the safe zone principle
Players need to enter an area, feel relatively safe, and read the environment before action begins. Consistent object vocabulary lets players assess threats honestly. If a level drops the player into chaos with no moment to orient, the design is fighting the player's ability to make meaningful decisions. Safe zones are not wasted space; they are where strategy happens.

## Testing execution instead of understanding in puzzles
The best puzzles test whether the player understands the system, not whether they can execute a precise sequence. If a puzzle is hard because the solution requires pixel-perfect timing or tedious repetition rather than an insight about how the system works, the difficulty is in the wrong place. Puzzle difficulty should come from the mental model, not from dexterity.

## Designer's curse -- knowing the level too well
When you've designed a level, you know where every encounter is, what every environmental cue signals, what every resource cache foreshadows. Players don't. The room that screams "arena encounter" to the designer reads as "interesting environment" to a fresh player. The fix is rigorous external playtesting and actively remembering that the player has no prior information.

## Stopping playtesting too early
Designers systematically overestimate when playtesting reaches diminishing returns. Late-stage playtests frequently reveal problems that would have shipped otherwise. Intuitions about when playtesting stops being useful are optimistic. Keep going longer than feels necessary.
