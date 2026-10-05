# London Property Strategy Atlas

A single self-contained page (`index.html`) bringing together the research on the Draft London Plan 2026, TfL connectivity and demand, house prices, and three property investment strategies. Open `index.html` in any modern browser. It needs an internet connection only for the map library (d3 from cdnjs) and fonts.

## Three strategies

| | Strategy 1: non-prime bargain, refurbish, sell | Strategy 2: prime bargain, refurbish, sell | Strategy 3: long-term rental hold |
|---|---|---|---|
| Where | Any zone, not prime | Top 10% house prices (median ≥ £1.53m) | Houses only, Zone 1–3 |
| Must pass | London Plan future-growth score ≥ 0.3; refurbished exit ≤ 10x local household income; 15% margin on cost | 15% margin on cost; listing below local £/sq ft and sold medians | London Plan future-growth score ≥ 0.3; net yield on all-in cost ≥ 5%; positive cash flow after refinancing |
| Market capex | £100/sq ft | £200/sq ft | £70/sq ft + £10k EPC |

## What the page contains

1. **Three strategies**: rules, verdicts and the market cost assumptions.
2. **Recommended deals (October 2026)**: live listings with the maximum bid that still clears each strategy's hurdle.
3. **Deal screen**: 206 Rightmove listings run through the cost model (SDLT at additional-dwelling rates, fees, finance, capex, exit value).
4. **Target areas by strategy**: neighbourhood shortlists.
5. **Corrections**: earlier conclusions that were revised.
6. **Research map**: borough and neighbourhood layers. Includes London Plan Opportunity Areas, town-centre upgrades, growth locations, the CAZ and its 3 km ring, industrial land and release sites, archaeology priority areas, conservation areas, protected views, Superloop, TfL station demand and seasonality, house price trends, and an extension-site checker.
7. **Evidence**: price effects of past transport schemes, large developments and town-centre facilities (1995–2025), market check, transport schemes, sector pros and cons, Opportunity Area table.

## Data workbooks (`data/`)

| File | Contents |
|---|---|
| `shortlist_market_costs.xlsx` | Deal screen results, near-passing flips, rental candidates, assumptions |
| `deal_profit_with_capex.xlsx` | Worked example deals with sensitivity |
| `three_strategies.xlsx` | Neighbourhood shortlists per strategy and method |
| `near_station_houses.xlsx` | Houses within 0.2 miles of target stations: station summaries (individual sales removed for the public repo) |
| `prime_near_station_houses.xlsx` | Same for prime stations, plus prime neighbourhood metrics |
| `TfL_station_monthly_entry_exit.xlsx` | Monthly entry and exit taps by station, Jan 2019 – Sep 2026 |

## Sources

- **Planning**: Draft London Plan 2026 (GLA); London Datastore (CAZ, town centres, SIL, LVMF); planning.data.gov.uk (archaeological priority areas, conservation areas, Article 4, listed buildings, flood zones).
- **Transport**: TfL 2026 Business Plan; Mayor's Transport Strategy delivery report 2025/26; TfL Network Demand open data; TfL StopPoint API; DfT NaPTAN.
- **Prices and population**: HM Land Registry Price Paid Data (2019–Aug 2026); ONS small-area house price statistics; ONS Price Index of Private Rents (Aug 2026); ONS small-area income estimates (FYE2023); Census 2021 (Nomis); ONS small-area population estimates.
- **Live listings**: Rightmove listings viewed on 5 October 2026.

Contains HM Land Registry data © Crown copyright and database right 2026. Contains OS data © Crown copyright 2026. Contains public sector information licensed under the Open Government Licence v3.0.

## Limitations

- **Map accuracy**: Opportunity Area points and transport routes are hand-placed and approximate.
- **Data age**: PTAL is from 2015, before the Elizabeth line opened.
- **Small samples**: resale counts are small for some areas.
- **Estimated inputs**: listing sizes are estimated from bedroom counts where the listing gives none. Asking £/sq ft is taken from current listings, not sold prices.
- **Assumptions**: cost, finance and rent assumptions are market mid-range estimates, not quotes.
- **Not advice**: this is a screening tool, not investment, tax or legal advice. SDLT and the holding structure materially change the results.
