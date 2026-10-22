---
name: aisafety-watch
description: Follow one AI lab, company or product on safety over the last 7 days — releases and system cards, research, incidents, vulnerabilities, jailbreaks, policy fights — from AI Safety HOT. Use when asked what OpenAI, Anthropic, Google DeepMind, Meta, xAI, DeepSeek or another lab did on safety lately, or whether a tool or model (Cursor, Claude Code, Copilot, an MCP server, an open-weight model) has had security problems recently.
---

# Watch a lab or a product

Data: the AI Safety HOT MCP server (`aisafetyhot`, https://aisafetyhot.com/api/mcp, no key needed).

1. Call `aisafetyhot_get_topics`. If the lab has a topic (group `company`, e.g. `anthropic`, `openai`), call `aisafetyhot_get_latest` with `topic: <slug>`, `window: "7d"`, `mode: "selected"`, `limit: 40`.
2. For a product or a lab without a topic, call `aisafetyhot_search` with `q: <name>`, `window: "7d"`, `mode: "selected"`, `limit: 40`; try a common alias if few results. For security questions also call `aisafetyhot_get_latest` with `category: "incident"` and keep items naming it.
3. Follow `page.nextCursor` with the same filters until `page.hasMore` is false. For an item that belongs to a bigger event, `aisafetyhot_get_story` (`public_id`, `depth: "summary"`) gives the other reports.
4. Answer newest first, grouped: releases & system cards · research · incidents & vulnerabilities · policy & governance · people & organization. One line each: date, what happened, original link. For a product's security, a table: date · what was found · affected versions as stated · fixed or not (only if the source says) · link.
5. Rules: keep claims attributed; flag items where the lab is only mentioned; say plainly when nothing turned up in 7 days — that is not proof of safety, and older history is on https://aisafetyhot.com; never reproduce exploit payloads or attack prompts.
