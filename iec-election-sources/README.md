# IEC election results: source catalogue

The Electoral Commission of South Africa (IEC) results files that MzansiData's election charts use: 172 files, each with its address on the IEC's results site, the date MzansiData retrieved it, its size, its SHA-256 checksum, and how many of MzansiData's checks were made against it. The same list is on https://mzansidata.co.za/data/elections/sources.

This catalogue holds no IEC figures and none of the IEC's files. The IEC's copyright notice (https://www.elections.org.za/pw/Copyright-Notice, read 7 November 2026) allows its material to be reproduced "in unaltered form only for personal, non-commercial use", so get the files from the IEC, under the IEC's terms, starting at https://www.elections.org.za/. Clause 2.9 of the IEC's website terms (https://www.elections.org.za/pw/Disclaimer) rules out using any technology "to search or copy content" from its website without the IEC's written consent, so there is no download script here.

Checks: last run 2026-11-07T23:03:12: 1722 checks, 1722 passed, 0 failed. MzansiData reads the figures from the IEC's Excel reports and checks each against the PDF of the same report or the IEC's results dashboard files.

## sources.csv

| Column | Meaning |
|---|---|
| `file_key` | MzansiData's name for the file |
| `title` | What the file holds (MzansiData's description) |
| `url` | Where the IEC publishes it |
| `retrieved` | Date MzansiData downloaded it |
| `bytes` | Size of the file MzansiData downloaded |
| `sha256` | SHA-256 of that file, so you can check your copy |
| `checks_against_file` | Number of MzansiData's checks made against this file |
| `checks_passed` | How many of them passed |

The catalogue itself (this README and sources.csv) is CC BY 4.0, MzansiData.
