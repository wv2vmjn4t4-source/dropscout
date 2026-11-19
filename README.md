# DropsFeed

A crypto airdrop tracker: live, upcoming and ended airdrops with step-by-step guides, filters, a watchlist and a deadline calendar.

The site is a single static page (`index.html`) with no build step. Deploy it on Netlify, Vercel or GitHub Pages.

> The projects listed are fictional demo data. Not financial advice.

## Editing airdrops (`airdrops.json`)

Each airdrop has these fields. Status (live / upcoming / ended) is calculated from `start` and `end` automatically.

- `start`, `end`: ISO dates, `end: null` means no deadline yet (shows TBA)
- `confirmed`: true only if the project itself confirmed a token airdrop
- `url`: official page only. Leave empty if you can't verify it
- `funding`, `fundingUsd`, `backers`, `share`, `cost`, `costUsd`, `timeMin`: feed the DropsFeed score (S/A/B/C)
- `sponsored: true`: pins the project to the top with a "Sponsored" label (paid listings)
- `affiliate: {"label": "Use wallet X for this drop", "url": "https://..."}`: shows an "Ad" referral box inside the guide

Banners: edit the `BANNERS` block in `index.html`.
