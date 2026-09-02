# SWV Bookie Odds — Kickform Prediction Cards

Bookmaker odds comparison prototype for TPP's Kickform match-preview pages,
implementing the `Bookie CTA` component from the Figma file
[DES-1334 — SWV — TPP Design Bookmaker Odds in Kickform Prediction Cards](https://www.figma.com/design/Z20oUbitTtFwhW7dmHLC4M/DES-1334---SWV---TPP-Design-Bookmaker-Odds-in-Kickform-Prediction-Cards?node-id=32-4184).

## What's here

`pages/aston-villa-vs-arsenal-4GVb9-with-odds-comparison-rows.html` — a real
Aston Villa vs Arsenal Kickform match-preview page (archived from
thepunterspage.com), with a bookmaker odds comparison added to all five
Kickform cards (Value Tip, Match Outcome, Correct Score, Both Teams to Score,
Match Goals). Each card gets a "Why? / Compare Odds" toggle; "Compare Odds"
reveals a bookmaker-by-bookmaker row list matching the Figma `Bookie CTA`
component exactly — logo, odds, welcome offer, and a "BET NOW" CTA, laid out
as one row per bookmaker (desktop) or a compact two-line row (narrower
cards / mobile), switching automatically via a CSS container query at the
component's own 560/561px breakpoint. The best price in each list is
highlighted with a tinted row and a teal odds figure.

`pages/assets/aston-villa-vs-arsenal-4GVb9/` — the real CSS, fonts, and
images the page depends on, downloaded and localized so the page renders
with no network access.

## Viewing it

Serve the `pages/` folder locally and open the HTML file, e.g.:

```bash
cd pages
python3 -m http.server 8000
```

Then visit `http://localhost:8000/aston-villa-vs-arsenal-4GVb9-with-odds-comparison-rows.html`.

## Status

Prototype for review — not yet registered in WIStorybook or merged into the
`wis-prototyping` skill's brand assets.
