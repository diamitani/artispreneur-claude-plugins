# Artispreneur Manager

Artispreneur Manager for independent musicians: Your HQ: priorities, planning, and anything across the team. Use when an artist wants the manager to plan, draft or prioritize this kind of work. Drafts in the conversation only; it does not send, publish, file or pay for anything. Includes the desk as a Claude subagent and as a skill.

Published by Artispreneur Inc. (https://www.artispreneur.com). Version 1.1.1.

## What's inside

- The Manager as a subagent, `agents/home-base.md` (Claude Code and Cowork).
- The same desk as a skill, `home-base-desk`, for claude.ai chat.
- `.mcp.json` pointing at the public, read-only Artispreneur MCP server, whose `get_skill` tool returns any desk skill's playbook.

## What it connects to and sends

The plugin declares one remote MCP server, `https://www.artispreneur.com/mcp` (Artispreneur public MCP, version 1.2.1), over HTTPS with no sign-in. Its tools are read-only: they return public playbooks, desk starters, pricing, an EPK outline and computed release checklists. When Claude calls a tool it sends only that tool's arguments, such as a skill slug, an EPK audience or a release date. The plugin has no hooks, scripts or executables, reads no files or credentials, and stores nothing. Skills work without the server; they then run from the instructions in this folder.

Legal, tax and financial content is general information, not professional advice. Have a lawyer, accountant or other professional review anything binding before you rely on it.

## Install

In Claude Code:

```
/plugin marketplace add diamitani/artispreneur-claude-plugins
/plugin install artispreneur-home-base@artispreneur
```

On claude.ai or in Claude Desktop, upload this folder as a zip from Customize > Plugins (Add > Upload plugin), or upload a single skill zip from Customize > Skills.

## Example prompts

See the Starter section of the skill.

## Support

https://www.artispreneur.com/support · pat@artispreneur.com · Privacy: https://www.artispreneur.com/legal/privacy · Terms: https://www.artispreneur.com/legal/terms
