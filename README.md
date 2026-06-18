# Zillion

Building **local-first developer tools** for AI assistants.

**Current focus**: giving LLM assistants (Claude Desktop, Claude Code, Cursor, Windsurf, Cline) deep code intelligence on your repos — without uploading anything to the cloud.

## What I'm shipping

- **[jarvis-graph-mcp](https://github.com/Zilli-on/jarvis-graph-mcp)** — Model Context Protocol server exposing 18 Python code-analysis tools to any MCP client. Refactor priority, coverage gaps, test skeleton generation, dead code, import cycles, risk-ranked TODO scan, full repo health reports. Designed for any MCP client; smoke-tested in-process via FastMCP.

- **[jarvis-graph-lite](https://github.com/Zilli-on/jarvis-graph-lite)** — The stdlib-only Python code index that powers it. Zero pip dependencies, 277 passing tests, local sqlite index, dogfooded on itself.

## Demo

- **[Walkable 3D World](demo/index.html)** — a small first-person 3D world you can walk around, right in the browser. WebGL + Three.js, single file, no install, no build. Open `demo/index.html` (or serve it locally) and click **Welt betreten**. Controls: `WASD` move · mouse look · `Shift` sprint · `Space` jump · `Esc` pause.

## Philosophy

- **Local-first**: your source never leaves your machine
- **Stdlib only** where possible: fewer pip installs = fewer ways to break
- **Honest READMEs**: nothing in my project descriptions that I can't demonstrate or reproduce
- **Dogfood everything**: if my tool can't analyze its own source cleanly, it's not ready

## Stack

Python 3.11+ · Model Context Protocol · stdlib · sqlite · ast

## Also

I also take on AI automation contracts (Telegram bots, content pipelines, workflow automation, self-healing agent systems). See **[jarvis-portfolio](https://github.com/Zilli-on/jarvis-portfolio)** for the services page, or open an issue on any of my repos.

## Contact

Issues on any of my repos are the fastest way to reach me.
