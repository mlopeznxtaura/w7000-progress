# Goal

Run on CASEBELIZE's two AMD FirePro W7000 4 GB GPUs:

1. A Vulkan path-tracer kernel.
2. A small 4-bit quantized app18 model.

## Hard constraints

- **GPU 0 and GPU 2 only. Never use GPU 1.** Select devices explicitly by index in every run, and never rely on the default device.
- 4 GB VRAM per card. Workloads must fit per card, including the model weights, KV/cache, and scratch buffers.
- Record the GPU index used in every daily log entry.

## Done when

- [ ] The path-tracer kernel runs on GPU 0 and GPU 2 (Vulkan) and produces correct output
- [ ] The 4-bit app18 model loads and runs inference within 4 GB on GPU 0 and/or GPU 2
- [ ] The daily collector on the Dell records results every day at 03:17
