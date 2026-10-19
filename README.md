# Unreal Engine 5 — Game Design Questionnaire Template

A reusable, genre-neutral workflow for designing a UE5 game **without endlessly specifying hypothetical engineering internals**.

## Start here
1. [Quiz rules and stop gate](docs/QUIZ_WORKFLOW.md)
2. [Functional category index](docs/CATEGORY_INDEX.md)
3. [Decision and section template](docs/DECISION_TEMPLATES.md)
4. Create a project-specific copy of the working index and only activate categories that serve the game's goals.

**Core rule:** Stop questioning once gameplay behavior, major architecture, and critical invariants are clear enough to implement. Defer internal algorithms, concurrency and optimization specifics until implementation evidence demonstrates they are needed. Audit Unreal's native capabilities and existing project systems before introducing custom infrastructure.

This repo is a **template**, not a game specification or UE plugin. It prescribes no genre, camera, combat model, mandatory accounts, co-op, or specific engine plugin. Project implementations must verify engine version, source availability, builds and runtime tests themselves.
