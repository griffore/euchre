# CLAUDE.md — Euchre

## Project Overview
This project is a high-performance, responsive Single Page Application (SPA) for the game of Euchre. It is intentionally contained within a single `euchre.html` file to simplify portability and deployment.

## Coding Standards
* **Single File Architecture:** All HTML, CSS, and JavaScript must remain within `euchre.html`. Do not create external `.js` or `.css` files.
* **CSS Architecture:**
    * Maintain the `:root` theme variables for all colors, spacing, and card dimensions.
    * Use `clamp()` for fluid typography and element sizing to ensure responsiveness from 320px to 4k resolutions.
    * New animations should follow the naming convention of existing keyframes (e.g., `card-deal-fly`, `trump-pop`).
* **JavaScript Patterns:**
    * **State Management:** All game state resides in a global `G` object (e.g., `G.upCard`, `G.phase`, `G.dealer`, `G.hands`).
    * **Rendering:** Use the central `render()` function to update the DOM based on state changes. Avoid manual DOM manipulation outside of the render cycle unless handling temporary overlays.
    * **Animations:** Coordinate game-feel animations using `setTimeout` and CSS classes within the core logic functions (e.g., `_dealCore`).

## Technical Specifics
* **Table Layout:** The table uses a CSS Grid layout (grid-areas: `top`, `center`, `bottom`, `left`, `right`, `log`). Ensure any new UI elements are assigned to the correct grid-area.
* **Game Phases:** Logic updates should strictly check `G.phase` (e.g., `dealing`, `bidding`, `playing`, `discarding`) before executing actions to prevent state desync.
* **SFX Engine:** Sound effects are handled via the `SFX` object. Use `SFX.play(frequency, type, duration)` for synthesized tones rather than external audio files.

## Development Workflow
* **Testing:** Test for responsiveness by resizing the browser window. The UI must remain functional at a minimum width of 320px.
* **Performance:** Prioritize CSS transitions for animations. Keep JavaScript logic synchronous where possible to avoid race conditions in the game loop.
