# Gotchas — Common Mistakes When Evaluating Economy Design

These are failure modes to watch for in your analysis. Avoid them.

## Treating all grinding as bad
Grinding can be the fun if it's a puzzle. When the loop itself requires interesting decisions — automation, layout optimization, bottleneck management — it's not grinding, it's gameplay. Before flagging a grind loop as a problem, ask whether the loop requires meaningful choices.

## Adding currencies to add depth
More currencies does not mean harder decisions. Many materials each tied to specific upgrades produce no real trade-offs — just "do I have enough of X?" Fewer currencies with broader use creates dilemmas. When two materials serve everything, every craft locks out other options. Recommend consolidation, not expansion.

## "More currencies increases agency" is backwards
This is a counter-intuitive trap. Designers add currencies to create "more decisions" but each additional currency that maps to a single use makes individual transactions less meaningful. When material A only upgrades weapon type A and material B only upgrades weapon type B, there is no decision — players just upgrade whatever they're using. The system has the appearance of complexity with none of the substance. Converters only create decisions when the same input can go toward competing outputs.

## Ignoring flow rate as a behavior lever
The rate resources appear and disappear shapes play style more than the resources themselves. An action game and a survival horror game both use health and ammo — but a fast flow rate creates aggression while a slow one creates caution. When evaluating an economy, assess flow rates before assessing resource types.

## Missing drains
Economies without sinks inflate until choices become meaningless. If a player can accumulate resources indefinitely without losing them, every decision eventually becomes "yes" instead of "this or that." Look for drains. If there are none, that's usually the highest-leverage fix.

## Drains that feel arbitrary break player trust
Arbitrary resource destruction — random breakage, unexplained taxes, mystery decay — feels like the game cheating the player. Drains that match the world's logic — equipment wear from use, fuel consumption during travel, food spoilage over time — feel fair. The mechanical effect is identical; the framing is everything. When recommending drains, always consider whether the player can understand what caused the loss and how to manage it.

## Evaluating economy in isolation
Economy serves game feel — it's not a separate system. When health comes from melee finishers and ammo from a special weapon, the economy IS the combat design. Evaluate how the economy shapes moment-to-moment play, not just whether the numbers balance on a spreadsheet.

## Assuming players will play as intended
If players can break a tap, they will. When evaluating taps, ask: can this be looped? Can the player bypass the intended flow? Design for exploit vulnerability, not ideal behavior.

## Fixing one exploit without tracing the full graph
Exploit-chain analysis is essential: fixing one exploit can redirect players to a worse one. Economy systems are interconnected — patching one tap or converter can redirect the exploit to an adjacent part of the system. Before recommending a patch for any broken economic node, trace all connected systems to predict where player behavior will flow next. Fixes need to be designed with the full economic graph in mind, not just the broken node.

## Overlooking inventory limits as a design tool
Carry limits force spending decisions. Without them, players hoard resources and defer all choices until they've accumulated enough that nothing matters. Inventory limits are not a UX inconvenience — they're an economic pressure valve. If a design has no inventory constraints and players aren't spending, recommend adding limits before adding more content.

## Positive feedback loops without cognitive demand
A positive feedback loop where each cycle requires new problem-solving is engaging. A loop where each cycle is identical repetition is grinding. The distinction is cognitive load, not mechanical complexity. A complex-looking loop that plays the same way every time is still a grind. A simple-looking loop that requires different thinking each cycle is still engaging. When evaluating a feedback loop, ask what the player is thinking on cycle 10 versus cycle 1 — if the answer is "the same thing," it's a grind regardless of how many systems are involved.

## Static prices in trader systems
Trade-route arbitrage will be found and exploited if price differentials are static. Any fixed price gap between two merchants is a guaranteed profit loop — players will shuttle between them endlessly. Static prices in a trader system are functionally a broken tap. Prices must either be dynamic (supply/demand degradation on repeated transactions), temporal (time-limited windows, spoilage), or gated by risk (travel cost, enemy presence, limited access) to prevent exploitation.

## Treating economy as a late-stage concern
Resource flow shapes moment-to-moment feel from day one. A game with too-abundant health plays differently than one with scarce health — and that difference matters from the first encounter, not just at endgame. Evaluate economy decisions as core design, not balance tuning.
