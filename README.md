# Cannon Cove · $0 → $100

A cute, pixel-inspired redesign of the public Cannon Cove experiment website.

## Versions

- `index.html` — simple landing page that lets visitors choose a screen-specific deck.
- `mobile.html` — phone-first layout with large touch targets, stacked cards, and a sticky bottom navigation bar.
- `desktop.html` — wide layout with a persistent project sidebar, split hero, dashboard stats, and five-step roadmap.
- `experiment-log.html` — public captain's log of ideas, actions, and results.
- `progress.html` — verified earned-revenue chart.
- `policy.html` — support/refund policy.
- `site-data.js` — single source of truth for the public ledger, revenue events, ideas, and actions.

## Updating the experiment

Most ongoing updates should happen in `site-data.js`.

Ledger types:
- `Revenue` — earned money that counts toward the $100 goal.
- `Support` — voluntary support, tracked separately.
- `Expense` — money spent by the experiment, recorded as a negative amount.

The current ledger includes the $20 Claude Pro development expense.

## Design direction

The redesign uses a nautical pixel-art vocabulary, chunky borders, high-contrast type, parchment-like cards, sea/sky colors, and tactile button shadows. The mobile and desktop versions are intentionally different layouts rather than a single desktop page merely squeezed onto a phone.

No build system is required. These are static files suitable for GitHub Pages.
