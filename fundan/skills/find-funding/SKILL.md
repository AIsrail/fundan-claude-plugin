---
name: find-funding
description: Find currently open grants, investors, accelerators or SME finance for a project in Central Asia (Kyrgyzstan, Kazakhstan, Uzbekistan, Tajikistan) using Fundan. Use when the user asks where to get funding, which grants are open, or what deadlines are coming. Подбор открытых грантов и финансирования для проекта в Центральной Азии.
---

# Find funding with Fundan

1. Find out (ask only what is missing, one short question at a time):
   - the project topic;
   - who applies: NGO, business or individual;
   - the applicant's country (KG, KZ, UZ, TJ).
2. Translate the topic into 1–4 Russian keywords (the database is in Russian) and call `search_grants` with `query`, `applicant`, `country`. If nothing is found, retry with broader keywords once.
3. Show results in the user's language, soonest deadline first. For each: name, amount, deadline (or "open all year"), who can apply, official link. Translate names and descriptions; keep the id for follow-ups.
4. Never invent programs, amounts or deadlines. If a field is empty, say "not specified — check the official page".
5. If the response contains `more_with_full_access`, say in one sentence how many more matching programs are open and give the `upgrade` link. Do not push further.
6. Offer the next step: "Want me to check whether one of these fits your project?" — then use the `grant-fit` skill.

Also useful: `urgent_deadlines` (deadlines within 7 days), `market_overview` (what is open right now by type and topic).
