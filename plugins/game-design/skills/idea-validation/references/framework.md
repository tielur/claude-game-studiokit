# Idea Validation Framework -- Reference

## The Core Premise: Idea Quality Dominates

Idea quality is the dominant variable in commercial success, more than execution quality, polish, or production value. Games with janky physics and placeholder art have sold millions on concept strength alone, while beautifully polished games with weak concepts regularly fail. This does not mean execution is irrelevant. It means the concept determines the ceiling and execution determines how close you get to it. When validating, weight the idea itself far more heavily than production concerns.

This reframes how much analytical attention to give the idea versus production quality. Developers systematically over-invest in execution and under-invest in validating the idea itself. Polish is fungible; a weak idea is not.

## The Workback Timeline -- When Validation Actually Matters

Evidence quality inversely correlates with decision utility across the development timeline:

- **Post-launch:** High certainty (sales data, player counts) but zero ability to change the core idea.
- **Late development (Steam Next Fest, announcement trailer):** Decent signal (wishlists, playtime, chart position) but sunk cost makes pivoting psychologically and financially painful. Feedback at this stage can tweak but not redirect.
- **Mid-development:** Moderate signal (viral trailer, devlog traction, community interest) but 6+ months of investment means negative data rarely changes trajectory in practice. Even a catastrophically bad signal at this stage will likely be rationalized away.
- **Early development:** Low-certainty evidence (pitch deck reactions, prototype feedback, itch.io metrics) but maximum ability to pivot, scrap, or redesign.

**Key rule:** Validate as early as possible. That is when validation can actually change the trajectory. Waiting for better data means waiting until the data no longer matters.

## The Idea Iceberg -- 5 Levels of Validation

Each level goes deeper. Skipping levels creates blind spots.

### Level 1: Experience & Context

The more games you have played and genres you understand, the better your instincts. Deep genre knowledge reveals gaps and opportunities. Being an avid gamer is a prerequisite, not an advantage.

A casual player with deep experience in free mobile games may not realize their demographic will not buy a paid puzzle game on Steam.

### Level 2: Skill

An idea is only good if the team can actually build it. A massive open-world extraction shooter is a great idea for a 350-person studio, not a solo beginner.

**Constraints-first design** turns this into a strength. Perform a skills audit: what can you build, what can you not, what is in the middle? Constraints eliminate 90% of ideas, leaving only ones you can execute. Some of the most commercially successful indie games exist because the developer could not animate walking characters, or could not create detailed art, so the constraints pushed the design toward something distinctive.

### Level 3: Market Research

The first step into objectivity. Key resources: Steam's yearly top-selling lists, SteamDB, genre earnings data from industry analysts.

**Genre ceiling is a hard constraint on market size.** Different genres have dramatically different revenue ceilings at every percentile. Across thousands of Steam titles, the top 1% of puzzle games earned roughly $1.1M while the top 1% of simulation games earned $4.6M. This is not a difference in execution quality -- it is a structural difference in demand. Choosing a genre is effectively choosing a maximum addressable market. This is not about chasing trends. It is about understanding the arena you are entering and what ceiling you are accepting.

**Concept ceiling framing.** $1M ceiling concepts are plentiful. $100M ceiling concepts are rare, maybe a handful per year. Good execution alone can get you to ~$100K, but the concept determines the ceiling.

**Genre-mixing requires separate appeal-coherence work.** Combining two popular genres does not automatically combine their audiences. The intersection may be tiny, and the appeal of each component may conflict with the other. A mixed-genre game built from market research must solve the appeal problem separately: who is this for, and does it deliver on a single clear fantasy? Each genre's appeal makes promises that the other genre's mechanics may break. Market research tells you where demand exists, not how to structure a coherent player promise.

Study games that are anomalies: small budgets and teams achieving outsized success. Look for concepts proven in other media (TV, film) but not yet done well as a standalone game. Translating successful media is a high-hit-rate strategy that is underused because the difficulty is execution, not concept.

### Level 4: External Validation (THE CRITICAL GAP)

Goal: answer "would people buy this game?" as early as possible. This is the hardest and most important level.

#### Behavioral Gap Detection

There is a critical difference between "oh yeah, this is cool" and "oh my God, I need to play this." What people say versus what they do are completely different data types, and only behavior predicts purchases.

**Must-have signals** (predict purchase behavior):
- Playtesters ask for new builds without being prompted
- Sessions run over without player awareness of time
- Playtesters recruit other players on their own
- Emotional investment in outcomes -- frustration at losing, excitement at winning, investment that implies the stakes feel real

**Just-cool signals** (do not predict purchase behavior):
- Playtesters complete builds but do not follow up
- Feedback is constructive but detached ("you could add X")
- Happy to stop when the session ends
- "That was neat" reactions without urgency or desire for more

If you are only seeing just-cool signals, the concept is not converting. This is the most reliable early indicator of commercial weakness.

**Calibration method:** Recall a game you bought day-one without hesitation. Observe your own behavior and emotions at the moment of that decision. That is the target response you are looking for in others.

#### Pitch Deck Validation

A pitch deck for a game that does not exist simulates the actual purchase funnel. The first step in buying a game is not playing it -- it is watching a trailer, seeing a GIF, reading a description. A pitch deck replicates exactly this experience without requiring a prototype. It tests whether the concept converts attention into interest, which is the same conversion a store page must perform.

