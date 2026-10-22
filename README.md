# Texas assessment data

STAAR and TELPAS results from the [Texas Assessment Research Portal](https://txresearchportal.com):
state, the 20 ESC regions, every district and every campus, by student group.

The data lives in this repo's **Releases**, not in git: one parquet per level x program,
the raw portal CSVs as `.tar.gz` (the source of record), and a `manifest.csv` with each
file's size, SHA-256 and row count. Built and validated by `R/19`-`R/21` in
`statewide-peims-explorer`.

Values for 1-4 testers are suppressed by the portal (`value` NA, `is_suppressed` TRUE);
never read them as 0.

Download a release: `gh release download <tag> --repo mrworthington/texas-assessment-data`
