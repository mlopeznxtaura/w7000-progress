# Daily collector plan (Dell / casebelizelinux, 03:17 daily)

The Dell (`casebelizelinux`) runs a collector every day at **03:17** local time.

## Plan

1. At 03:17, gather the previous day's results from the W7000 runs on CASEBELIZE (GPU 0 and GPU 2 only):
   - path-tracer kernel runs (status, timing, output check)
   - 4-bit app18 model runs (load status, VRAM used, tokens/sec)
2. Write a dated summary entry for `progress/daily-log.md`.
3. Commit the entry to this repo.

## Rules

- Never collect or commit secrets, tokens, `owncode`, or `config.yaml`.
- Flag any run that touched GPU 1 as an error.

Example schedule entry (cron): `17 3 * * * <collector command>`
