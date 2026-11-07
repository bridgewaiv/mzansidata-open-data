# South Africa's mid-year population by province, 2002 to 2026 (Stats SA, 2026 series)

Mid-year population of South Africa and its nine provinces for every year from 2002 to 2026, all from Stats SA's 2026 mid-year population estimates (P0302), summed from Stats SA's district council projection by sex and age.

Version 2026.11.0, released 2026-11-07. Published by MzansiData (https://mzansidata.co.za), a non-commercial South African public-data site. Download page: https://mzansidata.co.za/data/downloads#south-africa-population-2002-2026

## Terms of use

Stats SA's copyright notice (https://www.statssa.gov.za/?page_id=425, read 7 November 2026) says: "Users may apply the information as they wish, provided that they acknowledge Stats SA as the source of the basic data wherever they process, apply, utilise, publish or distribute the data, and also that they specify that the relevant application and analysis (where applicable) result from their own processing of the data." These tables are MzansiData's processing of Stats SA's data. If you use them, name Stats SA as the source of the basic data and say that any analysis is your own.

Licence of the data: Stats SA copyright notice: use with acknowledgement of Stats SA as the source (https://www.statssa.gov.za/?page_id=425). MzansiData's own documentation (README.md, the column descriptions in datapackage.json) is CC BY 4.0.

## How to cite

MzansiData (2026). South Africa's mid-year population by province, 2002 to 2026 (Stats SA, 2026 series), version 2026.11.0. Source of the basic data: Statistics South Africa, Mid-year population estimates 2026 (P0302). Tables are MzansiData's own processing of the data. https://mzansidata.co.za/data/downloads#south-africa-population-2002-2026

## Files

### sa-population-2002-2026.csv

Mid-year population, South Africa and the nine provinces, 2002 to 2026. 250 rows.

| Column | Type | Meaning |
|---|---|---|
| `year` | integer | Year (mid-year estimate, 30 June) |
| `geography` | string | South Africa or a province |
| `population` | integer | Mid-year population, people |

CSV files are UTF-8, comma separated, with a full stop as the decimal mark. A blank cell means no published value.

## Source

- Stats SA, Mid-year population estimates 2026, P0302 (released 30 July 2026), supplementary workbook "District Council projection by sex and age (2002-2026)". https://www.statssa.gov.za/publications/P0302/District%20Council%20projection%20by%20sex%20and%20age%20(2002-2026)_web.xlsx (retrieved 2026-11-01, 695864 bytes, SHA-256 `3fd9b21f495f5d35da0f2b589eb17775f12aea1aec762b4b1a28a5963abc47ae`).

## Notes

- Each figure is the sum over districts, sexes and ages in Stats SA's workbook. The 2026 totals match the provincial table in the P0302 release exactly.
- Because of rounding, the South Africa row can differ from the sum of the nine provinces by up to 2 people in some years.
- Every year comes from the same 2026 vintage. Earlier releases of P0302 gave different figures for past years; do not mix vintages.
- Provinces are on current boundaries for every year.

## Corrections

Found a figure that differs from the publisher's own file? Write to hello@mzansidata.co.za or use https://mzansidata.co.za/contact, naming the file, the row and the publisher's file you compared it with.
