# Agile effort datasets

Three datasets used for research on software effort estimation. The CSV files are provided as separate datasets because they have different targets and schemas.

| Directory | Files | Rows | Target | Description |
| --- | ---: | ---: | --- | --- |
| [`choet/`](choet/) | 16 CSVs | 23,313 | `storypoint` | One file per project; includes the original `split_mark` column. |
| [`ages/`](ages/) | 1 CSV | 23,006 | `Time Taken (days)` | Raw AgES issue records. |
| [`tawos/`](tawos/) | 1 CSV | 43,732 | `story_point` | Prepared TAWOS data for prediction at estimation time. |

Rows are counted excluding the CSV header. File hashes are listed in [`SHA256SUMS`](SHA256SUMS).

## Provenance

- **CHOET:** The 16 project CSVs were copied from the [GPT2SP `marked_data` collection](https://github.com/awsm-research/gpt2sp/tree/main/sp_dataset/marked_data), which credits the Deep-SE dataset developers. The five columns are `issuekey`, `title`, `description`, `storypoint`, and `split_mark`.
- **AgES:** `Raw_AgES_Dataset.csv` was copied from the local `Agile/ages_repro/ref/` research project. It contains 15 columns, including issue text and effort measured in days. The original distribution and reuse terms have not been verified here.
- **TAWOS:** `tawos_storypoint_pre_estimation_dataset.csv` was copied from the local `Agile/ages_repro/data/` research project. It is a prepared export derived from the [TAWOS dataset](https://doi.org/10.5522/04/21308124), with 33 columns. The source dataset's terms and Apache License 2.0 are described by the [TAWOS project](https://github.com/SOLAR-group/TAWOS).

This repository does not assign a new blanket license to third-party data. Consult each source's terms before reuse. In particular, the AgES source terms should be checked independently.
