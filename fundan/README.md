# Fundan for Claude — open grants for Central Asia

Fundan connects Claude to a curated database of **currently open** grants, investors, accelerators and SME finance for Kyrgyzstan, Kazakhstan, Uzbekistan and Tajikistan, plus international programs open to the region. Ask in English or Russian, for example:

- "Which grants for education NGOs in Uzbekistan are open now?"
- "What deadlines are in the next 7 days?"
- "Does donor-17 fit our project?"

Fundan — это плагин для Claude с базой **открытых сейчас** грантов, инвесторов, акселераторов и финансирования для МСБ в Кыргызстане, Казахстане, Узбекистане и Таджикистане. Спрашивайте по-русски или по-английски.

## What is included

- **MCP server** `https://fundan.cc/mcp` with four read-only tools: `search_grants`, `urgent_deadlines`, `get_grant`, `market_overview`.
- **Skill `find-funding`** — asks what is missing (topic, applicant type, country), searches, and shows results soonest-deadline first.
- **Skill `grant-fit`** — a go / no-go check of one program against your project, with blockers, fixes and what to prepare.

## Free and full access

Free: programs with a deadline within 7 days, a few always-open programs, and the market overview; other matches are shown only as counts. Full access (all open programs and full cards) needs a paid Fundan access code from https://fundan.cc. Enter it when Claude Code asks for the plugin option "Fundan access code"; leave it empty for the free tier.

## Data and privacy

The plugin does not run any local code or scripts. It only connects Claude to the Fundan server over HTTPS. When Claude calls a tool, the arguments of that call (a search query in Russian keywords, an applicant type, a country code, a program id) and, if you entered one, your access code are sent to `https://fundan.cc/mcp`. Fundan answers with program data and does not store your queries or conversations; it keeps only anonymous aggregate usage counters. The access code is stored by Claude Code in your system's secure credential store. Privacy policy: https://fundan.cc/privacy

Only currently open programs are shown. Program data is in Russian; Claude translates it. Always confirm conditions and deadlines on the official link before applying.

## Install

Claude Code:

```
/plugin marketplace add AIsrail/fundan-claude-plugin
/plugin install fundan@fundan
```

Claude on the web or desktop (no plugin needed): Settings → Connectors → Add custom connector → `https://fundan.cc/mcp`. Step-by-step guide: https://fundan.cc/ai/claude

Support: connect4fund@gmail.com
