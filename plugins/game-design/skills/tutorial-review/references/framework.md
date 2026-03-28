# Tutorial Review Framework -- Reference

## Does This Mechanic Need a Tutorial?

A five-step decision process. Work through these in order:

1. **How critical is it?** Is this a core loop mechanic the player uses constantly, or an optional system they might never touch? Core loop mechanics carry a higher teaching obligation.
2. **How discoverable is it?** Can a player find this through normal play (interacting with the world, pressing buttons, experimenting), or is it hidden behind a specific input sequence or modal system that nothing in the environment suggests?
3. **Is it a genre convention?** Players of this genre already know this pattern from other games. Genre-conforming mechanics carry transfer effects that reduce or eliminate the need for explicit teaching.
4. **What's the risk of confusion?** If the player misunderstands this mechanic, does it lead to frustration and blocked progress, or just slightly suboptimal play they won't even notice?
5. **What's the cost of failure?** Does getting this wrong mean death and restart, or a minor setback the player can recover from naturally?

**Decision rule**: If a mechanic is critical + low discoverability + high confusion risk + high failure cost, it requires explicit teaching. If it's optional + discoverable + genre convention, let players find it. Most mechanics fall between these extremes -- use the five factors to calibrate how much teaching is appropriate.

## Environmental Teaching Structure (Three-Beat)

The standard structure for teaching through play rather than text:

1. **Safe encounter**: The player meets the mechanic in a zero-risk context. They can experiment, fail, and retry without consequence. The goal is familiarity, not mastery.
2. **Low-stakes test**: The player must use the mechanic with mild consequences for failure. This confirms understanding and builds muscle memory. Failure here should cost seconds, not minutes.
3. **Real challenge**: The mechanic is now one tool among many in a genuine gameplay scenario. The player must choose when and how to apply it under real pressure.

This structure works because it builds muscle memory before demanding performance. Skipping to step 3 forces players to learn and perform simultaneously, which splits attention and increases frustration.

**Limitation**: This structure works reliably for implicit/systemic rules (fire burns wood, enemies react to sound) where players can generalize from examples. It breaks down for explicit/modal rules (specific input sequences, timing windows, conditional triggers) because observation doesn't communicate the precise constraint. Modal rules need direct communication.

## Implicit vs. Explicit System Classification

This distinction determines which teaching method is viable:

**Explicit systems** have specific inputs that produce specific outputs with no room for player improvisation. The rules are modal -- they activate under precise conditions. Examples: directional parry requirements, hold-to-activate abilities, specific button combos, conditional triggers. Players cannot intuit these from context. They must be told.

**Implicit systems** have rules that blend, extend, and produce emergent behavior through player experimentation. The rules feel physics-like -- they generalize. Examples: elemental interactions, AI behavior patterns, momentum and physics systems, environmental destruction. Players can discover these through play because the rules behave consistently and predictably once encountered.

**The classification mistake**: Teaching implicit systems explicitly spoils discovery -- this is one of the game's rewards. Leaving explicit systems to be discovered creates confusion -- the player has no path to the answer through experimentation alone. Match the teaching method to the system type.

## Show-Don't-Tell Hierarchy

Ranked from most to least player agency:

1. **Best -- player discovers through interaction.** No text, no prompts. The environment is constructed so that natural play reveals the mechanic. This only works when the mechanic is discoverable through experimentation.
2. **Good -- environment demonstrates.** An NPC performs the action, a visual sequence plays out, or an environmental event shows the mechanic in operation. The player observes before they act.
3. **Acceptable -- contextual prompt appears when relevant.** A button prompt near an interactable, a tooltip on first encounter, a brief instruction when the mechanic becomes necessary. Shown at the moment of need, not before.
4. **Last resort -- text explanation or cutscene.** A tutorial screen, text box, or non-interactive sequence explains the mechanic. This is documentation, not teaching.

Each level down reduces player agency and engagement. Default to the highest feasible level for each mechanic. The feasible level depends on the implicit/explicit classification -- implicit systems can reach level 1; explicit systems often can't go above level 3.

## Mystery as Design Feature vs. Betrayal

Not all withheld information is a tutorial failure. The test is whether the player's confusion is productive or destructive:

- **Design feature**: Withholding information that creates curiosity and motivates exploration. The player doesn't know what's behind the locked door, what the cryptic item does, or how the hidden system works -- and this uncertainty drives engagement. The game's contract with the player includes discovery.
- **Betrayal**: Withholding information that blocks progress or creates frustration. The player doesn't know how to use a critical mechanic, can't understand why they're failing, or misses core functionality because nothing taught them. The game's contract implied teaching and didn't deliver.

**The diagnostic question**: Is the player's confusion motivating exploration, or motivating quitting? If the answer depends on player patience rather than design intent, the information is probably being withheld accidentally, not deliberately.

## Genre Contract Alignment

Players arrive with a set of expectations from other games in the genre. These expectations form an implicit contract:

- **Mechanics that conform to genre conventions** require no teaching. Players transfer knowledge from prior experience. Teaching what players already know wastes time and patronizes.
- **Mechanics that deviate from genre conventions** require explicit teaching. Players will apply their prior expectations and get confused when the mechanic behaves differently than expected. The deviation itself is the teaching obligation.

**Audit process**: Map which of the game's mechanics match genre conventions and which deviate. Only deviations need tutorials. If the game is cross-genre or genre-defying, the teaching obligation increases because players have fewer reliable expectations to draw on.

## Layered Difficulty as Teaching Tool

Difficulty layers can function as progressive teaching:

- **Easy path** teaches the mechanic with fewer variables and lower pressure. The player learns the core behavior in a forgiving environment.
- **Hard path** rewards mastery of the mechanic with more variables, higher stakes, and greater demand for precision. This is the test of understanding.
- **Both paths should be visible** so the player understands they chose their difficulty. Invisible difficulty selection removes the teaching value because the player doesn't know what they opted out of.

This structure allows different players to self-select their teaching depth. Players who learn quickly take the hard path early. Players who need more practice take the easy path longer. Neither is forced through content that doesn't match their current understanding.

## Assist Modes as Design Communication

Offering an assist mode is itself a form of teaching:

- **What can't be adjusted** communicates what the game considers core to the experience. These are the mechanics the designer believes define the game.
- **What can be adjusted** communicates what the game considers peripheral -- important but not identity-defining.
- Frame assists as "experience customization" rather than difficulty reduction. This communicates design values honestly: the game has a specific intended experience, and the assist mode lets players adjust their path to it.

The selection screen itself teaches the player which challenges the game considers most important. A game that lets you skip combat but not puzzles is telling you it's a puzzle game with combat, not a combat game with puzzles.

**Framing matters**: Present the intended experience first, then offer adjustments. If the player encounters assist options before understanding what the game is trying to be, they can't make an informed choice about what to adjust.
