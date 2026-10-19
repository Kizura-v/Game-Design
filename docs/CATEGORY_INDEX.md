# Universal UE5 Game Design Categories

These are **optional areas for consideration**, not requirements that every game must implement. Select and merge as appropriate to genre and goals.

| Domain | Category / Prefix | Core quiz scope |
| --- | --- | --- |
| Product | Product vision & pillars / VISION | Audience, fantasy, platform, genre, differentiator |
| Product | Main gameplay loops / LOOP | Core actions, reward loop, retention, pacing, friction |
| Core | Combat / COMBAT | Only if applicable: inputs, targeting, encounters, balance, damage |
| Core | Skills, levels & progression / PROG | Advancement, rewards, unlocks, caps |
| Core | Companions, NPCs & AI / AI | Agents, autonomy, behaviors, party roles |
| Core | Quests, objectives & storytelling / QUEST | Mission patterns, discovery, branching, consequences |
| Core | Tutorial & onboarding / TUTORIAL | Learning path, guidance, first-session UX |
| Core | Camera, controls & interaction / CAMERA | View, movement, focus, targeting, input feel |
| World | World structure & procedural generation / WORLD | Geography, authored content, seed determinism, traversal |
| World | Exploration, navigation & travel / TRAVEL | Routes, mobility, discovery, transport |
| World | Time, calendar, seasons & weather / TIME | Simulation pace and gameplay relevance |
| World | World events & encounters / EVENT | Triggers, outcomes, consequences, frequency |
| World | Custom emergent threat/director systems / DIRECTOR | Optional systemic events, escalation and persistence |
| World | Ecology, resources & harvesting / RESOURCE | Availability, respawn/depletion, gathering roles |
| Creation | Building & construction / BUILD | Placement, permissions, pieces, ownership, upgrades |
| Creation | Crafting & production / CRAFT | Recipes, workstations, manufacturing, quality |
| Creation | Fishing & side activities / SIDE | Major skill vs lightweight function, time cost, rewards |
| Creation | Farming, cooking & survival / SURVIVAL | Optional sustenance, agriculture, meaningful constraints |
| Creation | Inventory, storage & equipment / INVENTORY | Capacity, management, equipping, interactions |
| Creation | Logistics, transport & automation / LOGISTICS | Movement of materials, routes, delegation |
| Creation | Economy, vendors & trading / ECONOMY | Prices, market interaction, supply, progression |
| Social | Guilds, factions & reputation / FACTION | Affiliation, benefits, consequences, roles |
| Social | Singleplayer, co-op & multiplayer / MODE | Hosting, authority, join/leave, persistence, scale |
| Social | Accounts, login, profiles & saves / ACCOUNT | Decide whether remote accounts are needed at all |
| Presentation | UI, HUD & maps / UI | Information, feedback, layouts, accessibility |
| Presentation | Menus, bindings & configuration / SETTINGS | Rebinding, controls, settings, pause |
| Presentation | Sound, music, voice & subtitles / AUDIO | Player feedback, mixing, spatial cues |
| Presentation | Art, animation & VFX / VISUAL | Style, readability, motion, feedback, budgets |
| Technical | Architecture, persistence & authority / ARCH | Only critical invariants, ownership, extensibility |
| Technical | Optimization & scalability / OPT | Forward budgets, profiling, per-system and final passes |
| Technical | UE tooling, plugins & content workflow / TOOL | Build-vs-reuse, editors, asset pipeline |
| Technical | Testing, packaging & release / RELEASE | Platforms, acceptance, regressions, release process |

## Suggested directory layout
```text
docs/
  QUIZ_WORKFLOW.md
  CATEGORY_INDEX.md
  DECISION_TEMPLATES.md
  decisions/
    README.md
    core/
    world/
    creation-economy/
    social/
    presentation/
    technical/
    Outdated/Archive/
```
Create category records as needed. Avoid empty placeholder files and duplicate authorities.

## Coverage review
For each selected category track: Not assessed / Needs decisions / Ready for implementation audit / Implemented / Validated / Deferred / Removed. Record source link, owner, dependent categories and next tangible implementation evidence.
