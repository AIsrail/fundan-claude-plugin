---
name: grant-fit
description: Check whether a specific open grant or program from Fundan fits the user's project — go / no-go with blockers, fixes and what to prepare. Use when the user asks "does this grant fit me", "can we apply", or names a Fundan program id. Проверка «подходит / не подходит» для конкретного гранта.
---

# Grant fit check (go / no-go)

1. Get the program: call `get_grant` with its id (find it with `search_grants` first if needed). If the tool says full access is required, tell the user in one sentence and give the link — do not guess the program's conditions.
2. Get the project facts (ask only what is missing): applicant type and registration country, organization age, project topic and region, requested amount, timeline, partners.
3. Compare strictly against the program card — `who_can_apply`, `restrictions`, `geography`, `amount`, `deadline`, `description`. Do not add conditions that are not in the card; if the card is silent, say "not stated — confirm on the official page".
4. Answer in the user's language in this order:
   - **Verdict:** Go / Go with fixes / No-go — one sentence why.
   - **Blockers:** hard mismatches (eligibility, country, applicant type, closed topic, deadline too close).
   - **Fixes:** what would remove each blocker (partner organization, smaller budget, different framing).
   - **What to prepare:** documents and steps before the deadline, with the days left.
   - **Official link.**
5. Be honest: if the chance is low, say so and suggest searching for a better match.
