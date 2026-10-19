# UE5 Game Design Quiz — Workflow and Stop Gate

## Mandatory rule

> Stop design questioning once the required gameplay behavior, major architecture, and critical invariants are sufficiently defined for implementation.
>
> Defer internal algorithms, concurrency details, and optimization mechanisms until implementation evidence demonstrates they are necessary.
>
> Prefer existing Unreal Engine capabilities and established project systems over new custom infrastructure.

## Quiz procedure
1. Inspect current code, game design documents, decisions, project assets and verification evidence **before** proposing questions.
2. Define the category's purpose, **major gameplay loop versus minor convenience feature**, player time/benefit, system boundaries, persistent state, and interfaces with other categories.
3. Ask **one decision that changes the product materially** at a time, using clickable A/B/C/D/Other choices and concise recommendation; confirm before locking.
4. Record the selected alternative, rationale, rejected alternatives, scope, impacted categories and evidence gaps. Never quiz settled questions without new contradictory evidence.
5. Apply the stop gate after every decision; if the remaining questions are about thread synchronization, exact cache policies, speculative micro-optimization, tuning constants, or implementation minutiae, mark them deferred and **stop**.
6. Inspect UE5 native facilities and already-owned project integrations, then implement and verify a coherent production-facing slice. Reopen design only when source, gameplay review or tests establish a real fork.
7. Use stable local IDs (e.g. COMBAT-001) and preserve original IDs when importing existing decisions. One authoritative owner per rule, links from dependent categories.

## The stop gate
Mark **Ready for implementation audit** when:
- player-facing behavior and intended core action/reward loop are defined;
- major constraints, essential failure handling and explicit non-goals are clear;
- shared authority, ownership, persistence and network boundary decisions that materially affect architecture are settled;
- the next step can be investigated in actual project source and Unreal systems;
- remaining questions are mainly engineering choices or numerical tuning.

If the category is low-value, **bench or remove it**, not elaborate it. No minimum number of questions.

## Prioritization
Evaluate **impact on gameplay**, player time, integration value, redundancy, implementation/maintenance cost and verification requirements. Core loops can justify depth; peripheral tasks should be fast, optional or automated if appropriate. Distinguish required architectural scope from optional scope expansion.

## Status taxonomy
Proposed | Open decision | Locked design | Ready for implementation audit | Source audited | Implemented | Integrated | Automated verified | Visually verified | Performance measured | Polished | Deferred | Superseded

Never represent design documents or successful commits as compiled gameplay, PIE, player-facing visual proof or GPU profiling.

## Conflict and revision policy
Cite competing current sources and their precedence. Recommend the best fit to the current goal and offer choices only for genuine forks. Retain superseded text or rationale in Outdated/Archive; state why it changed and how to revert.

## Unreal boundary
Assess native UE Tasks, PCG, World Partition, Enhanced Input, navigation, animation, ability/tag systems, audio and profiling **only where relevant** and only after checking the actual engine version/configuration. Do not assume any feature is enabled, or mandate a particular plugin.

## Verification handoff
Each completed category identifies an owning subsystem, integration dependencies, acceptance tests (automated and player-visible), save/reload/network implications as relevant, and measurable performance requirements when necessary.
