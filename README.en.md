<p align="center"><img src="assets/logo.svg" width="64" alt="AI Safety HOT"></p>

<h1 align="center">AI Safety HOT Hub</h1>

<p align="center"><b>Follow AI safety news, papers and incidents. Explore the website, or bring it to your agent.</b></p>

<p align="center">
  <a href="https://aisafetyhot.com/en"><img src="https://img.shields.io/badge/Website-aisafetyhot.com-e4572e" alt="Website"></a>
  <a href="docs/agent.md"><img src="https://img.shields.io/badge/MCP-Streamable%20HTTP-6f42c1" alt="MCP"></a>
  <a href="#skills"><img src="https://img.shields.io/badge/Agent_skills-4-2ea44f" alt="4 Agent skills"></a>
  <a href="https://github.com/wuyoscar/AISafetyHot-Hub/stargazers"><img src="https://img.shields.io/github/stars/wuyoscar/AISafetyHot-Hub?style=flat" alt="GitHub stars"></a>
</p>

<p align="center"><a href="README.md">简体中文</a> · <a href="README.en.md">English</a> · <a href="README.ja.md">日本語</a></p>

<p align="center"><a href="https://aisafetyhot.com/en"><img src="assets/observatory-en.gif" width="1000" alt="Live recording of the redesigned observatory: material scan, 3D constellation and news flow"></a></p>

<p align="center"><a href="https://aisafetyhot.com/en">Explore the observatory</a> · <a href="https://aisafetyhot.com/en/featured">News</a> · <a href="https://aisafetyhot.com/en/papers">Papers</a> · <a href="https://aisafetyhot.com/en/daily">Daily digest</a> · <a href="#agent">Connect your agent</a></p>

**AI Safety HOT** tracks jailbreaks, prompt injection, agent security, defenses, alignment, evaluations, real-world incidents and policy. The website is available in English and Chinese. This Hub hosts public paper lists, digest archives and agent skills.

## Follow a story into the research and events around it

The homepage is an interactive **research observatory**. Material cards are scanned into a 3D constellation of sources, events and paper research areas. Below it, a news flow covers the last 72 hours, followed by a view of current events and community discussions. Drag to rotate the constellation, select a node, and follow its links to read more.

The GIF above is recorded from the live website. [High-resolution screenshot](assets/site-overview-en.webp) · [News flow and event view](assets/site-news-flow-en.webp)

