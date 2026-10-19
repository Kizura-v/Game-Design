# Question, Decision & Category Templates

## Category card
```md
# [Category] — [Game]
Status: Needs decisions | Ready for implementation audit | ...
Sources of truth:
Existing implementation and tests:
Gameplay purpose:
Major loop or minor supporting function:
Known locked decisions:
Open material design questions:
System owner / related categories:
Non-goals and intentionally deferred scope:
Verification and runtime gaps:
Next implementation/audit step:
```

## One interactive quiz decision
Ask a single major design question; offer A, B, C, D and Other where meaningful. State the recommendation and why. Require explicit confirmation **before** locking or committing the choice. Don't recommend new features solely to fill a category.

```md
# [PREFIX-001] [Decision title]
Context: [existing locked facts]
Why this decision matters: [player effect or architectural boundary]
A: [option + tradeoff]
B: [option + tradeoff]
C: [option + tradeoff]
D: [option + tradeoff]
Other: [custom]
Recommendation: [letter and rationale]
Confirmation: [awaiting choice]
```

## Locked decision record
```md
ID:
Date:
Status: Locked design
Category and owning document:
Choice:
Player-facing behavior:
Required invariants / affected interfaces:
Rationale and alternatives:
Dependencies and compatibility:
Deferred implementation/tuning questions:
Acceptance criteria:
Verified evidence (if any):
Reason to reopen:
Superseded notes and reversal path:
```

## End-of-category handoff
```md
Stop gate: Passed / Not yet
Defined gameplay loop:
Agreed scope and non-goals:
Implementation owner to audit:
UE native/reuse candidates to inspect:
Cross-system integration:
First production-facing acceptance scenario:
Automated verification:
Visible player/playtest verification:
Performance budget and measurement (if relevant):
Blocked on:
```

**Rule:** Never claim implementation, test coverage or engine validation solely because design files were committed.
