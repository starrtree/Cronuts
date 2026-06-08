# Cronuts JavaScript Refactor Targets

The current game logic lives inside the inline `<script>` block in `index.html`.

Planned modules:

- `main.js` — bootstrapping and game loop
- `state.js` — shared game/player state
- `levels.js` — level definitions and maps
- `player.js` — player movement and animation
- `rendering.js` — canvas drawing helpers
- `controls.js` — keyboard, joystick, and mobile controls
- `particles.js` — particle and floating text systems
- `ui.js` — HUD, menus, level intro, pause, and end screen

Do the extraction in stages and test after each step.
