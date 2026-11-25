# Money calcs

A single-file, client-side money calculator suite combining portfolio growth projections, interest modeling, and reverse return analysis in one interface.

## Included Calculators

1. **Growth Chart**
   - Models a starting lump sum plus an optional monthly SIP over a chosen time horizon (`1` to `60` years) with monthly compounding.
   - Renders an SVG chart comparing projected portfolio value against total principal invested, paired with synced sliders and numeric inputs.

2. **Interest Counter**
   - Supports **Compound Interest** (`1x` yearly, `4x` quarterly, or `12x` monthly compounding) and **Simple Interest**.
   - Displays total maturity value, growth multiplier, invested principal vs. interest earned, a ratio bar, and average daily/monthly earning pace.
   - Includes a one-click summary copy action.

3. **Reverse %**
   - Works backward from an initial amount, final amount, and time duration (`years` or `months`) to compute annualized **CAGR**, flat **Simple Interest Rate**, and total gain/loss percentage.
   - Includes quick scenario presets and one-click result copying.

## Setup & Hosting

- Save the application file as `money_calcs.html` (or `index.html` if hosting it as the root page).
- No build step or backend server is required; open directly in a browser or host via GitHub Pages.
- Designed to sit cleanly alongside **Wired SYS** as part of a lightweight static tool collection.