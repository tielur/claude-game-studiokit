# Scope Review Gotchas

These are failure modes that consistently derail scope decisions. Flag them when you see them.

## Treating constraints as obstacles instead of blueprints

Ask "what game does this constraint want us to make?" not "how do we work around this?" Teams that design around constraints produce bloated, unfocused games. Teams that design with constraints produce focused, shippable ones. Constraints aren't the enemy of creativity -- they're the forcing function that produces it. A game built under four hard constraints (limited input, platform compatibility, specific audience, tight budget) will often be sharper and more coherent than an unconstrained brainstorm.

## The "one more go" test

Don't add content until playtesters spontaneously resist stopping. "Give me one more go" is proof that the core loop works. If you don't have it, you don't have a game worth expanding -- you have a prototype that needs more design work, not more content around it. Content creation feels like progress and provides visible output to share, so developers default to it. But adding levels, story, and systems to an unproven core is building on sand.

## Under-cutting during simplification

If you didn't add back at least 10% of what you cut, you probably didn't cut enough. Most designers under-cut. The instinct is to keep things, rationalize their value, and preserve the original vision. The discipline is to cut past comfort and see what actually breaks. Simplicity is a means to player engagement, not an end in itself -- but most projects err heavily toward too much, not too little.

## Saying no to expected genre features

Conventional wisdom says: give players what they expect from the genre. But consistently rejecting genre-standard features that don't serve your core (XP systems, equipment, prestige mechanics, skill trees) often produces a game that feels more novel and cohesive, not less complete. Players respond to intentionality -- a game that clearly knows what it is reads as confident, even when missing expected features. Cutting expected features and leaning into what remains often produces a more distinctive game than including everything the genre assumes.

## Development vs. design are separate activities

Time spent debugging, optimizing, refactoring, or learning tools is development, not design. Design is thinking about the end user, playtesting, and iterating based on player response. A developer can spend years opening an engine, writing code, and adding art without ever doing the design part. Scope estimates must account for both -- and teams routinely undercount design time because development time is more visible and feels more productive.

## Devlogs and community building as a validation trap

Positive community feedback on progress doesn't predict commercial success. Devlog comments validate visuals and effort, not gameplay. "Looks nice" about a game that would be unfun to play creates a feedback loop where developers keep polishing and adding content to something whose core loop has never been tested. Visual praise is not the same as someone resisting putting the game down. Community building is valuable, but it's marketing -- not validation of fun.

## Demo playtime devaluing the full game

A demo that's too long erodes the perceived playtime of the purchase. Players who spend 60-70 minutes maxing out a "30 minute" demo then experience the full game as shorter than it actually is, because they don't credit demo time toward what they purchased. A demo that's too short fails to demonstrate depth. The demo is a scope decision with direct commercial consequences -- it needs its own design constraints, not just a slice of the full game.

## Deferred features tend to get cut

If a feature is "for later," treat it as probably not shipping. Deferred features still carry hidden design weight -- they influence architecture, UI layout, save systems, and balance even when not yet built. Either commit to the feature now and account for it in the scope, or cut it entirely. The backlog is not free storage. Features that linger accumulate hidden dependencies and emotional attachment, making them harder to cut when the time comes.

## Art pipelines are the most commonly underscoped system

Content pipelines scale linearly with ambition. Each unique visual requires concept, production, iteration, and integration across multiple contexts (gameplay, menus, marketing, store pages). Code can be refactored and mechanics simplified, but hand-crafted visual assets have a hard floor on production time. For small teams, stylized or procedural art approaches vastly outperform hand-crafted assets per hour invested. Evaluate content volume early and honestly.

## Engine or tool upgrades mid-project

Upgrading an engine, framework, or major dependency mid-project creates invisible maintenance burden. Every workaround, every integration point, every downstream system that touches the upgraded component needs testing and often fixing. Document third-party workarounds with enough context that you'll understand them months later, and review the list before any upgrade. Budget explicitly for the cascade, or freeze tools early and live with known issues until after ship.
