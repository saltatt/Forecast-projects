# Forecast-projects
# Cafe Profit Forecast

Forecasts whether monthly profit of a small cafe kiosk (inside a baby swimming studio) will rise or fall from August to December 2026, using only one month of real sales data.

## Notebook
`cafe_profit_forecast.ipynb` – runs in Google Colab or Jupyter (needs `numpy`, `pandas`, `matplotlib`). Run all cells; charts appear inline.

## How it works
`profit = sales × (1 − ingredient cost share) − fixed costs (rent 110k + barista 65k KZT)`

| Section | What it shows |
|---|---|
| 1. August | daily sales vs 20k target, best weekdays |
| 2. Assumptions | product mix by month (cold drinks → hot drinks, pastries) |
| 3. Forecast | monthly profit in 3 scenarios + likely range (5,000 simulations) |
| 4. Drivers | why profit changes: demand, margin, days in month |
| 5. Sensitivity | which input moves December profit most |
| 6. Answer | plain-language verdict |

## Key result (base case)
Profit grows from ~40k KZT (Aug) to ~88k KZT (Dec), peaking in October; the main driver by December is better margin from hot drinks.

## Limits
- Only 19 recorded days; seasonal demand, product mix and cost shares are **assumptions** (marked ⚙️) – replace them with real data.
- Reaching the 20k KZT/day target needs ~40% more sales than August's average.
