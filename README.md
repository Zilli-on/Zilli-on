# Zillion

Building **local-first developer tools** for AI assistants.

**Current focus**: giving LLM assistants (Claude Desktop, Claude Code, Cursor, Windsurf, Cline) deep code intelligence on your repos — without uploading anything to the cloud.

## What I'm shipping

- **[jarvis-graph-mcp](https://github.com/Zilli-on/jarvis-graph-mcp)** — Model Context Protocol server exposing 18 Python code-analysis tools to any MCP client. Refactor priority, coverage gaps, test skeleton generation, dead code, import cycles, risk-ranked TODO scan, full repo health reports. Designed for any MCP client; smoke-tested in-process via FastMCP.

- **[jarvis-graph-lite](https://github.com/Zilli-on/jarvis-graph-lite)** — The stdlib-only Python code index that powers it. Zero pip dependencies, 277 passing tests, local sqlite index, dogfooded on itself.

## Demo

- **[Tiny Planet](demo/planet.html)** — an endless **galaxy of project worlds** you explore Super-Mario-Galaxy style. Each planet is a project node; hold the jump key to leap through space and get pulled onto the next world. Single self-contained HTML file (WebGL + Three.js). Inspired by `messenger.abeto.co`.
  - 🪐 **Galaxy mode**: gravity flight between procedurally generated planets, an "infinite" cluster that grows as you explore (Minecraft-style distance culling)
  - 🧠 **Data-brain**: worlds are linked like synapses with travelling data-pulses; a **brain map** (M) lets you tap any project world to travel there
  - 🎨 Per-theme worlds (grass / desert / snow / volcano / tech) with their own ambient FX, atmosphere halos and rings; toon shading, bloom, day/night cycle, shooting stars
  - 🤖 Rigged glTF hero with idle/walk/run; pick-up & delivery loop, compass, radar, timer, best score; procedural ambient audio + SFX
  - 💎 Glassmorphic UI (Outfit / Space Grotesk); works on desktop **and** phone. Controls: `W/S` walk · `A/D` turn · `Shift` run · **hold `Space`** planet-jump · `M` map
- **[Walkable 3D World](demo/index.html)** — a first-person tech-city you can walk around. `WASD` move · mouse look · `Shift` sprint · `Space` jump, plus touch controls on mobile.

Both are single self-contained HTML files (Three.js via CDN) — open them locally, or use a render link since GitHub shows `.html` as source rather than running it.

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
