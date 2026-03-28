# Randomness Framework -- Reference

This is the core framework for evaluating randomness in game design.

## The Core Insight

Randomness in games serves four purposes: **variety**, **balance**, **exciting rewards**, and **limiting the information horizon**. The critical design question is not whether to use randomness, but *when* in the decision loop it fires -- before or after the player commits to a choice.

## Two Types of Randomness

### Input Randomness (Pre-Luck)

Random events that happen *before* the player decides. The player sees the situation, then plans around it.

**Examples**: drawing cards before choosing which to play, procedural level generation, rolling dice before placement, random starting conditions.

**Design effect**: Supports strategic play. The player can read the board and make informed choices. Frustration is lower because failure feels like a planning mistake, not bad luck.

### Output Randomness (Post-Luck)

Random events that happen *after* the player decides. The player commits to a plan, then luck determines the outcome.

**Examples**: hit chances that can miss, loot drops with random contents, random enemy encounters.

**Design effect**: Can feel unfair -- your plan fails due to luck, not bad strategy. But it has valid uses: simulating imprecision in abstract combat, forcing risk management and contingency planning, and creating exciting moments of tension.

### Output Randomness Justification Checklist

Only use output randomness when at least one of these conditions holds:

1. **It only benefits the player.** The random outcome is exclusively positive (surprise critical hits, bonus drops, lucky saves). There is no downside surprise. Players never complain about output randomness that can only help them.
2. **Players can mitigate the worst outcomes.** The design gives players tools to reduce or recover from bad luck -- positioning, preparation, backup plans, rerolls. The randomness tests contingency planning, not just fortune.
3. **The random event is infrequent enough to feel like an event rather than noise.** A single dramatic dice roll per encounter creates tension. A random check on every action creates frustration. Frequency determines whether output randomness reads as meaningful or arbitrary.
4. **The game explicitly frames itself as a gambling or risk game.** When the entire premise is risk-taking (poker, press-your-luck games, betting mechanics), players opt in to output randomness as the core experience. The contract is clear.

## Five Evaluation Dimensions

### 1. Timing in the Decision Loop

Where does the randomness fire relative to the player's choice? Input randomness creates puzzles to solve; output randomness creates gambles to take. Neither is inherently better, but the designer should be deliberate about which experience they're creating.

**Key question**: Does the player see the random state before or after they commit to a decision?

### 2. Controlled Variance

Well-designed randomness isn't purely random -- it's shaped to prevent extreme outcomes. Specific techniques for controlling variance:

- **Bag randomness (draw without replacement)**: Shuffle all possible outcomes into a sequence, deliver in order. Guarantees even distribution over time -- every outcome appears before any repeats. Well suited for repeated small events like piece selection or enemy spawns.
- **Distributed shuffling**: Divide the deck or event pool into difficulty tiers or time segments, then shuffle within each tier. This guarantees pacing -- high-impact events are spread across the experience rather than clustering randomly.
- **Weighted loot**: Adjust drop rates based on player state, class, or progression. Biases results toward relevance for the current player rather than drawing uniformly from the entire loot table.
- **Mercy rules**: Guarantee success or a favorable outcome after N consecutive failures. Caps the worst-case streak length. Effective for rare high-value events where a long drought feels broken.

**Key question**: Are there guardrails preventing frustrating streaks or degenerate outcomes?

### 3. Information Flow

The ideal rhythm follows a **spiky information flow pattern**:

1. **Steady-state**: Known conditions, current plans remain viable, player is executing strategy
2. **Spike**: New random information arrives (enemy reveal, unexpected event, draw) that disrupts the current plan
3. **Regroup**: Player adapts strategy, makes new decisions based on the disruption
4. **Return to steady-state**: New plan stabilizes, player executes until the next spike

This rhythm gives players time to process and plan between random events. Two failure cases to watch for:

- **Constant spikes**: New random conditions every turn collapse the planning horizon to the immediate present. The system feels chaotic and unrewarding to engage with strategically, even though all randomness may technically be "input."
- **No spikes**: Flat information delivery makes plans too reliable. Gameplay becomes predictable and the randomness serves no purpose.

**Key question**: Does randomness create a healthy rhythm of planning and adaptation, or is it constant noise?

### 4. Transparency and Legibility

Players make better decisions and feel less cheated when they understand the odds. Showing hit percentages, using familiar mechanisms, and making probability intuitive all help.

**Physical randomness mechanisms** (dice, cards, spinners) are cognitively easier to trust than abstract percentages because the randomness is visible and tangible. Players have intuitive mental models of physical objects -- they can see the die has six faces, they can count the cards remaining in a deck. The same variance from an invisible algorithm feels arbitrary and suspect. Consider using physical metaphors even in digital games.

**Cards vs. dice -- a foundational distinction**: Cards enable dependent probability and synergy. Drawing from a finite deck means the composition is knowable and buildable -- each draw changes the odds of future draws, and players can construct combinations. Dice enable only independent probability -- each roll is identical regardless of prior rolls. This is the key distinction for choosing between card-like and dice-like systems. Use card-like systems when you want players to build toward synergies over time. Use dice-like systems when each event should be self-contained.

**Key question**: Can the player understand the probability space well enough to make meaningful risk decisions?

### 5. Directional Fairness

Randomness that only favors the player feels generous rather than unfair. When buildings have a small random chance to block incoming damage but never a chance to take extra damage, the output randomness is purely positive. When output randomness exists, biasing it toward the player preserves agency while adding positive surprise.

**Key question**: When randomness swings, does it swing toward the player or against them?

## Techniques for Better Randomness

- **Fudge the numbers** -- Some games display one hit chance but compute a different, more generous number behind the scenes. Others guarantee success after consecutive failures at low probability. The player doesn't need to know the true odds if the felt experience is fair. Design around how players actually perceive probability, not how probability actually works.
- **Discourage degenerate play** -- Gate starting bonuses behind having attempted a previous run to discourage restart-scumming for favorable RNG.
- **Shift output to input** -- Convert "will my attack hit?" (output) into "enemies telegraph attacks, you plan around them" (input). This preserves the strategic value of uncertainty while removing the feeling of wasted agency.
- **Use dependent probability** -- Cards drawn from a deck create dependent probability (drawing one card changes the odds of drawing others), enabling synergies and deck-building strategies. Dice are independent -- each roll is isolated. Choose the mechanism that fits your design goals.
