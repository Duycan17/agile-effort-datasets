# Agile effort datasets

Three datasets used for research on software effort estimation. The CSV files are provided as separate datasets because they have different targets and schemas.

| Directory | Files | Rows | Target | Description |
| --- | ---: | ---: | --- | --- |
| [`choet/`](choet/) | 16 CSVs | 23,313 | `storypoint` | One file per project; includes the original `split_mark` column. |
| [`ages/`](ages/) | 1 CSV | 23,006 | `Time Taken (days)` | Raw AgES issue records. |
| [`tawos/`](tawos/) | 1 CSV | 43,732 | `story_point` | Prepared TAWOS data for prediction at estimation time. |

Rows are counted excluding the CSV header. File hashes are listed in [`SHA256SUMS`](SHA256SUMS).
