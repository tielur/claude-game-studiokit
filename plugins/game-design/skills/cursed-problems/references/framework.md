# Cursed Problems Framework -- Reference

This is the core framework for identifying and working around cursed problems in game design.

## The Core Insight

A game is a state machine with a golden path from start state through play space to objective. In a cursed game, that golden path passes through fire -- states where player promises break. The player follows the path anyway because the objective demands it. No amount of tuning fixes this because the conflict lives in the game's premise, not its parameters.

## Player Promises

Player promises are the essential experiences that bring a player to the game. They live in two places:

- **The designer's heart** -- what drives the game's creation
- **The player's heart** -- what players believe the game owes them

Players infer promises from mechanics and systems whether the designer intended them or not. A game with a scoring system promises that scores matter. A game with character customization promises that expression matters. These inferred promises are just as binding as intentional ones.

Promises also evolve over time. As the community develops meta-strategies and player skill levels rise, conflicts that didn't exist at launch can become cursed. What was a theoretical concern at release becomes a dominant pattern as optimal strategies are discovered. A promise conflict that only manifests at high-level play will eventually define the entire game as the player base matures. Revisit promise analysis periodically, not just at design time.

## Cursed vs. Hard

Not every difficult design problem is cursed. Hard problems can be solved with enough effort. A space exploration game that feels empty across millions of worlds has no fundamental contradiction, just insufficient execution. A degenerate fighting game character playing hyper-defensively can be tuned without changing the game's identity.

Cursed problems cannot be tuned away. The test: do the two promises fundamentally contradict each other such that fulfilling one inherently breaks the other? If yes, the problem is cursed.

Key signal: if every plausible fix to the conflict requires changing the game's identity, it's cursed.

## Eight Cursed Problem Archetypes

### 1. Free-For-All Politics

- **Promise 1:** Focus on combat mastery (experience)
- **Promise 2:** Play to win (objective)
- **Conflict:** Winning in a free-for-all requires political play (alliances, betrayal, targeting), which is incompatible with rewarding combat skill. The game-theoretically optimal strategy is social manipulation, not the advertised skill. The best player often loses -- by design, not by accident.

### 2. Quarterbacking

- **Promise 1:** Cooperative experience where each player contributes uniquely
- **Promise 2:** Play to win via optimal strategy
- **Conflict:** Optimal strategy is centralized decision-making, which destroys interdependence. One experienced player can take over all decisions because the game state is fully visible.

### 3. Skill Inflation

- **Promise 1:** Long journey of mastery (years of improvement)
- **Promise 2:** Stable, vibrant community with broad skill levels
- **Conflict:** Mastery naturally raises the skill floor, making entry hostile for newcomers as weaker players leave. Long-lived PvP games where the remaining player base is so skilled that new players bounce off immediately.

### 4. Co-op Abuse

- **Promise 1:** Play to win in high-stakes competitive/cooperative play
- **Promise 2:** Social belonging and psychological safety
- **Conflict:** Frustrated competitive players lash out at teammates, destroying the safe social environment.

### 5. Quantified Creativity

- **Promise 1:** Express yourself through intrinsic creative goals
- **Promise 2:** Progress your character through extrinsic goals
- **Conflict:** Extrinsic goals don't just compete with intrinsic creative goals -- they consume them. This is a documented psychological pattern. In games that combine creative expression with progression rewards, the progression system will eventually dominate player behavior entirely. Creative play doesn't diminish gradually; it disappears. Players who intended to express themselves creatively get pulled into leveling or optimization loops instead. Any progression system, career track, or achievement layer added to a creative game will tend to subsume the creative experience.

### 6. Commodified Reward

- **Promise 1:** Rich, varied loot drop experiences
- **Promise 2:** Ubiquitous marketplace fantasy with efficient trading
- **Conflict:** When items are fungible via trading, every monster just drops currency. The item's intrinsic value (the surprise of finding the exact drop you wanted) is replaced by its exchange value. The loot surprise dies regardless of market tuning -- this is a structural property of efficient markets, not a tuning knob. Adding trade fees, limiting transaction volume, or adjusting drop rates are all attempts to add friction that fights the market promise itself.

