# Participant interaction logs

- [Baseline](baseline/): 32 participant folders.
- [System](system/): 32 participant folders.

Each participant folder contains `log.csv` and `intent.txt`. The text file includes the initial shopping purpose from the session metadata and all recorded prompt_submitted inputs in event order. When no prompt submission was logged, this is stated explicitly.

Original participant IDs P01–P64 are preserved to match the [image archive](https://github.com/yugyeongjang/recontextualization/tree/d5a0def75ba48c5b42ec0399082d2f44093a6348/results/images/); IDs are not renumbered within conditions. System IDs match the 32 participants with generated images and generation-result events. The remaining sessions are classified as baseline. Source CSVs do not contain an explicit condition column; labels are recovered from generation events and the image archive.

All 5,699 interaction events are retained. Names and session UUIDs are removed or replaced. Absolute timestamps are replaced with elapsed_seconds from the first event; event_order starts at zero. Generated-image local paths are reduced to filenames. Emails, if present, are redacted. CSVs use UTF-8 with BOM and details_json contains the structured event payload.

These are interaction logs, not questionnaire or statistical-analysis datasets.

## Source

Copied from [yugyeongjang/recontextualization](https://github.com/yugyeongjang/recontextualization/tree/d5a0def75ba48c5b42ec0399082d2f44093a6348/results/logs/) (commit `d5a0def75ba48c5b42ec0399082d2f44093a6348`). Participant intent files and CSV logs are unchanged. Only the logs folder is included here; the image archive and implementation remain in the source repository.
