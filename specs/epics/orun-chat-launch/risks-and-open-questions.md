# orun-chat-launch — risks and open questions

## OC-A — Workers AI cost and limits (ACCEPTED)

Every chat spends Workers AI neurons on the owner's Cloudflare account. The free allotment covers a demo; heavy use bills on Workers Paid.

## OC-B — Supabase or Cloudflare only (RESOLVED)

`ai-chatbot` needs Supabase and both free projects; `nuxt-ai-chatbot` needs Cloudflare alone and builds in about 7 minutes. Chosen: `nuxt-ai-chatbot`.

## OC-C — GitHub sign-in (RISK, mitigated)

Sign-in needs an OAuth app the platform does not broker. Until the owner adds it, chat works as a guest; the README says how to connect it.
