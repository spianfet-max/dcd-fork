# DCD Fork

A single-file interactive visualiser for a dual currency deposit (DCD). Drag the rate at maturity to see whether the deposit converts at the strike, what you receive in each case, and how the coupon, breakeven and history change the picture.

**Mockup only. Illustrative pricing, not a quote or investment advice.**

## Run it

Open `index.html` in a browser. No build step, no server.

## What it shows

- The rate path forking at the strike, with the coupon cushion up to the breakeven rate (hover the breakeven line for the formula).
- The two outcomes (converted or not) with amounts, the effective rate including coupon, and probabilities.
- Four coupon views (cushion, accrual, bars, net versus holding the deposit currency).
- Share of past days beyond the strike over 1 to 5 years, from bundled ECB history.
- Indicative model pricing of the coupon (Garman-Kohlhagen, no bank margin) with an editable plain time-deposit rate for comparison.
- English and Japanese, light and dark mode.

## Notes

- Rates are ECB daily reference rates (units per USD) bundled in the file, as of 2 Oct 2026. When online, the page tries to refresh spot rates from the Frankfurter API and falls back to the bundled rates.
- Volatility defaults and plain deposit rates are rough assumptions, editable in the terms sheet. Replace them with desk values before real use.
- Settings (language, mode, coupon view) are stored in the browser only.