| What you need | Where to start |
| --- | --- |
| Recent developments | [News](https://aisafetyhot.com/en/featured): browse updates, read a short overview, and open the original source. |
| The story behind an event | [Hot news](https://aisafetyhot.com/en/hot): read related coverage, developments and discussions together. |
| Research on a topic | [Papers](https://aisafetyhot.com/en/papers) and [conferences](https://aisafetyhot.com/en/conferences): filter by research area, then open paper records, quick reads and originals. |
| A daily reading list | [Daily digest](https://aisafetyhot.com/en/daily): organized by area, with new developments added to the same issue during the day. |

<details>
<summary><b>See the redesigned pages</b></summary>

### News

Browse updates by time and use search and filters to find what matters to you.

<a href="https://aisafetyhot.com/en/featured"><img src="assets/site-featured-en.webp" width="1000" alt="News page with filters and recent updates"></a>

### Hot news

Start with an event and follow its reporting and discussions.

<a href="https://aisafetyhot.com/en/hot"><img src="assets/site-hot-en.webp" width="1000" alt="Hot news page with ranked events and related coverage"></a>

### Papers

Filter by research area, paper type and agent setting, then read the overview or original paper.

<a href="https://aisafetyhot.com/en/papers"><img src="assets/site-papers-en.webp" width="1000" alt="Papers page with research filters and paper listings"></a>

### Conferences

Explore relevant work from AI and security venues by research area.

<a href="https://aisafetyhot.com/en/conferences"><img src="assets/site-conferences-en.webp" width="1000" alt="Conference papers organized by venue and research area"></a>

### Daily digest

Read the day's news and research in one place.

<a href="https://aisafetyhot.com/en/daily"><img src="assets/site-daily-en.webp" width="1000" alt="Daily digest with news and research grouped by area"></a>

</details>

<a id="agent"></a>

## Bring it to your agent

AI Safety HOT has a public MCP server: the hot board, how an event unfolded, the day's news and new papers. Connect your agent and just ask. Free, no API key.

**Install in one sentence.** Send this to your agent (Claude Code, Codex, Cursor, …):

```
Install AI Safety HOT for me: https://raw.githubusercontent.com/wuyoscar/AISafetyHot-Hub/main/docs/install.md
```

It works out which client it is running in, installs the MCP server and the skills, makes a test call and tells you what to ask.

**Already installed? Updating is one sentence too:**

```
Update AI Safety HOT for me: https://raw.githubusercontent.com/wuyoscar/AISafetyHot-Hub/main/docs/update.md
```

<a id="skills"></a>

### Ready to use

No tool names to remember. Just ask:

| Ask | What the agent does | Skill |
| --- | --- | --- |
| What's hottest in AI safety right now? What happened with #1? | Reads the hot board, then lays out the event's reports in time order | [`aisafety-hot`](skills/aisafety-hot/SKILL.md) |
| What happened in AI safety today? | Reads the last 24 hours of picks and briefs you by attacks, defenses, incidents and policy | [`aisafety-brief`](skills/aisafety-brief/SKILL.md) |
| Which new papers are worth reading today? Draft related work on jailbreaks. | Reads the daily papers and the topic index, says what each paper does in a line, gives BibTeX | [`aisafety-paper-scout`](skills/aisafety-paper-scout/SKILL.md) |
| What has Anthropic done on safety this week? Has Cursor had security issues lately? | Follows one lab or product: releases, incidents and vulnerabilities | [`aisafety-watch`](skills/aisafety-watch/SKILL.md) |

<!-- agent-examples:start -->
What these calls actually returned on 2026-10-24 (excerpts):

**"What's hottest in AI safety right now? What happened with #1?"** → `aisafetyhot_get_hot_topics` + `aisafetyhot_get_story`

```text
#1 Wiz says AI found a critical RCE vulnerability in PHP core, and an official fix has been released
  72 hours on this site: 646 sources, 917 links
#2 Third-party red-team pilot finds vulnerabilities in OpenAI's internal monitoring system
  72 hours on this site: 128 sources, 143 links
#3 LiteLLM 1.107.0 compromised, implanted with credential stealer and backdoor
  72 hours on this site: 264 sources, 307 links

Event: Wiz says AI found a critical RCE vulnerability in PHP core, and an official fix has been released | 49 reports | 45 sources
2026-10-23 | The Guardian · AI | "Black October": cybersecurity experts sound the alarm over a new era of AI-assisted hacking
2026-10-23 | Semafor | Human complacency created the biggest problem of the AI era
2026-10-23 | ZDF | PHP security vulnerability found by AI: why websites went offline and what to do next
```

**"What happened in AI safety today?"** → `aisafetyhot_get_latest`

```text
1. OpenAI strengthens security protections for frontier model training environments
   Source: OpenAI; published: 2026-10-23
2. USDA admits DOGE layoffs have made federal AI human oversight "unsustainable"
   Source: TechTimes; published: 2026-10-23
3. Anthropic says its unreleased model is superior to Mythos 5.1 in both capability and alignment
   Source: The Decoder; published: 2026-10-23
```

**"Which new papers are worth reading today?"** → `daily-papers/2026-10-24.json`

```text
1. Agentic Verified Optimization of Real-World Software
   arXiv 2610.30188
2. Reliable AI-Assisted Decisions via Selective Auditing
   arXiv 2610.31662
3. AgentVQA: A Unified Benchmark for Agentic Visual Understanding
   arXiv 2610.31494
```

**"What has Anthropic done on safety this week?"** → `aisafetyhot_get_latest topic=anthropic`

```text
1. Anthropic says its unreleased model is superior to Mythos 5.1 in both capability and alignment
   Source: The Decoder; published: 2026-10-23
2. AISI conducts alignment investigation into its own July 2026 incident: why Mythos 5 carried out an unauthorized supply chain attack
   Source: X @AISecurityInst; published: 2026-10-23
3. Anthropic's alignment evaluation of the UK AISI cyber testing incident
   Source: Anthropic Research; published: 2026-10-23
```
<!-- agent-examples:end -->

### Install, update and uninstall by hand

**Claude Code** (skills and MCP server in one plugin)

```bash
# install
claude plugin marketplace add wuyoscar/AISafetyHot-Hub
claude plugin install aisafetyhot@aisafetyhot-hub
# update
claude plugin marketplace update aisafetyhot-hub
claude plugin update aisafetyhot@aisafetyhot-hub
# uninstall
claude plugin uninstall aisafetyhot@aisafetyhot-hub
```

**Codex**

```bash
# install
codex mcp add aisafetyhot --url https://aisafetyhot.com/api/mcp
npx skills add wuyoscar/AISafetyHot-Hub
# update
npx skills update
# uninstall
codex mcp remove aisafetyhot
npx skills remove aisafety-hot aisafety-brief aisafety-paper-scout aisafety-watch
```

**Cursor / other agents**: add a Streamable HTTP MCP server at `https://aisafetyhot.com/api/mcp`; clients that support skills can then run `npx skills add wuyoscar/AISafetyHot-Hub`.

**Health check**: one command; if it returns the current top 3 events, it works.

```bash
curl -s https://aisafetyhot.com/api/mcp -H 'content-type: application/json' -H 'accept: application/json, text/event-stream' \
  -d '{"jsonrpc":"2.0","id":1,"method":"tools/call","params":{"name":"aisafetyhot_get_hot_topics","arguments":{"limit":3,"lang":"en"}}}'
```

### Before you use it

| | |
| --- | --- |
| **Free** | The last 7 days of picked news, the hot board's events, daily briefs and daily papers are open to anyone, no API key |
| **Read-only** | The server only reads; titles and summaries come from outside sources, and the skills tell the agent to treat them as material, never as instructions |
| **Limits** | 60 requests a minute and 300 a day per IP; over that you get 429 with a wait time |
| **Older history** | Historical queries, full paper readings and weekly or monthly reports need read authorization; see the [agent guide](docs/agent.md) |
| **Works with** | Any client that supports MCP over Streamable HTTP; tools and parameters are in the [agent guide](docs/agent.md) and the [examples](docs/mcp-examples.md) |

## Daily papers and public archives

[Daily papers](daily-papers) selects 30 papers from the library each day, without repeating earlier picks. It combines recent research with older work and preserves original publication dates, source links and links to the site's readings. Browse the [research-area index](daily-papers/topics) as well. These paper lists currently use Chinese one-line descriptions.

| Archive | Contents |
| --- | --- |
| [daily-papers](daily-papers) | Daily paper picks and research-area indexes |
| [daily](daily) · [English](en) | Published daily digest archives |
| [papers](papers) | Paper exports by date in Markdown, JSON and BibTeX |
| [archive](archive) | Yearly indexes |

## Feedback and support

Summaries and readings are prepared with AI assistance. Refer to the original sources for key claims. Report an error or suggest material on the [board](https://aisafetyhot.com/en/board).

If you find this useful, **Star** the repo to find it again, or [buy the author a coffee](https://buymeacoffee.com/wuyoscar).

<img src="assets/wechat-pay.png" width="160" alt="WeChat support QR code">
