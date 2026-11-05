# Ant Colony — Store Submission Materials

## Short description (CrazyGames / GameDistribution / itch.io)

Dig an underground ant empire: tunnel to the surface, haul food home, grow
the brood, and defend the queen from antlions and spiders. Survive 10 minutes.

(154 characters)

## Details

- Genre: Strategy / Simulation / Casual
- Controls: Mouse or touch. Tap dirt to dig (2 workers per order), tap food to
  forage, tap pits to send a soldier. Bottom bar: build rooms, train/station
  soldiers, backfill tunnels. In-game buttons: sound mute, 1x/2x speed, menu.
- Features:
  - Side-view underground cross-section on a 20x14 soil grid (dig, backfill,
    rock, rooms).
  - 3 procedurally generated maps (soil bands, rock density, threat rhythm),
    validated so the queen chamber can always dig through to the surface.
  - Room building on dug 2x2 spaces: Nursery (+50% egg speed, max 2), Store
    (+30 food cap), Barracks (unlocks soldiers).
  - Two ant castes: workers (dig / haul) and soldiers (station / fight);
    the queen lays workers, eats food, and must stay alive.
  - Threat system every ~60s: antlion funnel pits trap surface foragers,
    spiders invade through entrances and fight soldiers on contact.
  - Economy pressure: every ant eats 1 food per 30 seconds; storage caps
    force room planning.
  - Win by surviving 10 minutes with 10+ ants and a living queen; score from
    colony size, food gathered and rooms. Per-map best scores saved locally.
  - 1x/2x speed toggle, mute, pause menu, dig/backfill cell state machine,
    BFS tunnel pathfinding with the surface as a travel layer.
- All graphics are procedural Canvas 2D; all audio is synthesized WebAudio.
- Tech: single-file HTML5, vanilla JavaScript, zero external assets, no
  tracking, no external links. Works offline once loaded.

## Tags

ant, colony, strategy, simulation, dig, tunnel, queen, defense, builder,
casual, single-file, pixel

## CrazyGames submission checklist
- [x] Self-contained index.html (SDK loads only on crazygames domains)
- [x] gameplayStart / gameplayStop / loadingStart / loadingStop / happytime events wired
- [x] Responsive (letterboxed canvas scales to any viewport, touch friendly)
- [x] No external links inside gameplay, no analytics
- [ ] Cover: cover-16x9.png (1280x720)
- [ ] Screenshots: 1280x800

## GameDistribution
- Upload ant-colony-gd.zip (contains only index.html).
- The GameDistribution SDK loader activates automatically on gamedistribution /
  gd.games domains; gameplayStart/Stop are wired for CrazyGames and the GD SDK
  picks up its own lifecycle.

## itch.io
- Upload ant-colony-itch.zip, mark "This file is playable in browser",
  entry file: index.html, viewport: 960x584 (letterboxed, any orientation
  works), kind: html.
- Pricing: $0 (donations optional).
- Suggested caption: "Dig. Haul. Defend the queen."
