# Euchre

A high-fidelity, responsive Euchre Single Page Application (SPA) designed for seamless play across mobile and desktop browsers. This project emphasizes a "single-file" philosophy, packing a rich gaming experience into a portable and high-performance HTML file.

## 🃏 Project Overview

This repository contains a complete Euchre engine featuring autonomous AI opponents, fluid animations, and a dynamic UI. By utilizing modern CSS features like Grid, Flexbox, and `clamp()`, the game provides a "felt-table" experience that scales perfectly to any screen size.

### Key Features
* **Single-File Architecture:** The entire game—HTML, CSS, and JavaScript—lives in `euchre.html`.
* **Fluid Responsive Design:** Uses CSS variables and relative units to ensure the game is playable on everything from small smartphones to large monitors.
* **Smart AI Opponents:** Built-in logic for bidding, trick-taking, and strategy.
* **Immersive Game-Feel:** Custom keyframe animations for dealing, trump selection, and scoring, complemented by synthesized sound effects.
* **Visual Themes:** Toggle between various aesthetics including Classic, Vintage, Art Deco, and Neon.

## 🛠 Tech Stack
* **Language:** Vanilla JavaScript (ES6+)
* **Styling:** Modern CSS3 (Grid, Flexbox, Variables)
* **Automation:** GitHub Actions + Claude Code for autonomous issue resolution.

## 🚀 Getting Started

Because this is a single-page application, getting started is as simple as possible:

1.  Clone the repository:
    ```bash
    git clone [https://github.com/](https://github.com/griffore/euchre.git
    ```
2.  Open `euchre.html` in any modern web browser.

No build steps, compilers, or server-side dependencies are required.

## 🤖 Development with Claude Code

This repository is optimized for autonomous development. When using **Claude Code** to fix issues or add features:
* Refer to `CLAUDE.md` for project-specific coding standards and state management patterns.
* The automated GitHub workflow is configured to trigger on issues labeled `fix-with-claude`.

## 📜 License

This project is licensed under the **MIT License** — providing you the freedom to use, modify, and distribute the code while protecting the original authors from liability.
