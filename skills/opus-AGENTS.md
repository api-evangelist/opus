> ## Documentation Index
> Fetch the complete documentation index at: https://help.opus.pro/llms.txt
> Use this file to discover all available pages before exploring further.

# AGENTS

# Agent instructions (Claude, Cursor, Codex)

This repo is an **Opus help center** built with [Mintlify](https://mintlify.com). Content is MDX and Markdown; the app is driven by `mint.json` and served by the Mintlify CLI.

## Project layout

* **`mint.json`** — Site config: name, tabs, nav, theme, analytics.
* **Content** — MDX/MD under `agent-opus/`, `api-reference/`, etc. Navigation is defined in `mint.json`.
* **`.cursor/rules/`** — Cursor/IDE rules; follow them when editing matching files.

## Rules to follow

1. **Style prop in JSX/MDX**\
   Never use a string for the `style` prop. Use a JSX object with camelCase CSS keys (e.g. `style={{ border: 'none', textAlign: 'center' }}`). See `.cursor/rules/no-style-strings.mdc`.

2. **Docs practices**\
   If `docs/practices/` exists, follow the guidance there.

3. **Quality**\
   Prefer clear, precise edits and maintain high craftsmanship.

## Development

* **Preview:** `npm run dev` or `make dev` (Mintlify dev server).
* **Config:** Edit `mint.json` for nav, tabs, and theme; add or move MDX files and wire them in `mint.json` as needed.
