# Economy Design Framework — Reference

This is the core framework for evaluating game economies. These ideas draw from established game design analysis of resource flow systems.

## The Core Model

A game economy is the flow of resources around a system — coins, crafting materials, XP, ammo, health, anything the player earns, spends, or loses. Every game economy is built from five basic entities.

## Five Core Entities

### 1. Taps (Resource Generation)

Taps generate new resources: enemy loot drops, sawmills, regenerating health, ore nodes. They can be automatic (timers) or manual (player-mined).

Taps shape player behavior through what they reward. Loot on enemies encourages combat. Crafting materials scattered across biomes encourage exploration. Health drops from melee finishers encourage aggression — the economy IS the combat design.

**Flow rate is the behavior lever.** Rare ammo in survival horror creates caution and dread. Abundant munitions in an action shooter create power fantasy. The same resource produces opposite play styles depending on how fast the tap flows.

A broken tap can destroy the economy. If players discover they can loop a resource source — kill respawning creatures, sell the loot, rest to respawn, repeat — the economy collapses into an infinite money loop. Patching one broken tap without auditing adjacent systems can redirect player behavior to an even more profitable exploit elsewhere.

**Tap-rate equation for pacing.** Tap output x player actions per session / converter cost = sessions to next milestone. This is a concrete, tunable number — not a vibe. If pacing feels off, audit this formula to identify which parameter to adjust.

### 2. Inventories (Resource Storage)

Inventories hold resources, optionally with upper limits (carry weight, attache case slots). Limits create decisions about what to keep and force players to actually spend resources rather than hoarding thousands of potions "just in case."

Inventory limits are a design tool, not a restriction. They force spending decisions and prevent the economy from stalling when players stockpile instead of engage.

**Inventory caps as forced-action timers.** A capped inventory is a timer in disguise. When a player's inventory is full, they must act — use, sell, or discard — before acquiring more. This forces engagement with converters that players would otherwise defer, prevents late-game safety hoarding that removes tension, and creates decisions about opportunity cost (what do I drop to pick this up?). This is a behavioral design tool, not just hoarding prevention.

### 3. Converters (Resource Exchange)

Converters exchange one resource for another: shops, crafting stations, leveling up. They control pace — XP-per-kill and XP-to-level-up together determine how many enemies must be killed before gaining power.

**Currency design is where decisions live or die.** When a game uses many materials each tied to specific upgrades, there's no real trade-off — just "do I have enough of material X?" When only a couple of materials fuel everything, every craft locks out other options, forcing intentional choices.

The principle: **fewer currencies spent on more things = harder, more interesting decisions.** More currencies feels like it should add depth, but it actually removes trade-offs by siloing choices.

**Currency count is a deliberate design dial, not a binary.** Fewer shared currencies produce harder individual decisions with more weight — players must trade off competing needs. More distinct currencies produce more granular designer control but reduce agency per decision. This is a spectrum: if you want a system that produces tension, minimize currencies; if you want exploration rewards, multiply currencies tied to locations. The choice should be intentional.

### 4. Drains (Resource Removal)

Drains are the opposite of taps: breakable weapons, health loss, ammo consumption, taxes. They permanently remove resources from the system.

Drains serve multiple design functions:

- **Slow power growth** by forcing players to replace lost resources before progressing
- **Force action** — hunger meters demand food-seeking, spoiling crops require schedule planning
- **Encourage variety** — breakable weapons make players try new gear instead of optimizing one loadout
- **Add escalating risk** — runes or currency lost on death create tension that builds with each encounter; carrying more fragile cargo can be a risk/reward calculation
- **Create risk asymmetry** — drains convert a safe activity into a gamble. The same resource at different stack sizes carries different strategic weight. Drains are a lever for manufacturing tension without changing enemy stats or combat difficulty.

Drains also create **negative feedback loops**. Exponentially increasing level-up costs make farming weak enemies ineffective, pushing players to explore and fight tougher foes. This is one of three ways to mitigate grinding (see below).

**Reframing negative feedback loops.** Negative feedback loops are dual-purpose: they slow the leader AND incentivize exploration of unexplored content. Exponential cost curves experienced as "progression slowing" actually function as push mechanics toward new areas. The disincentive on the current strategy is simultaneously a positive signal toward a different strategy.

**Drains need legibility and in-world logic.** Equipment wear from use, fuel consumption during travel, food spoilage over time — these feel fair because they match the world's logic. Random breakage, unexplained taxes, or arbitrary resource destruction feel like the game cheating the player. The mechanical effect is identical; the framing is everything.

**Cautionary pattern: cascading loss spirals.** Once a player starts losing properties or units, they lose income, which means they can't recover, which means they lose more — a cascading negative feedback spiral with no escape. Drains without a recovery path create misery, not tension.

### 5. Traders (Economic Agents)

Traders are NPCs with their own inventories, wallets, and pricing rules. They are structurally distinct from vending machines. A static price list is just a converter with extra UI. True traders — those who own inventory, have location-based pricing, or have limited stock — create trade-route puzzles and emergent player strategies.

**What makes a trader a trader:** the merchant must have some combination of owned inventory that depletes, prices that vary by location or supply, or limited stock that refreshes on a schedule. Without at least one of these properties, the "trader" is functionally just a converter and should be evaluated as one.

Traders risk creating positive feedback loops — getting richer per transaction. Two mitigations:

- **Supply and demand** — letting players flood the market and crash prices punishes greed and creates a self-balancing system
- **Risk/reward mechanics** — fluctuating prices with a spoilage or expiration deadline create a window of opportunity that prevents riskless speculation

## Feedback Loops in Economies

**Positive feedback loops** (rich get richer) — output feeds back into input, reinforcing growth. Compelling but can lead to grinding. Idle games and roguelikes with permanent progression embrace this deliberately.

**Negative feedback loops** (catch-up mechanics) — growth becomes progressively harder, pushing players toward new content instead of repetition.

## Three Ways to Mitigate Grinding

1. **Turn it into a puzzle** — make optimization the challenge. The loop exists, but requires complex problem-solving: automation, layout planning, bottleneck management. The grind IS the game.
2. **Negative feedback loops** — exponentially increasing costs make farming weak sources ineffective, pushing players to explore and fight tougher foes.
3. **Add drains** — constant resource sinks slow accumulation and force ongoing engagement with the economy rather than letting players outgrow it.

## The Complete Flow

Resources flow: **Taps -> Inventories -> Converters**, with losses to **Drains** and exchanges with **Traders**. How these entities are designed and balanced shapes the pace, challenge, and feel of the game. Simpler games may omit entities; MMOs and real-money economies add further complexity beyond this framework.
