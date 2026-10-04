# DCD Fork

A single-file interactive visualiser for a dual currency deposit (DCD). Drag the rate at maturity and see whether the deposit converts at the strike, what you receive in each case, and the coupon accruing.

**Mockup only. Illustrative, not a quote or investment advice.**

## Run it

Open `index.html` in a browser. No build step, no server.

## Notes

- English and Japanese, light and dark mode.
- Rates are ECB daily reference rates (units per USD) bundled in the file, as of 2 Oct 2026. When online, the page also tries to refresh spot rates from the Frankfurter API and falls back to the bundled rates if that fails.
- Volatility defaults per currency pair are rough assumptions. Replace them with desk values before real use.
- Settings (language, mode) are stored in the browser only.
