# Feedback Loop Framework -- Reference

## The Core Insight

Every persistent game mechanic creates a feedback loop: action produces an outcome, the outcome changes the game state, the changed state influences the next action. The critical design question is whether each loop amplifies (positive) or dampens (negative), and whether the combination of all active loops produces the pacing, tension, and decision-making the designer intends.

## Feedback Loop Diagnostic

For each system in the design, trace the loop:

1. **Identify the cycle**: action -> outcome -> changed state -> next action
2. **Classify**: Does success make future success more likely (positive) or less likely (negative)?
3. **Check the downward spiral**: Does failure make future failure more likely? If yes, is failure reversible (retry/reload) or persistent (carry-over)?
4. **Trace recovery paths**: If failure persists, does the player have any way to reverse the spiral, or is it inescapable?
5. **Check for counterbalance**: Is there an opposing loop? If not, does the design need one?
6. **Assess visibility**: Can the player see the loop operating, feel it without seeing it, or is it hidden entirely?

## Mixed Signals Test

Before finalizing a negative feedback loop, ask: "If I explained exactly how this system works to the player, would it change their behavior in a way I don't want?"

This is the hardest failure to diagnose because it looks like player confusion, not design confusion. One loop rewards aggression, another rewards caution. Each makes sense in isolation. Together they produce players who can't figure out what the game wants them to do.

The fix is either:
- **Hide the loop** so the player can't game it (works for dynamic difficulty)
- **Redesign so the signal aligns with desired behavior** -- make the negative loop something the player actively wants to trigger, not something imposed on them

## Dampening Toolkit (5 Levels)

From lightest touch to most drastic intervention:

1. **Soft cap**: Diminishing returns on the leading resource or advantage. The loop still runs, but each cycle yields less. Preserves the feeling of progress while limiting runaway.
2. **Diminishing returns**: Each successive gain in the same direction is worth less than the previous one. Similar to soft cap but applied to individual gains rather than cumulative totals.
3. **Catch-up mechanic**: Trailing players receive bonuses proportional to their deficit. The further behind, the stronger the boost. Works well in racing and party contexts; can feel patronizing in competitive ones.
4. **Hard cap**: Absolute ceiling on advantage accumulation. Once you hit the cap, the loop stops. Clean and legible, but can feel arbitrary.
5. **Reset**: Periodic wipe of accumulated advantage -- round-based, seasonal, or event-triggered. The most drastic option. Works when the reset is framed as a natural part of the game's rhythm rather than a punishment.

## Loop Pairing Pattern

Pair a positive competitive loop with a negative cooperative loop (or vice versa). The tension between them creates interesting decisions.

The model: keep the positive loop (winning makes you stronger), but add a forced ceiling that periodically removes accumulated advantage. The key is making the ceiling feel desirable or narratively meaningful, not punitive.

This works because the positive loop provides motivation (players want to get stronger) while the negative loop prevents runaway (the reset keeps the field competitive). Neither loop alone is sufficient -- the pairing creates the design.

## Early-Game Sensitivity Rule

Small advantages amplify most in early game when the base values are smallest. A +1 bonus matters more when the baseline is 3 than when it's 30.

Practical implication: if your game has a positive loop, the first few turns, minutes, or rounds matter far more than later ones. A snowball that forms early will be much larger by midgame than one that forms later.

Playtest feedback loops specifically during the opening phase. A loop that feels balanced at the midpoint may have already become unrecoverable by then. Early-game negative loops (upkeep costs, empire penalties, scaling difficulty) exist specifically to address this window.

## Positive Loops in Single-Player with Permadeath

Positive loops are acceptable and even desirable in single-player games with permadeath or meaningful failure states because they serve tension. The snowball creates stakes -- you're getting stronger, but losing everything is a real threat.

Without permadeath or meaningful failure, positive loops become grinding. The loop still amplifies, but there's no tension because the player can't lose their progress. The amplification needs to be paired with risk to feel engaging rather than repetitive.

The danger case: positive loops in games where failure is persistent but not terminal. If dying means losing your best resources and the game continues, the positive loop runs in reverse -- each failure compounds into the next, creating an inescapable death spiral. The failure isn't "positive loop exists" -- it's the combination of positive loop, persistent failure, and no recovery path.

## Narrative Framing of Mechanical Loops

The same mechanical effect can feel completely different depending on how it's framed.

A catch-up mechanic framed as "desperate heroics" feels different from one framed as "pity bonus." A ceiling that removes your strongest asset framed as "liberation" or "graduation" feels different from one framed as "forced retirement." The mechanical effect is identical; the emotional experience is not.

Design principle: make loops feel intentional thematically. If the loop works mechanically but feels arbitrary or punitive, the fix might be narrative, not mechanical.

## Loop Visibility Spectrum

Loops exist on a visibility spectrum:

- **Fully visible**: The player sees the math. "You gain +2 attack for each enemy defeated this turn." Clear, legible, plannable.
- **Partially visible**: The player feels the effect but doesn't see exact numbers. "Enemies seem to get tougher as I level up." Intuitive but not precisely trackable.
- **Hidden**: The player doesn't know the loop exists. Dynamic difficulty adjustments, hidden catch-up bonuses, invisible scaling.

Each position has tradeoffs:
- Hidden negative loops feel unfair when discovered -- players feel deceived about the rules they were playing by.
- Hidden positive loops feel like skill when they're actually assistance -- this can be desirable (the player feels competent) or problematic (the player overestimates their ability and hits a wall when the assistance stops).
- Fully visible loops can be gamed -- if players know exactly how the catch-up mechanic works, they may sandbag intentionally.

The choice of visibility should be deliberate, not accidental. Ask: "What happens when players figure this out?" because eventually they will.
