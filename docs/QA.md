# Actual verification record

Date: 2026-10-11. Public GitHub Pages URL loaded in installed Chromium/Browse with HTTP 200. These are implementation checks, not business performance.

- Desktop viewport: 1440 × 1000. Mobile viewport: 390 × 844.
- Document horizontal overflow: false at both widths. Wide tables scroll inside their own containers.
- Browser console: no errors/warnings observed during checked flows.
- 13 deterministic Node tests pass.
- Live flows: Budget change updates spend/contribution; incomplete-window checkbox changes verdict to Wait; negative budget blocks export. Default small-sample verdict is inconclusive. Reset is repeatable.

Screenshots: [desktop](desktop.png), [mobile](mobile.png).

No real-device Safari/Firefox, screen-reader or load testing is claimed.

## Export and keyboard verification

Actual live export Blob contents captured and saved as [sample memo](sample-export.md) and [scenario JSON](sample-export.json). Memo includes sensitivity and experiment observations. Repeated exports produce valid content. Keyboard Tab from budget reaches reserve. Mobile table scroll is contained. Invalid inputs clear the forecast and block exports.
