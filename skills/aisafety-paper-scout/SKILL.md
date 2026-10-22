---
name: aisafety-paper-scout
description: Find AI safety papers on a direction (jailbreaks, prompt injection, agent security, backdoors, reward hacking, interpretability, evals, AI control, privacy...) from the AI Safety HOT paper library, with one-line takeaways and BibTeX. Use when the user asks for today's new papers, papers or a reading list on an AI safety topic, or a related-work section with citations for their own paper or idea.
---

# AI Safety paper scout

Data, no key needed:
- Paper index by direction: `https://raw.githubusercontent.com/wuyoscar/AISafetyHot-Hub/main/daily-papers/topics/<slug>.json` — every paper pushed so far under that direction: `title`, `titleZh`, `line` (what the paper does, one line), `topics`, `venue` (arXiv id or conference), `date`, `url`, `site`, `authors`.
- Daily lists: `https://raw.githubusercontent.com/wuyoscar/AISafetyHot-Hub/main/daily-papers/<year>/<YYYY-MM-DD>.json`.
- Direction slugs and definitions: MCP `aisafetyhot_get_topics`.
- This week's newest picks: MCP `aisafetyhot_get_latest` (`window: "7d"`) → `paperPicks`.

Steps:
1. Map the user's request to 1–3 slugs with `aisafetyhot_get_topics` (e.g. "prompt injection" → `prompt-injection`, "jailbreak" → `jailbreak`).
2. Fetch each slug's JSON; merge, drop duplicates by `id`; add `paperPicks` that match.
3. Rank: what the user asked for first, then newer first; keep up to 15 unless asked for more.
4. Output a table: title (linked), one line on what it does (from `line`), venue, date. Offer the AI Safety HOT reading link (`site`) when present.
5. If asked for citations, emit BibTeX: for `arXiv <id>` use `@misc{<firstword><year>, title={...}, eprint={<id>}, archivePrefix={arXiv}, url={https://arxiv.org/abs/<id>}}`; for conference papers use `@inproceedings` with the venue and year and the `url`. Use `authors` from the index for `author = {A and B and ...}`; never invent authors.

**Related work.** When the user gives a title, abstract or idea: list its 2–4 core ideas, map each to slugs, keep papers whose `title` or `line` matches, group them into 2–4 lines of work (one paragraph each: what the line does, the papers as [n], how the user's work differs — only from what the user said), then the numbered references and BibTeX. Say "per the paper's one-line summary" where you only have `line`, and tell the user which directions had few matches.

**Today's papers.** For "what's new today", read the newest `daily-papers/<year>/<YYYY-MM-DD>.json` and list its papers with their `line`.

The index grows by 30 hand-picked papers a day (well-known authors, top labs, strong groups); each entry also lists `authors`; the full library and readings are at https://aisafetyhot.com/zh/papers.
