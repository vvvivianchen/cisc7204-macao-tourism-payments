# Data files

Download date for every file in this folder: 4 November 2026.
Last month used: September 2026. October 2026 restaurant payments were not out yet. DSEC's calendar puts that release on 30 November 2026.

`pay_m09.xlsx`
The September 2026 DSEC workbook for restaurant and retail electronic payments (table id 502). It reports cumulative, year-on-year and month-on-month percentage changes. It does not give the monthly amount in patacas. That is why the level is not taken from this file.

`vis_m09.xlsx`
The September 2026 visitor-arrivals workbook (table id 402). The sheets compare recent months. They are not a 21-month time series of same-day and overnight visitors, so the counts are not taken from this file either.

`pay_news.json`
The text of 21 DSEC news releases, January 2025 to September 2026, one object per month (`y`, `m`, `t`). The monthly restaurant total is read from `t`.

`payment_levels.csv`
Those 21 monthly totals, in MOP billion, typed from the releases. January 2025 is the revised MOP1.3 billion named in the February 2025 release, not the MOP1.1 billion in the first January release.

`vis_news.json`
The text of the 21 visitor-arrivals releases for the same months (`y`, `m`, `id`, `t`). Same-day and overnight counts are read from `t`. A published total is kept only when it equals same-day plus overnight within 5 persons. Otherwise the total is the sum of the two counts.

`merged_monthly.csv`
The table the notebook writes after the checks above. One row per month. Payment is also stored in MOP million, and the two visitor counts in thousands, so a regression coefficient is MOP million per extra thousand visitors.
