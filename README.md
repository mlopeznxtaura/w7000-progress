# w7000-progress

Progress tracking for running GPU compute workloads on **CASEBELIZE**'s two AMD FirePro W7000 (4 GB) cards.

> Note: this repo was `git init`-ed on Oct 8, 2026 but had no files or commits. The files below were written on
> Oct 8, 2026 from the planned description of the project, so they are new rather than restored.

## Goal

- Run a **Vulkan path-tracer kernel** on the W7000s.
- Run a **small 4-bit quantized app18 model** on the W7000s.
- Use **GPU 0 and GPU 2 only. Never use GPU 1.**
- Each card has 4 GB of VRAM, so every workload must fit within 4 GB per GPU.

## Layout

- `GOAL.md`: goal and hard constraints
- `COLLECTOR_PLAN.md`: the Dell's (casebelizelinux) daily 03:17 collector plan
- `progress/daily-log.md`: daily log, one entry per day

## Never committed

- No file named `owncode` or `config.yaml`
- No secrets, tokens, keys, or credentials (see `.gitignore`)
