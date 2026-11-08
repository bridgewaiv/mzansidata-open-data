# Inflation in South Africa: Stats SA's Consumer Price Index, monthly, headline since 1922, provinces and groups since 2008

Stats SA's Consumer Price Index (CPI, P0141) as one tidy table: the official headline inflation rate every month since January 1922 and the headline index since 1980; the index and annual rate for the total country, rural areas, the nine provinces and the 13 spending groups since 2008; and core inflation for September 2026, all to the September 2026 release.

Version 2026.11.1, released 2026-11-08. Published by MzansiData (https://mzansidata.co.za), a non-commercial South African public-data site. Download page: https://mzansidata.co.za/data/downloads#south-africa-inflation-cpi

## Terms of use

Stats SA's copyright notice (https://www.statssa.gov.za/?page_id=425, read 7 November 2026) says: "Users may apply the information as they wish, provided that they acknowledge Stats SA as the source of the basic data wherever they process, apply, utilise, publish or distribute the data, and also that they specify that the relevant application and analysis (where applicable) result from their own processing of the data." These tables are MzansiData's processing of Stats SA's data. If you use them, name Stats SA as the source of the basic data and say that any analysis is your own.

Licence of the data: Stats SA copyright notice: use with acknowledgement of Stats SA as the source (https://www.statssa.gov.za/?page_id=425). MzansiData's own documentation (README.md, the column descriptions in datapackage.json) is CC BY 4.0.

## How to cite

MzansiData (2026). Inflation in South Africa: Stats SA's Consumer Price Index, monthly, headline since 1922, provinces and groups since 2008, version 2026.11.1. Source of the basic data: Statistics South Africa, Consumer Price Index (P0141), September 2026 release, its time series and the CPI History. Tables are MzansiData's own processing of the data. https://mzansidata.co.za/data/downloads#south-africa-inflation-cpi

## Files

### cpi-tidy.csv

CPI by month: index and annual inflation, headline, core, provinces and groups, long format. 11928 rows.

| Column | Type | Meaning |
|---|---|---|
| `date` | date | End of the period: the last day of the quarter (QLFS) or month (CPI) |
| `geo_code` | string | ZA = South Africa (CPI: total country); ZA-URB = all urban areas (the CPI headline); ZA-RUR = rural areas; ZA-WC, ZA-EC, ... = provinces (ISO 3166-2); CPT, BUF, NMA, MAN, ETH, EKU, JHB, TSH = the eight metros |
| `geo_name` | string | Name of the geography |
| `indicator` | string | cpi_index or inflation_annual (change on the same month a year earlier) |
| `definition` | string | headline, core, all_items, or a spending group coicop_01_... to coicop_13_... |
| `value` | number | The index or rate |
| `unit` | string | 'index, December 2024 = 100' or percent |
| `ci_low` | number | Blank: the CPI is not a sample survey estimate with published intervals |
| `ci_high` | number | Blank |
| `seasonally_adjusted` | boolean | false for every row: Stats SA's QLFS tables and CPI indices used here are not seasonally adjusted |
| `vintage` | string | The Stats SA release this row was read from (QLFS quarter or CPI month). Later versions add older and newer vintages as more rows |
| `break` | string | Blank, or a short note that this row is not directly comparable with earlier rows; the README explains each note |
| `source_release` | string | Which Stats SA publication and table the value comes from, or that it is MzansiData's calculation |

CSV files are UTF-8, comma separated, with a full stop as the decimal mark. A blank cell means no published value.

## Source

- Stats SA, P0141 CPI (COICOP) from January 2008, release 2026 09, ASCII time series. https://www.statssa.gov.za/timeseriesdata/Ascii/P0141%20-%20CPI(COICOP)%20from%20Jan%202008%20(202609).zip (retrieved 2026-11-08, 245695 bytes, SHA-256 `c2d0e7af15171284952526f42b0fc887459395ec0067d05a1efcd73361da05de`). Used: Monthly indices (December 2024 = 100), January 2008 to September 2026: all items for all urban areas, total country, rural areas and the nine provinces; the 13 COICOP divisions for all urban areas. Downloaded in a browser from Stats SA's site (its files sit behind a bot check).
- Stats SA, Consumer Price Index, September 2026, statistical release P0141 (embargoed until 21 October 2026, 10:00). https://www.statssa.gov.za/publications/P0141/P0141September2026.pdf (retrieved 2026-11-08, 531659 bytes, SHA-256 `0ee131034f62c195c09f4ca0ce14b5d09c38dd5c85cec0428de6b585f497ab36`). Used: Table A (main indices, including core), Table B (headline index and rates, 2022 to 2026), Table E (indices for all urban areas by group). Downloaded in a browser from Stats SA's site (its files sit behind a bot check).
- Stats SA, CPI History: Table B1, CPI headline index numbers (December 2024 = 100) since 1980, and Table B2, CPI headline year-on-year rates since 1911 (published with P0141 September 2026). https://www.statssa.gov.za/publications/P0141/CPIHistory.pdf (retrieved 2026-11-08, 429959 bytes, SHA-256 `b6b21ee9fec543fb7785ee05284393c17759ef4667d9629f080167cb5666a4b2`). Used: Headline index from January 1980 to December 2007, and the official inflation rates from January 1922. Downloaded in a browser from Stats SA's site (its files sit behind a bot check).

## Notes

- Not seasonally adjusted. Indices are on Stats SA's base, December 2024 = 100, one decimal, as published. Rates are % with one decimal.
- Definitions: `headline` is the CPI for all items in all urban areas, the figure Stats SA reports as the inflation rate. `core` is Stats SA's CPI excluding food and non-alcoholic beverages, fuel and energy. `all_items` is the CPI for the total country, rural areas or a province. `coicop_01_...` to `coicop_13_...` are the 13 spending groups (COICOP divisions) for all urban areas.
- Headline inflation rates (`inflation_annual`, `headline`) are the official rates as Stats SA published them in each month's release (CPI History, Table B2 and its note 3), not recalculated. All other annual rates are MzansiData's calculation from Stats SA's published, rounded indices (source_release says so). For September 2026 every one of them matches the release (Tables A and E); in earlier years a calculation from rounded indices can differ from a rate calculated on unrounded figures by a tenth or two, more where index values are small.
- Break in January 2009: until December 2008 the headline CPI covered primary urban areas only, and from January 2009 all urban areas; Stats SA also made substantial changes to how the CPI is compiled then and linked the two into one index (CPI History, notes 1 and 2). Headline rows before 2009 come from the CPI History and carry a note in `break`. The time series file's all-urban index for 2008 is a different series from the headline of the time, so it is left out.
- From 2009 the headline index comes from Stats SA's time series file. The CPI History's rounded headline index differs from it by 0,1 in 25 months between 2009 and 2016 and agrees exactly from 2017.
- Core inflation: Stats SA's time series files do not include it, so this version has only the three months in the September 2026 release's Table A. Longer core and group histories come with the archive of past releases.
- Stats SA's series for insurance and financial services (group 12) starts in December 2024; the row for its first month says so.
- Phase 1 keeps one vintage, the September 2026 release. Later versions add each month's release as a vintage; do not mix vintages.

## Corrections

Found a figure that differs from the publisher's own file? Write to hello@mzansidata.co.za or use https://mzansidata.co.za/contact, naming the file, the row and the publisher's file you compared it with.
