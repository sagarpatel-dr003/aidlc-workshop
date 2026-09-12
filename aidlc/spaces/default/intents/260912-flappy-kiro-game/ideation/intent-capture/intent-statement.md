# Intent Statement — Flappy Kiro

## Problem Statement

Flappy Kiro is a browser-based arcade game that recreates the Flappy Bird formula with a custom ghost character called Ghosty. The player needs an engaging, immediately playable game they can open in any browser without installation, demonstrate as a portfolio piece, and play repeatedly to beat their own high score. There is no existing implementation; this is a greenfield build. [desc]

## Target Customer

The primary user is the developer themselves, building a personal/portfolio project to demonstrate a working browser game. [Q3] The player interacts directly with the game: they tap the spacebar to navigate Ghosty through a series of pipe walls, aiming to survive as long as possible and set a new high score. The game is self-contained and requires no account, login, or server. [desc]

## Success Metrics

- The game runs in a modern web browser without installation. [Q1]
- Ghosty is rendered using the provided `assets/ghosty.png` sprite. [Q2]
- The player can flap (spacebar), score points by passing through wall gaps, and die by hitting a wall or the ground. [desc]
- The current score and all-time high score are visible on screen at all times. [assumption]
- The high score persists across browser sessions via `localStorage`. [Q5]
- Collision detection is accurate: a wall or ground hit ends the game. [desc] A game-over/restart state is shown after collision. [assumption]
- The `jump.wav` and `game_over.wav` audio assets play on flap and collision respectively, if audio playback is technically straightforward on the chosen stack; silence is acceptable if not. [Q6] [Q2]
- All game sprites render without visual artefacts; no placeholder rectangles remain in the final build. [Q3]

## Initiative Trigger

The developer wants to build a recognised game genre from scratch as a portfolio exercise, using existing assets already present in the repository. The finished game will be demonstrable as a portfolio piece. [Q3] [Q2]

## Initial Scope Signal

- **Workflow-selected scope:** `flappy-kiro-game` (custom, 13 of 33 stages) [scope]
- **User-confirmed product boundary:** A single-screen, single-player browser arcade game with fixed difficulty, persistent high score, and optional audio. No server, no multiplayer, no difficulty progression beyond fixed parameters. [Q1] [Q4] [Q5] [Q6]

## Assumptions & Open Questions

- [assumption] The browser target is modern desktop browsers (Chrome, Firefox, Safari, Edge) only — mobile browser touch support is not confirmed as a requirement.
- [assumption] The tech stack will be chosen by the architect during requirements analysis based on what is simplest for a browser-based arcade game (HTML5 Canvas with vanilla JavaScript/TypeScript is the most likely recommendation), since no preference was expressed. [Q7]
- [assumption] No background music asset exists in `assets/` (`ghosty.png`, `jump.wav`, `game_over.wav` only) — background music is therefore out of scope unless the developer adds an asset.
- [assumption] A start screen and game-over/restart screen are expected (the example UI implies a running game state; a restart flow is standard for this genre), but the exact UI treatment is not specified.
- [assumption] The score display format is "Score: N | High: N" shown in the status bar, as visible in the example UI screenshot.
