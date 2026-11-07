# Crime victims in South Africa: Stats SA's Governance, Public Safety and Justice Survey, 2018/19 to 2025/26

From Stats SA's Governance, Public Safety and Justice Survey (GPSJS, P0341): the share of victims who reported each crime to the police, the share of households hit by housebreaking, and the share of people who feel safe walking alone in their area by day and after dark, 2018/19 to 2025/26.

Version 2026.11.0, released 2026-11-07. Published by MzansiData (https://mzansidata.co.za), a non-commercial South African public-data site. Download page: https://mzansidata.co.za/data/downloads#south-africa-crime-victims-survey-2018-2026

## Terms of use

Stats SA's copyright notice (https://www.statssa.gov.za/?page_id=425, read 7 November 2026) says: "Users may apply the information as they wish, provided that they acknowledge Stats SA as the source of the basic data wherever they process, apply, utilise, publish or distribute the data, and also that they specify that the relevant application and analysis (where applicable) result from their own processing of the data." These tables are MzansiData's processing of Stats SA's data. If you use them, name Stats SA as the source of the basic data and say that any analysis is your own.

Licence of the data: Stats SA copyright notice: use with acknowledgement of Stats SA as the source (https://www.statssa.gov.za/?page_id=425). MzansiData's own documentation (README.md, the column descriptions in datapackage.json) is CC BY 4.0.

## How to cite

MzansiData (2026). Crime victims in South Africa: Stats SA's Governance, Public Safety and Justice Survey, 2018/19 to 2025/26, version 2026.11.0. Source of the basic data: Statistics South Africa, Governance, Public Safety and Justice Survey (P0341). Tables are MzansiData's own processing of the data. https://mzansidata.co.za/data/downloads#south-africa-crime-victims-survey-2018-2026

## Files

### gpsjs-reporting-to-police.csv

Share of victims who reported the crime to the police, by crime. 103 rows.

| Column | Type | Meaning |
|---|---|---|
| `survey_year` | string | GPSJS survey year, for example 2025/26 |
| `crime_type` | string | Crime, as Stats SA names it |
| `unit` | string | households (household crimes) or individuals (individual crimes) |
| `pct_reported` | number | Share of victims who reported at least one incident to the police, % |

### gpsjs-housebreaking.csv

Share of households that experienced housebreaking in the previous 12 months. 8 rows.

| Column | Type | Meaning |
|---|---|---|
| `survey_year` | string | GPSJS survey year |
| `crime_type` | string | Housebreaking/burglary |
| `pct_households_12_months` | number | Share of households that experienced it in the previous 12 months, % |

### gpsjs-feeling-safe.csv

Share of people aged 16 and older who feel safe walking alone in their area. 16 rows.

| Column | Type | Meaning |
|---|---|---|
| `survey_year` | string | GPSJS survey year |
| `walking_alone` | string | during the day or after dark |
| `pct_feel_safe` | number | Share who feel very or fairly safe, % |

CSV files are UTF-8, comma separated, with a full stop as the decimal mark. A blank cell means no published value.

## Source

- Stats SA, Victims of Crime: Governance, Public Safety and Justice Survey 2025/26, P0341 (released 1 September 2026). https://www.statssa.gov.za/publications/P0341/P03412026.pdf (retrieved 2026-11-01, 1712794 bytes, SHA-256 `414b1f3931af38ef4bf166cc8cbd4651264004bd632fe2626d12766bc65ee6ee`). Release tables and figures used for 2021/22 onward.
- Stats SA, GPSJS 2025/26 P0341 Trends of Key Indicators (workbook). https://www.statssa.gov.za/publications/P0341/GPSJS%202025_26%20P0341%20Trends%20of%20Key%20Indicators%2031082026.xlsx (retrieved 2026-11-01, 76240 bytes, SHA-256 `d0218beeaf8b70ded0a9402be91bd44559370a8c9f9005359dc35645e8c0f77b`). Sheets "Reporting of crime", "Table 5 household crime 12mths" and "Feeling of safety", used for 2018/19 to 2020/21.

## Notes

- GPSJS replaced the Victims of Crime Survey in 2018/19 and Stats SA treats this as a series break, so only GPSJS years are here.
- Some items were not collected in some years; those rows are absent, not zero.
- Where the release PDF and the trends workbook disagree, the PDF is used from 2021/22 on.
- Survey years run from April to March.

## Corrections

Found a figure that differs from the publisher's own file? Write to hello@mzansidata.co.za or use https://mzansidata.co.za/contact, naming the file, the row and the publisher's file you compared it with.
