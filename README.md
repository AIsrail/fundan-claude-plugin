# Fundan for Claude — open grants for Central Asia

**EN.** Fundan connects Claude to a curated database of **currently open** grants, investors, accelerators and SME finance for Kyrgyzstan, Kazakhstan, Uzbekistan and Tajikistan, plus international programs open to the region. Ask in English or Russian:

- "Which grants for education NGOs in Uzbekistan are open now?"
- "What deadlines are in the next 7 days?"
- "Does donor-17 fit our project?"

**RU.** Fundan подключает Claude к базе **открытых сейчас** грантов, инвесторов, акселераторов и финансирования для МСБ в Кыргызстане, Казахстане, Узбекистане и Таджикистане. Спрашивайте по-русски или по-английски.

## Install / Установка

**Claude Code**
```
/plugin marketplace add AIsrail/fundan-claude-plugin
/plugin install fundan@fundan
```

**Claude (web / desktop)** — Settings → Connectors → Add custom connector → URL `https://fundan.cc/mcp`

## Free and full access / Бесплатно и полный доступ

| | Free / Бесплатно | Full / Полный |
|---|---|---|
| Deadlines within 7 days / Дедлайн ≤ 7 дней | ✅ | ✅ |
| A few always-open programs / Несколько программ «круглый год» | ✅ | ✅ |
| Market overview / Обзор рынка | ✅ | ✅ |
| All open programs, full cards / Все открытые программы, полные карточки | count only / только число | ✅ |

Full access: get a Fundan access code at https://fundan.cc/en/pay (USD) or https://fundan.cc (KGS), then:
- Claude Code: set the environment variable `FUNDAN_CODE=<your code>`;
- Claude web/desktop: use the connector URL `https://fundan.cc/mcp/<your code>`.

Полный доступ: код Fundan на https://fundan.cc, затем переменная `FUNDAN_CODE` (Claude Code) или адрес `https://fundan.cc/mcp/<ваш код>` (веб/десктоп).

Only open programs are shown. Data is checked against donors' official pages; always confirm on the official link before applying.
