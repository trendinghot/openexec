\# OpenClaw



\*\*Deterministic execution engine for governed systems.\*\*



OpenClaw is responsible for \*doing work\* — not deciding whether work should be done.



It executes tasks \*\*only after\*\* governance approval has been granted by ClawShield.



---

## System architecture

This project is part of a three-layer governed execution system:

- **OpenClaw** executes actions deterministically.
- **ClawShield** governs whether actions are permitted before execution.
- **ClawLedger** records immutable receipts of what was decided and why.

Execution, governance, and evidence are intentionally separated.
No layer replaces another.
Together, they make autonomous systems legible, reviewable, and defensible.



\## What OpenClaw does



\- Executes approved actions

\- Produces execution outcomes

\- Emits execution metadata for receipts

\- Operates deterministically given the same inputs



---



\## What OpenClaw does NOT do



\- It does not define policy

\- It does not approve intent

\- It does not override governance

\- It does not self-authorize execution



---



\## Relationship to ClawShield



\- \*\*ClawShield\*\* decides \*whether\* an action may proceed  

\- \*\*OpenClaw\*\* performs the action \*after approval\*



OpenClaw trusts governance receipts.

ClawShield never executes.



---



\## Design principles



\- Execution must be \*\*deterministic\*\*

\- Side effects must be \*\*observable\*\*

\- Failures must be \*\*explicit\*\*

\- Silence is preferable to speculation



---



\## Status



This repository defines the \*\*execution contract\*\* for OpenClaw.



The running system may be implemented elsewhere.



---

## Related repositories

- **ClawShield** — Governance sidecar (policy + preflight)  
  https://github.com/trendinghot/clawshield

- **ClawLedger** — Witness ledger (immutable receipts)  
  https://github.com/trendinghot/clawledger


---

\## License



To be defined.



