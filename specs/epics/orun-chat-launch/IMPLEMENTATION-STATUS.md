# orun-chat-launch (OC) — Implementation status

As-built ≠ intent. This file records what actually shipped, and every place
the code departed from `design.md`.

| Milestone | State | PR |
|---|---|---|
| OC0 — the spec | ✅ shipped 2026-11-12 | #3 |
| OC1 — plain chatbot live | ✅ shipped 2026-11-12 by the baseline build | #1, #2 |
| OC2 — chessboard background | ✅ shipped 2026-11-12: grey board (OC-2), then bold cream and brown (OC-3) | #4, #5 |

## Departures from the design

OC1 landed through the baseline's own tasks (BASE-1, BASE-2 in EP-1 `nuxt-ai-chatbot-baselining`) before this epic was minted, so it has no OC task of its own.

OC2 departs from the design's "two near-neutral tones": after the first grey board the owner asked for a bolder cream-and-brown board (#f0d9b5 / #b58863 at 4rem; #8b6b4a / #4a3221 in dark mode). The sidebar gained a `bg-default/70` surface so its muted text stays readable over the brown squares.
