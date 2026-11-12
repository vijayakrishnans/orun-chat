# orun-chat-launch — implementation plan

Milestones land in order, one task and one pull request each.

## OC0 — the spec

This doc set, merged to `main`.

**Done when**
- the five documents are on `main`
- `task_get orun-chat-launch` shows the epic with OC0 and OC1

## OC1 — plain chatbot live

The `nuxt-ai-chatbot` baseline-v2 build under the name Orun Chat: the D1 and R2 roots applied per environment, the schema migrated, the `web` Worker deployed to stage and prod.

**Done when**
- `https://orun-chat-web-stage.vijayakrishnan12994.workers.dev` and `…-prod…` answer 200
- a message on prod streams a Workers AI reply
- the chat is in the history after a reload

## OC2 — chessboard background

The app's own look: the page background becomes a subtle chessboard of alternating squares, drawn in CSS (no image), tuned separately for light and dark mode, with the chat column kept on a solid surface so text stays readable.

**Done when**
- stage and prod show the chessboard behind the chat in light and dark mode
- messages and the prompt box read as clearly as before

## Sequencing note

OC1 is the baseline's own one landing (it shipped before OC0 merged); OC0 records the design of what it landed. OC2 follows OC0.
