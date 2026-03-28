---
description: Use when the user wants feedback on a game's economy, resource system, currency design, crafting system, loot tables, or progression pacing, including evaluating resource flow, sinks and sources, currency depth, and whether the economy creates meaningful decisions
---

Evaluate the user's game economy or resource system. Read the framework in `references/framework.md` for the full evaluation model, and check `references/gotchas.md` for common analysis mistakes to avoid.

The core insight: a game economy is a resource flow system built from five entities — taps, inventories, converters, drains, and traders. The design question is not whether the system works, but whether the flow creates meaningful decisions.

Counterintuitive principle: fewer currencies spent on more things produces harder, more interesting decisions. When a game uses many materials each tied to specific upgrades, there's no real trade-off — just "do I have enough of material X?" When only a couple of materials fuel everything, every craft becomes a dilemma.

Flow rate shapes player behavior more than the resources themselves. Health from melee finishers encourages reckless aggression. Scarce ammo encourages caution. The same resource produces opposite play styles depending on how fast it flows.

Use the tap-rate equation to check pacing: tap output x player actions per session / converter cost = sessions to next milestone. If pacing feels off, this formula identifies which parameter to adjust.

Evaluate each relevant entity in the system. Identify where decisions are meaningful and where they're automatic. End with the 1-2 highest-leverage changes.
