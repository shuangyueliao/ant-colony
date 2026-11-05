# Ant Colony

A free, original single-file HTML5 strategy game. You run an underground ant
colony: dig tunnels, build rooms, haul food home and defend the queen from
antlions and spiders.

**Play:** open `index.html` in any modern browser (or visit the GitHub Pages
URL). Desktop mouse + keyboard and mobile touch are both supported.

## How to play

- Tap dirt next to a tunnel to send 2 workers digging (deeper = slower).
- Tap glowing food on the surface — workers haul it home (beware predators).
- Build rooms on dug 2x2 spaces:
  - **Nursery** (30 food) — ant production speed +50%, max 2.
  - **Store** (20 food) — +30 food storage.
  - **Barracks** (15 food) — unlocks soldier training (10 food each).
- Every ~60 seconds a predator strikes: **antlions** dig trapping pits on the
  surface, **spiders** invade through tunnel entrances. Station soldiers
  (Post), attack pits with a soldier, or **backfill** tunnels (Fill) to seal
  them out — at the cost of your food line.
- Every ant eats 1 food every 30 seconds. Grow wisely.
- **Win:** survive 10 minutes with 10+ ants and a living queen.

## Features

- 3 procedurally generated maps with different soil, threat pacing and rock.
- Seeded RNG, BFS tunnel pathfinding (including the surface as a travel layer),
  cell state machine for dig / backfill, predator AI with mutual combat.
- All graphics are procedural Canvas, all audio is synthesized WebAudio.
- Single file, zero external assets, no tracking, works offline once loaded.
- 1x / 2x speed toggle, mute button, per-map best scores in localStorage.

## Tech

Vanilla JavaScript, Canvas 2D, WebAudio. No frameworks, no build step.
The platform SDK (CrazyGames / GameDistribution) is only loaded when the page
is served from those domains; everywhere else it runs fully standalone.
