# Level Design Framework -- Reference

This framework provides three complementary lenses for evaluating level design. Use whichever lenses fit the design being reviewed.

## Lens 1: Principles of Good Level Design

### Fun to navigate
Traversal has three gameplay vectors: observational (surveying surroundings), strategic (forming a plan), and navigational (actual movement). Use a consistent visual language of light, geometry, color, and animation to guide players along the critical path. What the player doesn't notice matters too: hidden collectibles and alternate speed paths reward exploration and replayability. Clarity (following visual cues to the goal) and depth (hidden paths, secret areas, speedrun routes) are separate layers that serve different players at different times.

### Does not cool the action
Empty spaces with nothing to do kill momentum. Every room, corridor, and transition should serve a purpose. Emptiness can work as a pacing tool when the absence of enemies IS the tension, but emptiness without tension is dead time. Space between encounters should contain discovery, narrative, or environmental interest. Rest is not the absence of content -- it is lower-intensity content.

### Tells a story through the broken circle
A good story is like a broken circle: the player fills in the gap. Three types of narrative in levels:
- **Explicit**: cutscenes, dialogue, text (creates the circle)
- **Implicit**: what the player figures out from the environment -- abandoned drinks, water-stained floors, period-mismatched decor all tell a story without words
- **Emergent**: the story the player creates through choice -- the freedom to poison a target, go in stealthily, or take a chaotic approach

**The broken circle as calibration tool:** Explicit narrative creates the circle. Implicit narrative creates the gap. Emergent narrative fills it. Over-communicating is as much a failure as under-communicating. To calibrate: (1) identify what you want the player to conclude, (2) decide what to tell them explicitly, (3) design the environment to create a gap, (4) leave room for player choice to fill it. If the gap is too large, players feel lost. If too small, they feel patronized.

### Teaches through play
The human mind enjoys processing patterns. Each level should introduce, showcase, or subvert a key mechanic. The gold standard structure: introduce equipment, design rooms that each teach a new use, test mastery with a boss or culminating challenge, then demand creative reuse in subsequent areas. The learning loop: Learn, Play, Challenge, Surprise -- and it nests fractally within levels and across the full game.

### Surprises
Don't follow predictable routines. The classic rollercoaster pacing (crescendos with troughs) becomes predictable if followed rigidly. Players learn the meta-pattern and anticipate the beats. Periodically violate the pattern deliberately -- use absence, sudden reversal, or subverted expectation. Some of the most memorable level moments emerge from working around constraints rather than executing a plan.

### Empowers the player
Empowerment means delivering on the level's specific promise, not necessarily a power fantasy. A meditative exploration game empowers emotionally. A horror game empowers through survival. A destruction-focused game lets the player reshape the world. The principle is "let the player feel the impact of their actions in a way that fulfills the game's central fantasy." Don't give players mundane tasks they could do in real life.

### Embeds difficulty through risk/reward pathways
Difficulty select screens ask players to evaluate difficulty before they've played -- an uninformed, irrevocable choice. The richer alternative is embedded risk/reward through multiple physical pathways:
- Design a base critical path at easy-to-medium challenge
- Add clearly signaled high-risk shortcuts with proportional rewards
- Add easier alternatives when the main path peaks in difficulty
- Use the level's visual language to make these paths legible (not hidden, but not mandatory)
- Audit: does any risk break the overall difficulty curve? If so, compensate dynamically

Players self-select difficulty through exploration choices, making continuous contextualized decisions rather than one upfront abstraction.

### Uses modular encounter design with modifier patterns
Design levels as strings of discrete, mechanic-driven modular encounters rather than continuous bespoke spaces. Each module can be recombined, reordered, or repurposed across multiple levels. Apply modifiers to existing modules (enemy type, lighting, objective, time pressure) instead of building new geometry. Design both inbound and outbound experiences differently -- same spaces, completely different gameplay logic (different enemies, mechanics, objectives, or environmental state). Backtracking without modification is a failure; modifier-driven bi-directionality is the technique.

### Creates emotion through space
Level design's closest art analogue is architecture. Spatial empathy techniques:
- Tight corners with limited field of view create tension and claustrophobia
- Twisting labyrinths create confusion, panic, and disorientation
- Wide-open sudden transitions from narrow spaces create wonder and awe
- Vast open space with no landmarks creates isolation and epic scale
- Enemies attacking from above create persecution
- Reward placed at the top of a tall structure creates hope and aspiration
- Heights with no safety net create vertigo

