# Perfect Timing

A counting-up quiz game prototype. A number climbs from zero; tap the big button the instant it reaches the answer.

- First to tap at or past the answer wins the round. Within 1.5 seconds of the exact number is a bullseye, worth double.
- Tap too early and the button says so and keeps counting.
- If the count reaches double the answer, the round is dead and nobody scores.
- Ten rounds. Most points wins.

## Running it

The whole game is `index.html`: no build step and no dependencies beyond two Google Fonts. Open the file in a browser, or serve the repo with GitHub Pages.

## Changing it

- **Questions** live in the `DEFAULT_DECK` array near the top of the script. Each entry is `[question, answer, unit, note]`; an entry with `{ m: [...], i: [...] }` has a metric and an imperial version. Players can also edit the deck on their own device from Settings → Edit the deck.
- **Pacing and scoring** are in the `TUNING` block just above the deck: seconds to reach the answer, the bullseye window, the double-the-answer cutoff, and the small/medium/big mix per game.
- **Colors and fonts** are tokens in the `:root` block at the top of the stylesheet.