### 7. Life Disruption

- **Promise 1:** Magical overlay on real life, playable anywhere and anytime
- **Promise 2:** Personal safety, convenience, and mindfulness
- **Conflict:** Any restriction on when or where you play weakens the core promise of ubiquitous play. The always-on location-based design inherently conflicts with player safety.

### 8. Kingmaking

- **Promise 1:** Player agency -- every player can affect the outcome
- **Promise 2:** Fair competition determined by skill
- **Conflict:** When a losing player can decide the winner, both promises are violated simultaneously. The losing player's agency becomes destructive rather than meaningful, and the winning player's skill becomes irrelevant in the final outcome. This is a cross-player cursed problem -- harder than intra-game ones because the designer cannot satisfy both players' promises simultaneously even in principle. Standard cursed problems conflict one player's promises with themselves; kingmaking conflicts one player's promises with another's.

## Four Workaround Strategies

These don't solve the problem. They require sacrifice. Name the sacrifice explicitly when recommending one.

### 1. Barriers -- Remove the Ability Entirely

Cut affordances that enable the problematic behavior. The promise-breaking action becomes impossible.

- **Free-for-all politics:** Battle royale format spreads players apart with high lethality and hidden information, making political play unviable
- **Co-op abuse:** Limiting communication to movement and contextual pings makes it impossible for players to mistreat each other
- **Cost:** Removes a potentially fun dynamic. The battle royale format sacrifices the PvP control fantasy. Minimal communication sacrifices rich social channels.

### 2. Gates -- Make Promise-Breaking Difficult

Softer than barriers. Don't eliminate the behavior, but raise the difficulty so most players don't bother.

- **Free-for-all politics:** Hiding scores and using complex scoring formulas gives players plausible deniability to just play hard instead of playing politics
- **Co-op abuse:** Sharing team resources (shared XP, shared economy) makes it hard to identify who's underperforming and therefore who to blame
- **Cost:** Reduces individual expression and legibility. Hidden scores sacrifice buzzer-beater tension. Shared resources sacrifice the sense of individual contribution. Hiding information is a design tool for suppressing emergent social dynamics -- when players can't easily identify who's winning, they default to playing the actual game instead of targeting each other.

### 3. Carrots -- Redirect the Objective

Change or add goals that keep players on the desired path without encountering the fire.

- **Free-for-all politics:** Tournament scoring that awards points for placement (not just wins) reduces incentive for political play since personal performance matters more
- **Quantified creativity:** Rewarding creative solutions mechanically (off-meta designs that counter standard attacks) or adding social metagames that incentivize creative expression alongside the core game
- **Cost:** Adds an external motivation layer that can diminish the magic circle. Tournament-level scoring changes the feel of individual games. Mechanical creativity rewards still constrain expression since you're optimizing.

### 4. S'mores -- Make the Fire Fun

Lean into the broken promise so hard it becomes the game's identity. Give players marshmallows to roast in the fire.

- **Free-for-all politics:** Embracing political play as the core mechanic, with secrecy, alliances, and betrayal becoming the entire point
- **Quantified creativity:** Leaning fully into strategic depth, effectively removing the creative expression goal to make a different but excellent strategy game
- **Party brawler:** Weakening both combat mastery and winning promises by embracing chaos with random items, stage hazards, and party-game energy. A different game than the original dream, but a great one.
- **Cost:** Changes the game's identity. The resulting game may be excellent but it's not the game you set out to make. The most celebrated solutions to cursed problems involved letting go of the original vision and embracing a different one that the constraints naturally supported. Reframe the workaround as a creative pivot, not a compromise. The sacrifice is not "the game you couldn't make" but "the constraint that produced the game you did make."