Work backwards from the desired emotion. Define the specific emotional response (not "fun" -- be precise: persecuted, exhilarated, desperate, full of wonder), then select spatial parameters, narrative elements, and mechanics that produce it.

### Supports concurrent objective structure
Present multiple objectives the player can complete in any order. Completing one objective modifies the remaining ones -- new paths open, difficulty shifts, narrative context changes. This creates a constantly evolving problem space rather than a checklist. Players author their own pacing through the order they choose.

## Lens 2: Design Layers

Layer game spaces with decision-rich design tied to curated narrative themes. Not infinite freedom, but player freedom within a curated space.

### Layer 1: Nonlinear, explorable space
Interconnected, circular spaces where multiple points of interest are visible from any position. Players read their surroundings and choose what to engage with. Every movement decision builds investment.

### Layer 2: Finite resources
Limited ammo and items with multiple purposes force measured, creative thinking. Switching between resource management and action engages different parts of the player's brain.

### Layer 3: Reactive physics
Not just crates and ragdolls. When physics interact with navigation and resource management -- spending finite resources to build new paths, for example -- the layers compound. Physics as a navigation tool is richer than physics as spectacle.

### Layer 4: Sensory-based AI
Enemies that see, listen, and get distracted. When enemies can be fooled by environmental manipulation, every object in the level becomes a potential tactical tool. Players question their surroundings: "Was that object there before?"

### Layer 5: Tactically advantageous space (safe zones)
Let players enter an area, feel relatively safe, and read the environment before action begins. Consistent object vocabulary: a fire-jetting pipe is always a real hazard, never a fake prop. Clear, honest communication through environmental design.

### Layer 6: Narrative as curation
Environmental storytelling lets players interpret locations and puzzle over details. Level design exercise: "What were the people in this space doing in the last hour of their lives?" Then populate accordingly. Props reinforce themes. Everything in the environment should have purpose and a reason for being there -- specific, not generic.

## Lens 3: System-Centric Puzzle Design

### Design the system first, find puzzles within it
"System-centric" means the entire game exists to showcase a discovered system. Puzzles serve the system, not the other way around. Players' motivation mirrors the designer's: excitement to see what the system can do next.

### Simplify to the minimum needed to convey the idea
Remove unnecessary solution steps that are too hard or unrelated. Trim the possibility space so fewer wrong paths exist. Easier than expected is often better when the goal is communication rather than testing.

### Keep puzzles bite-sized
Each puzzle should say: "did you know you can do this cool thing?" Some puzzles are "show levels" with no real challenge that simply demonstrate something delightful. Challenge is one tool, not the goal.

### Sequence puzzles as a distinct skill from puzzle creation
A well-designed puzzle in the wrong position teaches nothing. Key operations: insert, modify, delete, reorder, or optionalize puzzles. Sequence to build on previous knowledge: introduce a concept, test it, combine it with a prior concept, test the combination. Always give players access to multiple puzzles at once so no single puzzle becomes a hard gate.

### Use "things-almost-happen" as a generative playtesting method
When multiple playtesters attempt strategies that don't quite work, those failed attempts are design opportunities. Build content where that approach IS the solution. This crowdsources puzzle and challenge ideas from player intuition without additional brainstorming.

### Evaluate mechanics for naturalness, not just function
Mechanics that feel "kind of cool" but arbitrary are a warning sign. Mechanics that generate puzzles but feel bolted on -- external to the system rather than natural extensions -- add cognitive load and dilute the experience. Trust the "feels arbitrary" signal. Filter for "natural extension" not just "generates puzzles."

### Grey-box early validation
Risky or novel level ideas must be tested in grey-box (minimal art) form before investing in full art production. If the level doesn't work without polish, polish won't save it. A good idea that is never tested is a cut idea.

## Three Types of Narrative in Levels

When evaluating storytelling in a level, distinguish between:

1. **Explicit narrative**: cutscenes, dialogue, text, waypoints. Creates the story circle.
2. **Implicit narrative**: environmental storytelling. Abandoned party decorations, water-stained floors, period-mismatched decor. The player reads the space and fills in the story.
3. **Emergent narrative**: the story the player creates through choice. Missions where one player poisons the target, another goes in disguised, another snipes from a balcony. Each player leaves with a different story.

The strongest levels use all three, but implicit and emergent narrative are where level design does its best work. Explicit narrative is writing; implicit and emergent narrative are design. Emergent narrative is not designed -- it is enabled. You create the conditions (choice, varied mechanics, open-ended systems) that allow the player to generate story.
