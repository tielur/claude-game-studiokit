# Polish & Identity Framework

## Core Principle: Consistency Beats Quality

Players cannot evaluate isolated assets -- they evaluate patterns. An inconsistent high-quality asset reads as an anomaly. A consistent mid-quality asset reads as intention, craft, and identity. The payoff from reinforcing your own rules compounds over time in a way that individual asset polish does not.

Pick constraints and stick to them. Mixed resolutions, clashing art styles, and inconsistent UI elements break the visual contract with the player faster than low-fidelity art does.

## Audio-Visual Partnership

Audio and visual direction derive from the same problem: establishing and reinforcing identity. Treating them as separate pipelines that converge at the end produces games where each is good but they don't reinforce each other. Without shared vocabulary and early alignment, "making the game feel right" means something different to the artist and the sound designer.

Both palettes should derive from the same theme and constraints, established together from the start.

## Identity Palette Method

1. Find the theme or essence of the game -- the thing that makes it special
2. Derive a color palette from that theme
3. Derive a sound palette from the same theme (ask: what constraints does this theme imply for audio?)
4. Choose a constraint-identity pairing as the unifying rule (e.g., "only mouth-made sounds" or "one synthesizer" or "grayscale with one accent color"). This makes consistency automatic -- any decision that follows the rule is automatically in-palette
5. For every subsequent decision, ask: does this reinforce the palette or deviate from it?
6. Deviations that don't serve the identity should be cut; deviations that serve a deliberate purpose (subversion, focal point) should be intentional and spaced out

### Practical + Conceptual Constraint Pairs

Two types of constraints serve different purposes:

- **Practical constraint:** A single rule that determines what tools or elements are allowed (mouth sounds only, one synthesizer, grayscale only). Enforces consistency mechanically.
- **Conceptual constraint:** A thematic or experiential goal that all decisions must serve (make the player feel small, make everything look delicious, make the world feel tangible). More open in what is permitted, but requires constant evaluation.

Pick at least one of each. A practical constraint paired with a conceptual one produces distinctive visual and audio language.

## Pattern-Pop-Subversion Sequence

1. **Establish patterns** through consistent repetition (color coding, sound signature, recurring element). This is the baseline.
2. **Set expectations** -- players learn what is "normal" and start relying on the pattern.
3. **Deploy "pop" sparingly** -- moments that break the pattern for emphasis. Pop works because the pattern makes it legible.
4. **Reserve subversion** for moments where breaking the expectation has narrative or emotional meaning. Subversion is entirely dependent on the player having been trained by the pattern.

Without an established pattern, pop becomes noise and subversion is invisible.

## Audio Evaluation

**Three-function test:** Does each sound (1) cue a gameplay state the player needs to act on, (2) confirm or deny a player decision, or (3) reinforce the emotional tone of the game? If a sound fails all three, it is likely unnecessary noise.

**ADSR as emotional dial:** The envelope of a sound controls its emotional shape more than the sound source itself.
- Longer attack = anticipation, less immediacy
- Shorter attack = snap, urgency
- Longer release = weight, persistence, power
- Shorter release = precision, finality

These are conscious design choices, not just technical settings. The same raw sound reshaped through ADSR can serve completely different emotional purposes.

**Frequency-split attenuation:** Assign short attenuation distance to high frequencies and long attenuation to low frequencies. This creates spatial realism from a single asset -- one sound effect behaves like many different sounds across distance without additional content production.

**Reverb as diagnostic:** If a scene feels disjointed, try shared reverb before assuming individual sounds are wrong. Reverb glues sounds to each other and to the environment. If the scene feels more unified after shared reverb, the problem was environmental context, not the raw sounds.

**Sound shapes player behavior below conscious awareness:** A weak-sounding weapon makes players cautious; a powerful-sounding one makes them aggressive. This happens below conscious attention. Audio should feel inevitable, not impressive -- the moment players consciously notice the audio doing its job, it stops working.

**Realistic + abstract layering:** For games with tangible worlds, give physical objects (vehicles, tools, doors) realistic sounds to ground believability, and give player interactions (combat, crafting, collection) abstract sounds that prioritize feel over realism. Only realistic sounds makes interactions feel dry; only abstract sounds makes the world feel arbitrary.

## Visual Evaluation

**Color coding as free genre convention:** Top-down processing means genre-familiar players already know what standard color codings mean before you explain them. Red = danger, green = safe, gold = reward. Using these conventions gets comprehension for free. Subvert only after establishing the pattern first.

**Bottom-up vs top-down processing:** Silhouettes and color register instantly (bottom-up). Players identify elements by shape and hue before reading any detail. Detail and texture engage top-down processing. Design for both: readable at a glance, rewarding up close.

**Space out the highs:** If everything glows, pulses, and sparkles, nothing stands out. A screen shake on a critical hit means nothing if the screen shakes on every hit. Focal points in art and audio only work in relation to the ambient level around them. Restraint creates contrast, and contrast creates impact.

## Typography Evaluation

**Two-font visual language system:** One font for headers/UI (carries personality), one for body text (carries information). More than two increases cognitive load that compounds across every screen, every dialogue box, every inventory panel for the entire play session.

Assign each font a role and enforce it everywhere:
- Before adding any new font or variant (bold, italic, underline, color change), write a one-sentence rule for what that variant means
- Apply that rule everywhere without exception
- When edge cases arise (damage numbers, special UI states), explicitly decide whether they get a new rule or use an existing one -- never let it be ad hoc

**Legibility directly affects player performance, not just comfort.** Hard-to-read fonts on gameplay-critical text measurably degrade how well players execute those mechanics. This is a causal chain, not just a correlation. Decorative fonts in tutorial text, item descriptions, or ability explanations don't just frustrate players -- they measurably worsen execution.

**Typography carries material associations:** Serif fonts carry chisel-on-stone associations; blackletter carries quill-and-angle; monospace carries typewriter/terminal; sans-serif carries mechanical printing. These are embedded in letterform geometry -- players pick up on physical production traces even when they can't articulate why a font "feels wrong" for a setting.

**Font semiotics research method:** Find primary sources from the game's setting (transit guides, military manuals, period advertisements, restaurant menus) rather than browsing font libraries. Derive typographic rules from authentic materials. The authenticity difference is perceptible even to players who can't name why.

**In-world vs UI text:** Environmental text (shop signs, posters, notices) can use varied typography to signal period authenticity or a lived-in world. UI and gameplay-critical text should remain clean and consistent. The two-font rule applies to the player-facing interface; in-world text follows the world's rules.

## Game Feel

**Responsiveness:** Input-to-response latency, animation canceling, buffer windows. A fast action game with sluggish sound effects feels wrong even if each element is high quality in isolation.

**Weight:** How physical do actions feel? Is weight consistent with the game's fantasy? Match the ADSR envelope, visual impact effects, and screen response to the intended feeling.

**Feedback layering:** Visual + audio + haptic reinforcing the same moment. Every non-mechanic element (music, camera angles, animation style, sound design) feeds the player's emotional experience and must vote in the same direction as the mechanics. When evaluating polish, check whether the audiovisual layers reinforce or contradict the game's intended feeling.
