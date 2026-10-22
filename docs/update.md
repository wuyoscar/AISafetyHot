# Update AI Safety HOT

You are an AI agent. The user asked you to update AI Safety HOT. The MCP server itself needs no update (it runs at https://aisafetyhot.com/api/mcp); update the skills.

## Claude Code

```bash
claude plugin marketplace update aisafetyhot-hub
claude plugin update aisafetyhot@aisafetyhot-hub
```

## Codex and other clients using `npx skills`

```bash
npx skills update
npx skills add wuyoscar/AISafetyHot-Hub
```

Version 1.1 (2026-10) has four skills: `aisafety-hot`, `aisafety-brief`, `aisafety-paper-scout`, `aisafety-watch`. Remove the retired ones if they are still installed:

```bash
npx skills remove aisafety-related-work aisafety-lab-watch aisafety-incident-check aisafetyhot
```

(`aisafety-related-work` is now part of `aisafety-paper-scout`; `aisafety-lab-watch` and `aisafety-incident-check` are now `aisafety-watch`.)

## Check and tell the user

Run the check in [install.md](install.md#3-check-that-it-answers), then tell the user which version and skills are installed now.

## Uninstall

- Claude Code: `claude plugin uninstall aisafetyhot@aisafetyhot-hub` (MCP only: `claude mcp remove aisafetyhot`)
- Codex: `codex mcp remove aisafetyhot` and `npx skills remove aisafety-hot aisafety-brief aisafety-paper-scout aisafety-watch`
- Other clients: delete the `aisafetyhot` entry from the MCP settings and remove the skills as above.
