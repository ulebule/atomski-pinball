# ATOMSKI PINBALL

A retro pinball table in the browser, modelled on **Atari Video Pinball
(1980)**. Everything sits in a single `index.html` — no libraries, no
build step, no network calls. Double-click it and play.

**[▶ Play it here](https://ulebule.github.io/atomski-pinball/)**

## Play

Open `index.html` in a browser, or visit the published page on GitHub
Pages.

## Controls

| Key | Action |
|---|---|
| `◀` `▶` | left / right flipper |
| `▼` or `Space` | pull back and launch the ball |
| `Z` / `X` | nudge (a shove against the table) |
| `Enter` | start / new game |
| `M` | sound on / off |

On a touch screen the left and right thirds of the screen are the
flippers, the bottom middle is the plunger, and the `↯` button in the top
right is the nudge.

## The table

- **three round bumpers** — 100 points
- **Atari diamond** in the middle — 500 points; four hits award an
  **extra ball**
- **A-T-A-R-I** rollovers along the top — 300 points each, and lighting
  all five scores **5000 points** and raises the multiplier (up to x5)
- **spinner** on the left edge — 10 points per revolution
- **slingshots** above the flippers — 50 points
- **tilt**: three nudges in a row lock the flippers until the ball drains

Three balls per game. The hi-score and the top-ten table are stored
locally in the browser (`localStorage`) — tied to that device and
browser.

## Languages

The interface detects the device language; the button in the top left
cycles through Slovenian, English, German, Italian and French.

## Install it

The game is a PWA: a browser will offer to add it to the home screen (on iOS,
Share → *Add to Home Screen*), and it then opens standalone, without browser
chrome. A service worker caches `index.html`, the manifest and the icons, so
after the first visit the game **runs with no connection at all**.

The worker only touches same-origin requests, and the cache key is prefixed
with the repo name — the other games published under `ulebule.github.io` keep
their own caches instead of evicting each other.
