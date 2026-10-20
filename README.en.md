<p align="center"><img src="assets/logo.svg" width="64" alt="AI Safety HOT"></p>

<h1 align="center">AI Safety HOT Hub</h1>

<p align="center"><b>Follow AI safety news, papers and incidents. Explore the website, or bring it to your agent.</b></p>

<p align="center">
  <a href="https://aisafetyhot.com/en"><img src="https://img.shields.io/badge/Website-aisafetyhot.com-e4572e" alt="Website"></a>
  <a href="docs/agent.md"><img src="https://img.shields.io/badge/MCP-Streamable%20HTTP-6f42c1" alt="MCP"></a>
  <a href="#skills"><img src="https://img.shields.io/badge/Agent_skills-6-2ea44f" alt="6 Agent skills"></a>
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

Connect the MCP server and install the skills to ask about recent news, research leads, labs or incidents in plain language.

**Claude Code** · Install the skills and MCP server

```bash
/plugin marketplace add wuyoscar/AISafetyHot-Hub
/plugin install aisafetyhot@aisafetyhot-hub
```

**Codex**

```bash
npx skills add wuyoscar/AISafetyHot-Hub
codex mcp add aisafetyhot --url https://aisafetyhot.com/api/mcp
```

**Cursor / other agents** · Install supported skills with `npx skills add wuyoscar/AISafetyHot-Hub`, then add `https://aisafetyhot.com/api/mcp` as a Streamable HTTP MCP server in your client.

Recent news briefs need no API key. Historical queries and full paper readings require read authorization; see the [agent guide](docs/agent.md) for access and setup. The website is free to read.

<a id="skills"></a>

### Six skills to choose from

| Skill | Use it for | Try asking |
| --- | --- | --- |
| [`aisafety-brief`](skills/aisafety-brief/SKILL.md) | Recent safety briefings | What happened in AI safety this week? |
| [`aisafety-paper-scout`](skills/aisafety-paper-scout/SKILL.md) | Paper and citation leads | Find research on prompt injection against agents. |
| [`aisafety-related-work`](skills/aisafety-related-work/SKILL.md) | Organizing related work around a question | Use this abstract to organize related work on reward hacking. |
| [`aisafety-lab-watch`](skills/aisafety-lab-watch/SKILL.md) | Following a lab | What has Anthropic published on safety this week? |
| [`aisafety-incident-check`](skills/aisafety-incident-check/SKILL.md) | Incident and vulnerability reports | What recent security incidents involve Cursor? |
| [`aisafetyhot`](skills/aisafetyhot/SKILL.md) | MCP tools and query reference | Show the tools, filters and pagination options. |

[See query examples](docs/mcp-examples.md)

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
