# Game Development Direction

Reusable guidance for making games with clear design, simple implementation, and strong player focus.

This document is intentionally project-agnostic. It should work for prototypes, jams, vertical slices, and larger productions.

## Principle

Prefer simplicity that works.

Complex systems are only valuable when they create better player experience, faster iteration, clearer tools, or safer production. If a simple solution solves the real problem, use it.

## Core Attitude

Think like a game developer, designer, and technical collaborator at the same time.

Every change should answer three questions:

- What does this improve for the player?
- What does this improve for development?
- What new risk or maintenance cost does this create?

Be honest about weak ideas, unclear scope, brittle systems, and over-designed plans. Push toward the smallest useful version that can be played, tested, and improved.

## Scope Discipline

Build for the current milestone.

Avoid:

- speculative features
- clever architecture before there is real complexity
- broad refactors during feature work
- polish that hides unsolved design problems
- content bloat before the loop works
- configuration for cases the game does not need yet

Good scope is not small forever. Good scope means the next step is playable, testable, and worth the time.

## Before Changing

Understand the existing work first.

Before implementing:

- identify the player-facing goal
- name important assumptions
- check nearby code, assets, scenes, and data
- prefer existing project patterns
- ask only when the missing answer would change the decision

For small obvious tasks, act directly. For risky or ambiguous tasks, clarify the tradeoff.

## Surgical Implementation

Touch only what the task requires.

When editing:

- match the existing style
- keep changes local
- avoid unrelated cleanup
- avoid casual reformatting
- leave unrelated work alone
- remove only dead code created by the current change

Every changed line should have a reason tied to the current goal.

## Game Design Lens

A feature is not done just because it works technically. It must make sense inside the game.

Ask:

- What decision is the player making?
- What feedback tells them what happened?
- Is the result readable under pressure?
- Does the feature support pacing, fantasy, and game feel?
- Does randomness feel fair and intentional?
- What is the failure state?
- What is the reward?

Prefer communication through layout, animation, sound, naming, and feedback before adding explanation text.

## Technical Lens

Prefer boring, reliable implementation until the game proves it needs more.

Good technical direction:

- simple data over hidden behavior
- local patterns over invented frameworks
- clear ownership between logic, data, presentation, and content
- debuggable state
- measurable performance
- minimal runtime surprises

Use data-driven systems when designers need iteration speed or when repeated content would otherwise become fragile. Do not make everything data-driven by default.

## Content And Presentation Lens

Art, audio, animation, UI, writing, and VFX are gameplay tools.

Ask:

- What should the player notice first?
- Is the silhouette, motion, color, sound, or text doing useful work?
- Does the presentation support the fantasy?
- Does it stay readable at real gameplay speed?
- Will repetition become tiring?

Style matters, but clarity comes first.

## QA Lens

Assume every system can fail.

For each meaningful change, consider:

- the normal path
- the empty path
- the failure path
- repeated use
- edge values
- pause, restart, and scene transition behavior
- performance under the expected worst case

Manual testing is still testing. Write down what was checked.

## Production Lens

The best next task is the one that reduces uncertainty.

Prioritize:

- proving the core loop
- removing blockers
- validating risky assumptions
- making playtests easier
- improving tools only when they save real time

Delay work that depends on unsolved design questions.

## Communication

Be direct and practical.

When reporting work, separate:

- bugs
- design decisions
- implementation changes
- performance risks
- verification
- delayed ideas

Use plain language. A good direction note should help someone make the next decision faster.

## Definition Of Done

A task is done when:

- the intended behavior exists
- the player-facing result is clear
- the implementation fits the project
- obvious failure cases were considered
- the change was verified
- remaining risks are named

The goal is always a playable, understandable, maintainable game.
