# MzansiData open data

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24337957.svg)](https://doi.org/10.5281/zenodo.24337957)

Clean, documented CSV files of South African public data from MzansiData (https://mzansidata.co.za), a non-commercial site that turns South Africa's public data into charts and explainers. Every figure comes from the publishing body itself, and each package names the publisher's file it comes from, with the address, retrieval date and, where we downloaded a file, its SHA-256.

We publish a dataset here only when its publisher's own terms allow it, and each package carries those terms. The same files are on https://mzansidata.co.za/data/downloads.

## How to cite

Cite the package you used with its own `CITATION.cff` (each names its publisher's source). To cite the whole collection, use its Zenodo DOI, which always points to the latest version: MzansiData, *MzansiData open data*, Zenodo, https://doi.org/10.5281/zenodo.24337957. Every release has its own version DOI on that page. GitHub's "Cite this repository" button uses `CITATION.cff` at the top of this repository.

## Packages

| Package | Publisher | Terms | Files |
|---|---|---|---|
| [`south-africa-claude-usage/`](south-africa-claude-usage/) | Anthropic (Anthropic Economic Index) | CC BY 4.0 | Usage by geography (world, 26 African countries, 4 provinces); South Africa's top request topics, job categories and tasks |
| [`south-africa-population-2002-2026/`](south-africa-population-2002-2026/) | Statistics South Africa (P0302) | Stats SA copyright notice: name Stats SA as the source, say the analysis is your own processing | Mid-year population, South Africa and the provinces, 2002 to 2026 |
| [`south-africa-crime-victims-survey-2018-2026/`](south-africa-crime-victims-survey-2018-2026/) | Statistics South Africa (P0341, GPSJS) | As above | Reporting to the police, housebreaking, feeling safe, 2018/19 to 2025/26 |
| [`south-africa-unemployment-qlfs/`](south-africa-unemployment-qlfs/) | Statistics South Africa (P0211, QLFS) | As above | Official and expanded (LU3) unemployment, employed, unemployed, participation and absorption: South Africa and the provinces every quarter since 2008, the eight metros since 2015, with 95% ranges for the latest quarters |
| [`south-africa-inflation-cpi/`](south-africa-inflation-cpi/) | Statistics South Africa (P0141, CPI) | As above | Headline inflation every month since 1922, the CPI index, provinces and spending groups since 2008, core inflation |

Each data package has a `README.md` (data dictionary, source, terms, citation), a [Frictionless](https://frictionlessdata.io/) `datapackage.json` (schema, row counts, SHA-256) and a `CITATION.cff`.

## Where else to get them

The same files, version by version:

| Package | On mzansidata.co.za | Internet Archive (version 2026.11.4) | Kaggle |
|---|---|---|---|
| `south-africa-claude-usage` | [Downloads](https://mzansidata.co.za/data/downloads#south-africa-claude-usage) · [the story](https://mzansidata.co.za/posts/how-south-africans-use-claude) | [mzansidata-south-africa-claude-usage-2026.11.4](https://archive.org/details/mzansidata-south-africa-claude-usage-2026.11.4) | [kaggle.com/datasets/elroyparkinson/south-africa-claude-usage](https://www.kaggle.com/datasets/elroyparkinson/south-africa-claude-usage) |
| `south-africa-population-2002-2026` | [Downloads](https://mzansidata.co.za/data/downloads#south-africa-population-2002-2026) | [mzansidata-south-africa-population-2002-2026-2026.11.4](https://archive.org/details/mzansidata-south-africa-population-2002-2026-2026.11.4) | [kaggle.com/datasets/elroyparkinson/south-africa-population-2002-2026](https://www.kaggle.com/datasets/elroyparkinson/south-africa-population-2002-2026) |
| `south-africa-crime-victims-survey-2018-2026` | [Downloads](https://mzansidata.co.za/data/downloads#south-africa-crime-victims-survey-2018-2026) · [the story](https://mzansidata.co.za/posts/crime-long-term) | [mzansidata-south-africa-crime-victims-survey-2018-2026-2026.11.4](https://archive.org/details/mzansidata-south-africa-crime-victims-survey-2018-2026-2026.11.4) | [kaggle.com/datasets/elroyparkinson/south-africa-crime-victims-survey-2018-2026](https://www.kaggle.com/datasets/elroyparkinson/south-africa-crime-victims-survey-2018-2026) |
| `south-africa-unemployment-qlfs` | [Downloads](https://mzansidata.co.za/data/downloads#south-africa-unemployment-qlfs) · [latest figures](https://mzansidata.co.za/topics/economy#unemployment) | [mzansidata-south-africa-unemployment-qlfs-2026.11.4](https://archive.org/details/mzansidata-south-africa-unemployment-qlfs-2026.11.4) | [kaggle.com/datasets/elroyparkinson/south-africa-unemployment-qlfs](https://www.kaggle.com/datasets/elroyparkinson/south-africa-unemployment-qlfs) |
| `south-africa-inflation-cpi` | [Downloads](https://mzansidata.co.za/data/downloads#south-africa-inflation-cpi) · [latest figures](https://mzansidata.co.za/topics/economy#inflation) · [inflation since 1922](https://mzansidata.co.za/posts/inflation-since-1922) | [mzansidata-south-africa-inflation-cpi-2026.11.4](https://archive.org/details/mzansidata-south-africa-inflation-cpi-2026.11.4) | [kaggle.com/datasets/elroyparkinson/south-africa-inflation-cpi](https://www.kaggle.com/datasets/elroyparkinson/south-africa-inflation-cpi) |

Charts and explainers built on these tables: https://mzansidata.co.za.

## Election results

Not here. The Electoral Commission's copyright notice allows its material to be reproduced "in unaltered form only for personal, non-commercial use", so we do not republish its files or tables made from them.

## Versions

Versions are named `year.month.n`; `2026.11.0` is the first. Files never change within a version.

## Corrections

Found a figure that differs from the publisher's file? Write to hello@mzansidata.co.za or use https://mzansidata.co.za/contact, naming the file, the row and the publisher's file you compared it with.

MzansiData's own documentation here is CC BY 4.0. The data in each package is under the terms that package gives.
