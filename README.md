# Turkey Aftershock Forecasting

How long does aftershock activity in Turkey take to return to its background level
after a large earthquake, and can the daily number of events be forecast from recent activity?

🚧 Work in progress: data cleaning and exploration (October–November 2026).

## Data

**Source:** AFAD Deprem Dairesi Başkanlığı, earthquake catalog — https://deprem.afad.gov.tr  
Used with attribution. The raw data is **not redistributed** in this repository, in line with AFAD's terms.

**How to download the same file:**
1. Go to deprem.afad.gov.tr → Deprem Kataloğu (Event Catalog)
2. Use these settings:
   - Date: 01-01-2010 00:00:00 → 28-02-2025 23:59:59 (UTC)
   - Latitude: 35.5 → 42.5
   - Longitude: 25.5 → 45.0
   - Minimum magnitude: 2.5
   - Everything else: default
3. Export as CSV and save it as `data/raw/afad_turkey_2010-2025_m2.5.csv`

The download contains 92,986 events.

## Project structure

- `data/raw/` – original download (not committed)
- `data/processed/` – cleaned data (not committed)
- `notebooks/` – analysis notebooks
- `figures/` – saved plots
