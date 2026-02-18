# Sydney Metro Rental & Hospital Research Dashboard

Interactive dashboard for comparing rental prices, hospital proximity, and commute options across all 31 Sydney Metro stations — built to support a move from Toongabbie by end of November 2026.

## Live Demo

Deploy this yourself using one of the methods below, or just open `Sydney_Metro_Dashboard.html` in any browser.

## What's Included

| File | Description |
|------|-------------|
| `Sydney_Metro_Dashboard.html` | Interactive dashboard with filterable charts, rent comparisons, hospital driving matrix |
| `Sydney_Metro_Rental_Research.xlsx` | Full dataset across 6 tabs — station overview, rent ranges, hospital guide, move comparison, hospital-to-metro driving analysis, data sources |

## Dashboard Features

- **Filter by** metro line, budget, station status (open vs. opening H2 2026), and price tier
- **2BR and 3BR rent comparison** charts across all 31 stations
- **Rent distribution by line segment** (North West, City, Southwest)
- **Hospital-to-metro driving analysis** — every major Sydney teaching hospital mapped to nearest metro station with drive times
- **Full sortable station table** with rent ranges, nearest hospital, and suburb notes

## Quick Deploy

### Option A: Netlify Drop (no account needed)

1. Go to [app.netlify.com/drop](https://app.netlify.com/drop)
2. Drag `Sydney_Metro_Dashboard.html` onto the page
3. Get a live URL instantly

### Option B: GitHub Pages

```bash
git clone <this-repo>
# GitHub Pages serves from root by default
# Enable Pages in repo Settings > Pages > Source: main branch
```

The `index.html` will be served at `https://<username>.github.io/<repo-name>/`

### Option C: Vercel

```bash
npx vercel --prod
```

### Option D: Just open locally

```bash
open Sydney_Metro_Dashboard.html
# or on Windows:
start Sydney_Metro_Dashboard.html
```

No build step, no dependencies, no server required. The file is fully self-contained — Chart.js is loaded from CDN on first load.

## Data Sources

- **Rent data**: CoreLogic (via YourInvestmentPropertyMag), SydneyMovingGuide, RealEstateInvestar, Domain — Q3/Q4 2025 medians
- **Hospital data**: NSW Health, HealthDirect, Sydney Local Health District
- **Metro stations**: Sydney Metro (sydneymetro.info), Transport for NSW
- **Drive times**: Rome2rio, Google Maps estimates

## Disclaimers

- Rent figures are **estimates** based on median data. Actual rents vary by property age, condition, floor level, and exact location.
- Southwest line stations (Marrickville → Bankstown) are **not yet open**. Expected H2 2026 but has already slipped once.
- Hospital drive times are approximate and assume off-peak conditions unless noted.
- **Nepean Hospital** (Penrith) is the only major teaching hospital where metro access is borderline (30-45 min from Tallawong in peak traffic).
- Always verify current rents on [Domain.com.au](https://www.domain.com.au) or [RealEstate.com.au](https://www.realestate.com.au) before making decisions.

## Last Updated

February 2026
