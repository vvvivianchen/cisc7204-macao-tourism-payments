# Codebook

Class D – Team 01. Restaurant electronic payments and visitor arrivals, Macao.
Unit of observation: one calendar month. Window: January 2025 to September 2026 (21 months). Download date: 4 November 2026.

The dependent variable is restaurant electronic payment transaction value. It is not restaurant revenue. DSEC compiles it from major merchant acquirers, which handle about 95% of electronic payment value in Macao. Cash is excluded. Residents and visitors are not separated. Electronic payments are about 70% to 80% of restaurant and retail receipts (DSEC release for August 2026, cited in the report).

| Column | Unit | Meaning |
| --- | --- | --- |
| date | month | First day of the month, used only as the time label |
| year, month | calendar | Taken from the release the row came from |
| payment_billion | MOP billion | Monthly restaurant total as stated in that month's news release. January 2025 is the revised 1.30 |
| payment_mop_million | MOP million | `payment_billion × 1000`. This is the regression outcome |
| same_day | persons | Same-day visitors in the arrivals release |
| overnight | persons | Overnight visitors in the arrivals release |
| total | persons | Published total if it matches same-day + overnight within 5 persons; otherwise the sum |
| total_published | true/false | Whether the published total was kept |
| same_day_thousands, overnight_thousands, total_thousands | thousand persons | Person counts divided by 1,000 |
| overnight_share | percent | Overnight visitors divided by total, times 100 |
| payment_index, overnight_index, same_day_index | index | January 2025 = 100 |
| payment_yoy, overnight_yoy, same_day_yoy | percent | Change from the same month a year earlier. Blank for 2025. Nine values in 2026. Not used in the regression |

No month is interpolated. A missing month would have been dropped and listed. None was missing, so the table has 21 rows.

The two visitor groups are not put into a model together with their total. Total = same-day + overnight, so that model would be perfectly collinear.
