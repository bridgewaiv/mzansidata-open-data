# Unemployment in South Africa: Stats SA's Quarterly Labour Force Survey, Q1 2008 to Q2 2026, national, provinces and metros

Stats SA's Quarterly Labour Force Survey (QLFS, P0211) as one tidy table: the official unemployment rate and the broader rates LU2, LU3 (the expanded rate) and LU4, employed, unemployed, labour force, people outside the labour force, labour force participation and absorption, for South Africa and the nine provinces every quarter from Q1 2008 and the eight metros from Q1 2015, with 95% intervals for the latest two quarters.

Version 2026.11.1, released 2026-11-08. Published by MzansiData (https://mzansidata.co.za), a non-commercial South African public-data site. Download page: https://mzansidata.co.za/data/downloads#south-africa-unemployment-qlfs

## Terms of use

Stats SA's copyright notice (https://www.statssa.gov.za/?page_id=425, read 7 November 2026) says: "Users may apply the information as they wish, provided that they acknowledge Stats SA as the source of the basic data wherever they process, apply, utilise, publish or distribute the data, and also that they specify that the relevant application and analysis (where applicable) result from their own processing of the data." These tables are MzansiData's processing of Stats SA's data. If you use them, name Stats SA as the source of the basic data and say that any analysis is your own.

Licence of the data: Stats SA copyright notice: use with acknowledgement of Stats SA as the source (https://www.statssa.gov.za/?page_id=425). MzansiData's own documentation (README.md, the column descriptions in datapackage.json) is CC BY 4.0.

## How to cite

MzansiData (2026). Unemployment in South Africa: Stats SA's Quarterly Labour Force Survey, Q1 2008 to Q2 2026, national, provinces and metros, version 2026.11.1. Source of the basic data: Statistics South Africa, Quarterly Labour Force Survey (P0211), Q2 2026 release and its trends workbook. Tables are MzansiData's own processing of the data. https://mzansidata.co.za/data/downloads#south-africa-unemployment-qlfs

## Files

### qlfs-tidy.csv

QLFS by quarter: South Africa, nine provinces and eight metros, long format. 12100 rows.

| Column | Type | Meaning |
|---|---|---|
| `date` | date | End of the period: the last day of the quarter (QLFS) or month (CPI) |
| `geo_code` | string | ZA = South Africa (CPI: total country); ZA-URB = all urban areas (the CPI headline); ZA-RUR = rural areas; ZA-WC, ZA-EC, ... = provinces (ISO 3166-2); CPT, BUF, NMA, MAN, ETH, EKU, JHB, TSH = the eight metros |
| `geo_name` | string | Name of the geography |
| `indicator` | string | unemployment_rate, employed, unemployed, labour_force, outside_labour_force, working_age_population, labour_force_participation_rate or absorption_rate |
| `definition` | string | For unemployment_rate: official (LU1), lu2, expanded_lu3 (LU3) or lu4; otherwise official, or 'aged 15 to 64' for the working-age population |
| `value` | number | The estimate |
| `unit` | string | percent or thousand persons |
| `ci_low` | number | Lower end of an approximate 95% interval (MzansiData's calculation from Stats SA's coefficient of variation); latest two quarters only |
| `ci_high` | number | Upper end of that interval |
| `seasonally_adjusted` | boolean | false for every row: Stats SA's QLFS tables and CPI indices used here are not seasonally adjusted |
| `vintage` | string | The Stats SA release this row was read from (QLFS quarter or CPI month). Later versions add older and newer vintages as more rows |
| `break` | string | Blank, or a short note that this row is not directly comparable with earlier rows; the README explains each note |
| `source_release` | string | Which Stats SA publication and table the value comes from, or that it is MzansiData's calculation |

CSV files are UTF-8, comma separated, with a full stop as the decimal mark. A blank cell means no published value.

## Source

- Stats SA, Quarterly Labour Force Survey (QLFS) trends workbook, Q1 2008 to Q2 2026 (published with P0211 Q2 2026). https://www.statssa.gov.za/publications/P0211/QLFS%20Trends%202008-2026Q2.xlsx (retrieved 2026-11-01, 1724015 bytes, SHA-256 `9a3d4d3becff0efaf3319613dcf34845306135c108b5d3b37c579a9029bebf22`). Used: Table 2.3, Labour force characteristics by province and metro. Downloaded in a browser from Stats SA's site (its files sit behind a bot check).
- Stats SA, Quarterly Labour Force Survey, Quarter 2: 2026, statistical release P0211 (embargoed until 11 August 2026, 11:00). https://www.statssa.gov.za/publications/P0211/P02112ndQuarter2026.pdf (retrieved 2026-11-01, 4987275 bytes, SHA-256 `ccfdb081197bb22857bc0ed976ad560e181fe0266b32cdd4f65f2e7af65ba59c`). Used: Table A (key labour market indicators), Table E (unemployment rate by province), Table 2.3A (sampling variability by province and metro), section 1 (the Q3 2025 questionnaire change). Downloaded in a browser from Stats SA's site (its files sit behind a bot check).

## Notes

- Not seasonally adjusted. Levels are in thousands of people aged 15 to 64, rounded to the nearest thousand; rates are % rounded to one decimal, as Stats SA prints them. Every figure for Q2 2026 matches the release's Table A (South Africa) and Table E (official rate and LU3 by province) for the three quarters each table shows; the tests in the MzansiData repository check this on every build.
- Definitions (P0211 Q2 2026, concepts and definitions): `official` (LU1) counts people aged 15 to 64 who were not employed in the reference week, actively looked for work or tried to start a business in the four weeks before the interview, and were available to start. `expanded_lu3` (LU3) adds the potential labour force: people available for work but not looking, or looking but not yet available. `lu2` adds time-related underemployment to the official rate; `lu4` combines both. Stats SA's releases now report LU1 to LU4. The "expanded" rate in releases before Q3 2025 is a different measure from LU3; this table uses LU3 for every quarter, from Stats SA's own trends workbook, so the broad series is consistent.
- Break: Stats SA revised the questionnaire in Q3 2025. Its Q2 2026 release (section 1) says the revision does "not affect the measurement or definition of employment and unemployment", so the official rate stays comparable, but the outside-the-labour-force concept changed and now includes the potential labour force. Rows for LU2, LU3, LU4 and outside_labour_force from Q3 2025 carry a note in `break`.
- ci_low and ci_high: an approximate 95% interval, value ± 1,96 × coefficient of variation × value, calculated by MzansiData from the coefficients of variation Stats SA publishes in the release's Table 2.3A (Q1 2026 and Q2 2026 only). Blank in earlier quarters. Differences between quarters smaller than the interval may be sampling noise.
- Metros: the workbook has metro estimates from Q1 2015 and none for Q4 2021 (no row for that quarter). Stats SA notes that values of 10 000 or lower are too small for reliable estimates.
- Phase 1 keeps one vintage, the Q2 2026 release. Stats SA revises past quarters (for example when population estimates change), so a later version adds earlier releases as rows with older vintages; do not mix vintages.
- Earlier method notes that are only in older releases (for example on how interviews were done in 2020 and 2021) are not yet flagged here; they come with the archive of past releases.

## Corrections

Found a figure that differs from the publisher's own file? Write to hello@mzansidata.co.za or use https://mzansidata.co.za/contact, naming the file, the row and the publisher's file you compared it with.
