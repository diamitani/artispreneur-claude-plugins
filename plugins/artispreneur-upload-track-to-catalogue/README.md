# Artispreneur Catalog Upload

Catalog Upload for independent musicians: Build one complete catalog record per track: metadata, credits, splits, rights and registration status. Draft-first Artispreneur skill; nothing is filed, sent, published or paid.

Published by Artispreneur Inc. (https://www.artispreneur.com). Version 1.1.1.

## What's inside

- One skill, `upload-track-to-catalogue`, run as `/artispreneur-upload-track-to-catalogue:upload-track-to-catalogue` or loaded when the conversation matches its description.
- `.mcp.json` pointing at the public, read-only Artispreneur MCP server.

## What it connects to and sends

The plugin declares one remote MCP server, `https://www.artispreneur.com/mcp` (Artispreneur public MCP, version 1.2.1), over HTTPS with no sign-in. Its tools are read-only: they return public playbooks, desk starters, pricing, an EPK outline and computed release checklists. When Claude calls a tool it sends only that tool's arguments, such as a skill slug, an EPK audience or a release date. The plugin has no hooks, scripts or executables, reads no files or credentials, and stores nothing. Skills work without the server; they then run from the instructions in this folder.

Legal, tax and financial content is general information, not professional advice. Have a lawyer, accountant or other professional review anything binding before you rely on it.

## Install

In Claude Code:

```
/plugin marketplace add diamitani/artispreneur-claude-plugins
/plugin install artispreneur-upload-track-to-catalogue@artispreneur
```

On claude.ai or in Claude Desktop, upload this folder as a zip from Customize > Plugins (Add > Upload plugin), or upload a single skill zip from Customize > Skills.

## Example prompts

See the Starter section of the skill.

## Support

https://www.artispreneur.com/support · pat@artispreneur.com · Privacy: https://www.artispreneur.com/legal/privacy · Terms: https://www.artispreneur.com/legal/terms
