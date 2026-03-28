# Playtesting Framework -- Reference

## Two Types of Playtesting

### Kleenex Testing (Fresh Testers)

Each tester is used once. After they've seen your game, they are permanently burned for that content and can never give first-impression feedback again. This is a hard expiration, not a soft one.

**Purpose**: Usability issues, tutorials, onboarding, first impressions, learning curve, stumbling blocks in player understanding.

**Method**: Observe over the shoulder, take real-time notes, record the session. Do not help unless the player is completely stuck. Watch what they do, not what they say.

### Deep Testing (Repeat Testers)

The same testers play repeatedly over time, developing strategies and exploring depth.

**Purpose**: Balance, strategic depth, emergent gameplay, competitive fairness, evolving meta.

**Method**: Regular builds with changelogs, structured feedback channels, long-term relationships with testers. A dedicated chat channel with a low-friction feedback bot produces more and better data than periodic surveys. Push frequent builds to keep testers engaged and returning.

## Playtester Segmentation

For each tester, collect their genre experience and general gaming frequency. Then weight observations against their profile:

- **Fresh testers (Kleenex)**: One-time use. Test usability and first impressions. Never reuse for the same content.
- **Repeat testers (Deep)**: Build familiarity over time. Test balance, depth, and long-term engagement.
- **Genre-expert testers**: High game literacy but bring strong expectations from competitors. Their frustration may be deviation from mental models, not actual UX problems. Always ask about their genre experience and interpret with care.
- **Non-gamer testers**: Valuable for accessibility and onboarding validation, but not for balance or depth testing.

## Layered Feedback Architecture

Balance data collection across multiple layers, from most passive to most active. Never rely on one layer alone. Passive metrics catch problems vocal feedback misses, and vice versa.

1. **Anonymous aggregate metrics** (run data, win rates, completion rates, session length). Highest volume, lowest bias. Silent players who never write a word still generate this data. If you only optimize for vocal feedback, you systematically underweight the majority of your players.
2. **Automated feedback tools** (in-game surveys, rating prompts, feedback bots in chat channels). Medium volume, some self-selection bias. Lower the barrier to contributing: no forms, no surveys, just a bot that accepts freeform messages at any time.
3. **Community channels and streamers**. Streamers are especially valuable because they narrate their full internal monologue for an audience, making them more candid than in-person subjects. In-person subjects hold back criticism when the developer is present. Treat streamer footage as high-quality qualitative data. Community channels provide real observations that are often surprising, but audiences cannot report on game feel, input precision, or tactile elements.
4. **Watched playtests** (observation + think-aloud). Lowest volume but highest insight per session. This is irreplaceable for usability issues. Narrated video playtesting is the highest-signal method for understanding exactly where players stumble.

## Observation Methodology

### Positioning and Recording

- Position yourself 45 degrees behind the player -- visible enough that they know you're there, removed enough not to influence their behavior.
- Record the session (video + audio). Human memory is unreliable even during observation. Recordings are rewatchable months later with fresh analytical perspective. A five-minute observation without recording produces worse data than a recorded session watched twice.
- Do not intervene during the session. If you jump in to explain something, you've contaminated the test. The confusion you interrupted was data. Agree on intervention rules before the session starts and stick to them.

### Record Problems, Not Solutions

Write down what went wrong, not what you think should change.

- Write: what the player did, where they were, what they seemed to expect.
- Do not write: what you think should be changed.
- "Add a minimap" is a solution. "I got lost in level 3" is a problem. There may be ten solutions to each problem, and the tester's solution is rarely the best one.
- Solutions should come from analysis of all data after the session, not snap judgments during it.

### "Things-Almost-Happen" Moments

Watch for moments where testers try approaches that don't work in the current design. If multiple players attempt a strategy that fails, consider designing content where that approach is the solution. This crowdsources design ideas from player intuition.

## The Fast Forward Method -- Post-Session Questionnaire

A structured post-play questionnaire that avoids open-ended rambling. Use as a form or single-page handout. Ask these six questions:

1. What were you trying to do?
2. What did you expect to happen?
3. What actually happened?
4. Was anything confusing?
5. Was anything frustrating?
6. What was the most fun moment?

Structured questions constrain answers into actionable data. Even thoughtful testers give vague answers to open questions like "what did you think?" This method works far better than unstructured conversation because most players cannot articulate gameplay experiences without scaffolding.

### Interpreting Misaligned Player Perception

When playtesters identify an unintended element as the core of your game:
- Option A: Shrink that element (restore your intended design).
- Option B: Lean into it (follow the fun, let the game become what players are enjoying).
Neither is automatically correct -- the framework forces you to make a conscious choice rather than ignore the signal.

## When to Test at Each Stage

### Prototype
Focus on Kleenex testing the core mechanic. Does the fundamental interaction make sense? Is it satisfying? Test on paper or with minimal builds. Testers don't need polish; they need a clear interaction to react to.

### Alpha
Expand Kleenex testing to onboarding and learning curve. Begin Deep testing with a small, committed group for balance and systems. Establish a feedback channel and push regular builds with changelogs.

### Beta
Heavy Kleenex testing with wider demographics. Deepen the Deep testing group and start collecting metrics. Narrated video playtests are especially valuable here for sequencing and difficulty curve issues.

### Pre-Launch
Final Kleenex passes for the complete experience. Use metrics to validate balance decisions (but interpret carefully -- see gotchas). Test the full player journey from start to credits.

## Give-First Recruitment Framework

Before asking for playtesting, contribute value to the community you're recruiting from. Spend time in their spaces, offer feedback on their work, participate in their conversations. Then ask. This is a relationship investment, not a transactional exchange. The quality of testers you get correlates with the relationship quality.

If you show up to a community only to post "please test my game," you'll get low response rates and low-quality feedback. Communities reward contributors.

**Incentives that work**:
- Name in credits
- Payment (even small gift cards)
- Food and social occasions (pizza night for board game playtests)
- The excitement of being involved in game development

**Online options**:
- Submit to feedback-focused game jams where mutual playtesting among designers is the norm
- Reach out to small indie-focused streamers; their audiences provide additional observation data, and streamers verbalize their thought process constantly

**Local options**:
- Contact schools, colleges, or universities with design or computing programs
- Offer something in return (a talk or workshop about game development in exchange for student playtesting sessions)

**For ongoing Deep testing**:
- Build a dedicated feedback channel (Discord, Slack)
- Lower the barrier to contributing: no surveys, no forms, just a bot that collects messages
- Recruit genre-expert players who will stress-test and try to break the game

## Metrics Collection

Passive data collection scales far better than active feedback methods. An in-house metric server collecting anonymous data on every run (cards, items, events, choices, duration) enables objective decision-making even in early development.

**What metrics enable**:
- Identifying outlier content or strategies without relying on player reports
- Sorting data by difficulty level or player skill for granular balance insights
- Catching silent player behavior (players who never give written feedback still generate useful data)
- Validating or challenging qualitative impressions with hard numbers

**Self-selecting difficulty as a data tool**: Incremental, unlockable difficulty levels (rather than simple easy/medium/hard menus) cause players to naturally climb to their real skill ceiling. This creates organic skill-cohort segmentation in your data without manual tagging.

**Critical limitations**: See `gotchas.md` for survivorship bias, sampling bias, and other metrics traps.
