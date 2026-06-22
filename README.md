# Zillion

Building **local-first developer tools** for AI assistants.

**Current focus**: giving LLM assistants (Claude Desktop, Claude Code, Cursor, Windsurf, Cline) deep code intelligence on your repos — without uploading anything to the cloud.

## What I'm shipping

- **[jarvis-graph-mcp](https://github.com/Zilli-on/jarvis-graph-mcp)** — Model Context Protocol server exposing 18 Python code-analysis tools to any MCP client. Refactor priority, coverage gaps, test skeleton generation, dead code, import cycles, risk-ranked TODO scan, full repo health reports. Designed for any MCP client; smoke-tested in-process via FastMCP.

- **[jarvis-graph-lite](https://github.com/Zilli-on/jarvis-graph-lite)** — The stdlib-only Python code index that powers it. Zero pip dependencies, 277 passing tests, local sqlite index, dogfooded on itself.

## Demo

- **[Tiny Planet](demo/planet.html)** — an endless **galaxy of project worlds** you explore Super-Mario-Galaxy style. Each planet is a project node; hold the jump key to leap through space and get pulled onto the next world. Single self-contained HTML file (WebGL + Three.js). Inspired by `messenger.abeto.co`.
  - 🪐 **Galaxy mode**: charge-jump with gravity flight + trajectory aim-preview between procedurally generated planets; an "infinite" cluster that grows as you explore (jump into the void to discover new worlds) with Minecraft-style distance culling
  - 🧠 **Living data-brain**: worlds are linked like synapses with travelling data-pulses — connections between projects in the same language run warmer and busier, and every delivery sends a ripple through the whole network; a **brain map** (M) lets you tap any project world to fly there. Each world is a project — press **E** to open a panel with the live GitHub README
  - 🎞️ **Cinematic grade**: full post pipeline — bloom, volumetric god rays toward the sun, plus a film grade (filmic contrast, teal/orange split-tone, subtle chromatic aberration, vignette and animated grain)
  - 🎨 Per-theme worlds (grass / desert / snow / volcano / tech) with their own flora, wildlife (penguins, lizards, hover-drones…), ambient FX (lava, snowfall, holograms), atmosphere halos, rings and sky tint; toon shading, bloom, day/night cycle, shooting stars, depth fog
  - 🤖 Custom **procedural avatar** — a "data courier" explorer (glowing visor + pulsing antenna node) built entirely from primitives with hand-coded animation: walk/run cycle, tucked flight pose, charge crouch, squash-&-stretch (no external model, so nothing to fail to load); pick-up & delivery loop with per-world goals, combo pops, compass, radar, timer, best score; procedural ambient **music** + SFX
  - 🎬 **Showreel** (auto-fly attract mode) and 📷 **photo mode** (C) for clean shots; first-time onboarding; dynamic top-down camera that tilts while aiming a jump
  - 💎 Glassmorphic UI (Outfit / Space Grotesk); works on desktop **and** phone. Controls: `W/S` walk · `A/D` turn · `Shift` run · **hold `Space`** planet-jump · `M` map · `E` project · `C` photo
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