Process:

1. Brainstorm ideas, vote on favorites
2. Filter through experience, feasibility, market research, appeal, and fantasy strength
3. Pick the top ideas and define the game loop (weak ideas fall apart here)
4. Create pitch decks and share with people (~1 hour of work per deck)
5. Ask people to rank or choose, not critique. Selection data is signal; improvement suggestions are noise.
6. Cut ideas with low selection rates before prototyping

Caveats: skip pitch decks for games where the mechanic is the idea (tactile, card-manipulation feel that cannot be conveyed without playing). For those, go straight to playable prototype. Also, pitch deck results are relative rankings among your idea pool, not absolute market signals. A pitch deck that wins internally may still be weak in absolute terms.

#### Free Demo on itch.io

Make a free demo and see if people will play it. If people will not play your game for free, they will not buy it.

**Benchmarks (itch.io views):**

- **< 5,000 views** -- unlikely to succeed commercially (still possible for hobbyist goals)
- **5,000-10,000 views** -- decent; expect ~1,000-10,000 Steam sales
- **10,000-50,000 views** -- magic zone; strong commercial potential
- **50,000+ views** -- probable hit

Post to itch.io (lowest friction for browser games), seed with 2-3 targeted Reddit posts, then let the itch.io algorithm push it organically. Read your data: low CTR means bad thumbnail/title; high views but low plays means your page does not look appealing; plays but low retention means broken game loop or onboarding.

**CTR on your demo thumbnail predicts Steam performance, not just itch performance.** Steam and itch.io both use thumbnail-driven discovery. A low CTR on itch is not an itch problem -- it is a signal that your capsule art and title will also underperform on Steam. Fix it before Steam launch.

#### The Validation Loop

1. Prototype and post a web build to itch.io
2. If it gets traction (~1,000+ plays), refine and post a polished version
3. If the refined version does even better, you have a winner
4. If either step fails, scrap or pivot before investing more time

### Level 5: Intuition

Intuition is a real and trainable faculty, not a mystical substitute for data. Each shipped game -- including commercial failures -- sharpens judgment about what will work. Early in a career, lean heavily on external validation because your intuition has not been calibrated yet. Later, intuition becomes a faster and surprisingly reliable signal that guides countless micro-decisions during development.

Intuition is valid but only after working through Levels 1-4. Skipping straight to "I just know this is good" without the preceding levels is the most common failure mode.

## Fantasy-First Approach

Players do not buy mechanics -- they buy experiences. The industry default of "it's X but Y" trains developers to treat mechanical novelty as the primary appeal driver. But players encountering a store page are not evaluating design elegance -- they are asking "do I want to be in that world?" A game about a mundane activity can outsell a mechanically innovative game if the context promises something emotionally resonant. The mechanic is downstream of the fantasy.

Start with what players want to do or be, not with a mechanic. "Cute bunny platformer" (mechanic-first) is generic. "Feel like the cutest bunny alive" (fantasy-first) opens up many possible game formats.

**Fantasy size = market size.**

- "Cheat at poker and win big" resonates with millions of people
- "End the world in gory ways" has a niche but real audience
- If the fantasy does not resonate with somebody, nobody will buy it

Think of fantasies as cravings players have when browsing for games. Mine your own cravings as a gamer.

**The hook vs fantasy distinction.** Hooks (mechanical novelty) can work and still be the wrong strategy to optimize for. The danger is that focusing on the hook causes developers to neglect the experience layer. The hook becomes a substitute for appeal rather than a complement to it. Test this with the removal test: if you removed the novel mechanic from the pitch entirely, would the game still be appealing? If yes, the hook is additive. If no, the hook is load-bearing and the game lacks native appeal -- a fragile position.

**Fantasy-to-design constraint pipeline.** When starting from a fantasy, commit to fully serving it. The fantasy creates constraints: add only elements that reinforce the fantasy, cut elements that split attention or dilute the feeling. Marketing becomes easier because the pitch is the fantasy itself.

## Single-Sentence Pitch Filter

Format: **Goal** the player pursues + **key actions** they take to achieve it.

If you cannot write this sentence, you have a setting or story idea, not a game idea. Use this to audit all ideas and separate wheat from chaff.

## Ideation Techniques (Brief Reference)

Use these when the user needs to generate or refine ideas before validating:

- **SCAMPER** -- Substitute, Combine, Adapt, Modify, Purpose, Eliminate, Rearrange. Apply to an existing game or idea to generate variations.
- **Constraints-first** -- Start from what you can build; constraints push toward unique concepts.
- **Fix a genre problem** -- Pick a genre you dislike and identify what would need to change. The problem defines your target market and marketing angle.
- **Design for memorable moments** -- Imagine players excitedly recounting their playthrough to friends, then design the game that creates those stories.
- **Draw from life** -- Mundane jobs and everyday experiences produce more original games than zombies and spaceships.
- **Look at non-games** -- Borrow interaction patterns from familiar non-game contexts (swipe interfaces, physical tools, everyday objects). Familiarity removes the learning curve.
- **Translate successful media** -- Concepts proven in other media (TV, film, books) are high-confidence starting points. The difficulty is execution, not concept. The market rewards well-executed adaptations of popular fantasies even when the inspiration is obvious.
