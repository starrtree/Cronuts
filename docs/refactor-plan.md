# Cronuts multi-file refactor plan

This repository currently runs primarily from a single `index.html` file with inline HTML, CSS, and JavaScript.

Target structure:

```txt
index.html
css/styles.css
js/main.js
js/state.js
js/levels.js
js/player.js
js/rendering.js
js/controls.js
js/particles.js
js/ui.js
```

Recommended migration phases:

1. Extract the inline `<style>` block into `css/styles.css`.
2. Extract the inline `<script>` block into `js/main.js` without changing behavior.
3. Move level definitions into `js/levels.js`.
4. Move global game/player state into `js/state.js`.
5. Move controls, particles, UI, rendering, and player logic into their own modules.
6. After the game works unchanged, merge Level 12 content into `levels.js`.

This plan is intentionally staged to avoid breaking the playable build.
