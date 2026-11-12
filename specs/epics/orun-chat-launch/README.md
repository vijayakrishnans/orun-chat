# Epic: orun-chat-launch (OC)

**There is no Orun Chat today. This epic puts a plain AI chatbot live on stage and prod — streaming chat on Workers AI, history in D1, uploads in R2 — by building it from the `nuxt-ai-chatbot` baseline, so the first release needs no AI key and no custom code.**

Orun Chat is for anyone who wants a private AI chat on their own Cloudflare account. When it ships, a visitor can open the site, chat with a Workers AI model, and find the chat in their history after a reload. Persona, knowledge and embedding are later epics.

## Status

| Field | Value |
|-------|-------|
| Status | In progress |
| Cluster | **OC** (OC0–OC2) |
| Owner(s) | `apps/web` (the Nuxt app and its Nitro API) · `infra` (D1 and R2 roots) |
| Builds on | `nuxt-ai-chatbot baseline-v2` — chat, history, uploads, sign-in as shipped |
| Changes | Adds the product as built; changes nothing in the baseline's contexts |
| Decisions locked | (1) Workers AI through the binding; no vendor key. (2) Cloudflare only: D1 + R2, no Supabase. (3) GitHub sign-in waits for the owner's OAuth app. |
| Gate | OC1 is the first user-visible change; OC2 is the first change of our own. |
| Shipped as | |

## Read order

1. `design.md`
2. `implementation-plan.md`
3. `risks-and-open-questions.md`
4. `IMPLEMENTATION-STATUS.md`

## Milestones at a glance

| Milestone | What it lands | Done when |
|---|---|---|
| OC0 — the spec | this doc set | merged; `task_get OC-1` reads done |
| OC1 — plain chatbot live | the baseline build, branded Orun Chat | stage and prod answer; a chat streams and persists across a reload |
| OC2 — chessboard background | a subtle chessboard behind the chat, light and dark | the squares show on stage and prod; chat text stays readable |
