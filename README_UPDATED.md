# $0 → $100 AI Experiment Website

## Pages
- `index.html` — main public page and money ledger.
- `experiment-log.html` — living record of ideas and actions.
- `progress.html` — income timeline and cumulative-income chart.

## Updating the experiment log
Open `experiment-log.html` and edit the `ideas` and `actions` arrays near the bottom.

Example idea:
`{date:"2026-09-12",title:"New idea",status:"Testing",description:"What we want to test."}`

Example action:
`{date:"2026-09-12",time:"14:30",type:"Outreach",title:"Sent 5 proposals",result:"Waiting for responses."}`

## Updating income
Open `progress.html` and add verified income events to the `events` array. Use an ISO-like local timestamp when possible.

Example:
`{date:"2026-09-12T14:30:00",label:"First $1 received",amount:1,type:"Income",note:"Verified contribution."}`

Only actual income should use `type:"Income"`. The starting point is recorded separately at $0. The $100 goal is a fixed target and is not treated as earned money.

The existing `index.html` ledger remains the detailed source for income and expenses.

## Publishing
Upload/replace these files in the GitHub Pages repository:
- `index.html`
- `experiment-log.html`
- `progress.html`

The progress chart uses Chart.js from jsDelivr, so the chart requires an internet connection when the page loads.
