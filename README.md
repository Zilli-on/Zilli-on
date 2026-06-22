# Zillion

Building **local-first developer tools** for AI assistants.

**Current focus**: giving LLM assistants (Claude Desktop, Claude Code, Cursor, Windsurf, Cline) deep code intelligence on your repos — without uploading anything to the cloud.

## What I'm shipping

- **[jarvis-graph-mcp](https://github.com/Zilli-on/jarvis-graph-mcp)** — Model Context Protocol server exposing 18 Python code-analysis tools to any MCP client. Refactor priority, coverage gaps, test skeleton generation, dead code, import cycles, risk-ranked TODO scan, full repo health reports. Designed for any MCP client; smoke-tested in-process via FastMCP.

- **[jarvis-graph-lite](https://github.com/Zilli-on/jarvis-graph-lite)** — The stdlib-only Python code index that powers it. Zero pip dependencies, 277 passing tests, local sqlite index, dogfooded on itself.

## Demo

- **[Tiny Planet](demo/planet.html)** — an atmospheric **action-adventure across tiny floating planets** (Zelda-style exploring × Super-Mario-Galaxy hopping × Windblown-ish island combat). Single self-contained HTML file (WebGL + Three.js). Inspired by `messenger.abeto.co`.
  - ⚔️ **Adventure loop**: land → explore → fight enemies (melee `J`, wind-blast `K`, dodge-dash `Q`) → clear/liberate the world → collect **memory fragments** that whisper a lost world's story → travel on. Occasional **guardian mini-bosses** that wind up and **dash-strike** (then leave a punish window) with their own **health bar**; 5-heart health with respawn. Combat reads fairly — foes **telegraph** an incoming hit (they puff up and flash) so the dash has a real window — with impact **hit-stop and screen-shake** for punch, and **adaptive music** that tightens when enemies close in.
  - 🪐 **Galaxy hopping**: charge-jump with gravity flight + trajectory aim-preview between procedurally generated planets; an "infinite" cluster that grows as you explore (jump into the void to discover new worlds) with Minecraft-style distance culling
  - 🧠 **Living data-brain**: worlds are linked like synapses with travelling data-pulses — connections between projects in the same language run warmer and busier, every delivery fires a bright **data packet** that travels along a real synapse to the nearest world, and the **brain map** (M) lights up each node you've reactivated (with a live "N/N nodes active" readout) and lets you tap any world to fly there. Each world is a project — press **E** to open a panel with the live GitHub README, language and ⭐ star count (shown on arrival too)
  - 🎞️ **Cinematic grade**: full post pipeline — bloom, volumetric god rays toward the sun, plus a film grade (filmic contrast, teal/orange split-tone, subtle chromatic aberration, vignette and animated grain)
  - 🎨 Per-theme worlds (grass / desert / snow / volcano / tech) with their own flora, wildlife (penguins, lizards, hover-drones…), ambient FX (lava, snowfall, holograms), atmosphere halos, rings and sky tint; toon shading, bloom, day/night cycle, shooting stars, depth fog
  - 🤖 Custom **procedural avatar** — a "data courier" explorer (glowing visor + pulsing antenna node) built entirely from primitives with hand-coded animation: walk/run cycle, tucked flight pose, charge crouch, squash-&-stretch (no external model, so nothing to fail to load); pick-up & delivery loop with per-world goals, combo pops, compass, radar, timer, best score; procedural ambient **music** + SFX
  - 📖 **Story / quest layer**: the data-brain has gone dormant — as a data courier you reactivate its synapses through a 5-stage mission (first delivery → wake a node → data stream → weave the network → awaken the brain), tracked in a live HUD panel, building to a celebratory finale; then keep exploring the endless galaxy. Collected memory fragments grow a glowing **memory garden** around the home core — a visible record of the story you've gathered
  - 🏅 **Progression that sticks**: persistent best scores plus unlockable achievements (Combo-Meister, Entdecker, Kurier, Daten-Logistiker) and a "data-brain reactivated" badge, all shown on the start menu
  - 🎬 **Showreel** + **attract mode** (auto-fly after ~30s idle, ideal as a kiosk) and 📷 **photo mode** (C) with cinematic letterbox framing for clean shots; in-game help overlay (`H` / ❔); first-time onboarding; dynamic top-down camera that tilts while aiming a jump
  - 😄 Avatar **emoji expressions** (press `F` / on-screen button; auto-pops on deliveries & landings) — a charm nod to `messenger.abeto.co`; plus a polished loading screen
  - 💎 Glassmorphic UI (Outfit / Space Grotesk); works on desktop **and** phone. Controls: `W/S` walk · `A/D` turn · `Shift` run · **hold `Space`** planet-jump · `M` map · `E` project · `C` photo · `F` emoji · `H` help
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
