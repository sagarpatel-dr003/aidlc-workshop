## Sources

- [desc] Initial description: "I want to build a Flappy Bird clone called Flappy Kiro. Flappy Kiro is an arcade-style game in which the player controls a ghost called Ghosty, which moves persistently to the right. They are tasked with navigating Ghosty through a series of walls that have equally sized gaps placed at random heights. Ghosty automatically descends and only ascends when the player taps the spacebar. Each successful pass through a pair of walls awards the player one point. Colliding with a wall or the ground ends the gameplay."
- [scope] Workflow-selected scope: `flappy-kiro-game`.

---

## Q1. What platform(s) should Flappy Kiro target?

The initial description doesn't specify where the game should run. This affects the tech stack choice for the entire build.

A. Browser-based (runs in a web browser, no install needed — HTML5/Canvas or a JS game library)
B. Desktop application (native Windows/macOS/Linux app — e.g. Electron, Tauri, or a native framework)
C. Mobile app (iOS and/or Android — e.g. React Native, Flutter, or native)
D. Multiple platforms simultaneously (please specify which in X)
E. No preference — choose what's simplest for a solo build
X. Other (please specify)

[Answer]: A. Browser-based

---

## Q2. Are the game assets in the `assets/` folder intended to be used, or are they reference/example material?

The README mentions `assets/` (audio and sprites) and there is an example UI screenshot. This determines whether we build around what's there or design freely.

A. Yes — use those sprites and audio files as-is in the game
B. Partially — use some assets but we may need to create or replace others
C. They are reference/inspiration only — we will create or source different assets
D. Not yet decided — assess what's there and recommend
E. Not applicable — generate/use placeholder assets for now
X. Other (please specify)

[Answer]: A. Yes — use those sprites and audio files as-is in the game

---

## Q3. Who is the intended player, and what is the primary goal for this game?

Understanding the audience shapes decisions about difficulty, polish, and what "done" looks like.

A. Personal/portfolio project — it's for me or to demonstrate a working game; functional is sufficient
B. Friends/small group — playable and fun for a small audience; some polish expected
C. Public release — intended for general players; needs to be polished and enjoyable to strangers
D. Workshop/learning — the main goal is the learning experience of building it, not the game itself
E. Not yet defined
X. Other (please specify)

[Answer]: A. Personal/portfolio project

---

## Q4. What does the difficulty curve look like over time?

The description specifies random gap heights but doesn't say whether the game gets harder as the score increases.

A. Fixed difficulty — wall gap size and scroll speed stay constant throughout the game
B. Gradual ramp — walls come faster and/or gaps shrink as the score increases
C. Level-based — distinct difficulty tiers are introduced at score thresholds (e.g. every 10 points)
D. Not yet decided — go with the Flappy Bird standard (slow ramp)
E. Not applicable — keep it simple, fixed difficulty is fine
X. Other (please specify)

[Answer]: A. Fixed difficulty

---

## Q5. Should the game keep track of a high score between sessions?

This affects whether any persistence (local storage, file) is needed.

A. Yes — persist the all-time high score across browser sessions / app restarts
B. In-session only — track best score during the current session, reset on close
C. No score persistence needed — score display during play is sufficient
D. Not yet decided
X. Other (please specify)

[Answer]: A. Yes — persist the all-time high score across browser sessions via local storage

---

## Q6. Are there any audio requirements?

The `assets/` folder appears to contain audio files. Clarifying whether sound is in scope affects the build significantly.

A. Yes — sound effects for flap, score, collision, and/or background music are required
B. Optional — implement audio if it's straightforward; silence is acceptable otherwise
C. No audio — the game should be silent (or muted by default with no sound effects implemented)
D. Not yet decided — assess what audio assets exist and recommend
X. Other (please specify)

[Answer]: B. Optional — implement audio if it's straightforward; silence is acceptable otherwise

---

## Q7. Is there a specific technology preference or constraint for the implementation?

The architect perspective needs this to make informed decisions in later stages.

A. No preference — choose the simplest/most appropriate tech for the target platform
B. JavaScript / TypeScript (vanilla or with a specific library — please name it in X if specific)
C. Python (e.g. Pygame)
D. A specific game engine (e.g. Godot, Unity, Phaser) — please specify in X
E. Must use only what's already in this repository (no new dependencies)
X. Other (please specify)

[Answer]: A. No preference — choose the simplest/most appropriate tech for the target platform

---

## Consolidated Summary Confirmation

<!-- Filled after all questions answered -->

- Looks correct
- Request changes

[Answer]: Looks correct
