# How South Africans use Claude: Anthropic Economic Index, May 2026

Claude usage in South Africa, its four provinces with published figures and 26 African countries, from the Anthropic Economic Index (period 1 May 2026): the Anthropic Usage Index and rank, work, personal and coursework shares, augmentation and automation, and South Africa's top request topics, job categories and tasks against the world.

Version 2026.11.0, released 2026-11-07. Published by MzansiData (https://mzansidata.co.za), a non-commercial South African public-data site. Download page: https://mzansidata.co.za/data/downloads#south-africa-claude-usage

## Terms of use

The Anthropic Economic Index data is released by Anthropic under CC BY 4.0 (code under MIT). These tables are a selection from it, reshaped by MzansiData. If you use them, credit "Anthropic Economic Index, Anthropic, CC BY 4.0" and MzansiData for the tables, and say if you changed them.

Licence of the data: Creative Commons Attribution 4.0 International (https://creativecommons.org/licenses/by/4.0/). MzansiData's own documentation (README.md, the column descriptions in datapackage.json) is CC BY 4.0.

## How to cite

MzansiData (2026). How South Africans use Claude: Anthropic Economic Index, May 2026, version 2026.11.0. Anthropic Economic Index, Anthropic, CC BY 4.0. Tables by MzansiData. https://mzansidata.co.za/data/downloads#south-africa-claude-usage

## Files

### claude-usage-geographies.csv

Usage by geography: the world, 26 African countries and 4 South African provinces. 31 rows.

| Column | Type | Meaning |
|---|---|---|
| `geography_level` | string | world, country or province |
| `code` | string | ISO 3166-1 alpha-3 for countries, ISO 3166-2 for provinces; blank for the world |
| `name` | string | Geography name as published |
| `usage_index` | number | Anthropic Usage Index (countries only): share of usage divided by share of working-age population |
| `rank` | integer | Rank by usage index (countries, of rank_of) or by share of South Africa's usage (provinces) |
| `rank_of` | integer | How many geographies the rank is out of |
| `share_of_country_usage_pct` | number | Provinces: share of South Africa's observed Claude usage, % |
| `work_pct` | number | Share of classified conversations that look like work, % |
| `personal_pct` | number | Share that look like personal life, % |
| `coursework_pct` | number | Share that look like coursework, % |
| `augmentation_pct` | number | Share in augmentation style (the person stays involved), % |
| `automation_pct` | number | Share in automation style (the person directs Claude to complete the task), % |
| `top_request_topic` | string | Provinces: the most common request topic |
| `top_request_topic_pct` | number | Provinces: that topic's share of the province's conversations, % |
| `education_topic_pct` | number | Provinces: share of conversations on Education & Learning, % |

### claude-usage-za-breakdown.csv

South Africa: top request topics, job categories and tasks against the world. 28 rows.

| Column | Type | Meaning |
|---|---|---|
| `facet` | string | request_topic (top 10), job_category (top 10) or task (top 8) |
| `rank` | integer | Rank within the facet in South Africa |
| `name` | string | Topic, job category (O*NET major group) or task (O*NET task statement), as published |
| `za_pct` | number | Share of South Africa's classified conversations, % |
| `global_pct` | number | The same share for all covered countries, % |

CSV files are UTF-8, comma separated, with a full stop as the decimal mark. A blank cell means no published value.

## Source

- Anthropic Economic Index (dataset metadata: publisher Anthropic, licence CC BY 4.0, latest period 2026-05-01, modified 2026-06-24). https://www.anthropic.com/economic-index (retrieved 2026-10-31). Read through the Anthropic Economic Index MCP tools (econ_index_*), not a downloaded file, so there is no file checksum. The same data is published at https://huggingface.co/datasets/Anthropic/EconomicIndex ("Data released under CC-BY, code released under MIT License").

## Notes

- Observed Claude chat and Cowork conversations. Not a measure of jobs, the labour market or AI use overall.
- The Anthropic Usage Index is a geography's share of Claude usage divided by its share of working-age population; 1,0 is usage in line with population. Countries are compared with all 121 covered countries.
- Provinces have no published usage index. share_of_country_usage_pct is the province's share of South Africa's observed usage; the four provinces published add up to 94,74%.
- A blank cell means the value is not published. It may be zero.
- Augmentation and automation are conversation styles, not job outcomes. They are published for South Africa and the provinces only in this selection.

## Corrections

Found a figure that differs from the publisher's own file? Write to hello@mzansidata.co.za or use https://mzansidata.co.za/contact, naming the file, the row and the publisher's file you compared it with.
