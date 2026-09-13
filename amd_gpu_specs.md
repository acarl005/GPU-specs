# AMD GPU Specifications

Master reference table of AMD GPUs spanning GCN 1 through RDNA 4 / CDNA 3, analogous to the NVIDIA specification table, with AMD's own terminology mapped onto the closest NVIDIA-equivalent concepts.

## Column mapping (NVIDIA → AMD)

| NVIDIA concept | AMD analog | Notes |
|---|---|---|
| CUDA Cores | Stream Processors | Same idea — ALU count |
| SM (Streaming Multiprocessor) | Compute Unit (CU) | RDNA 3/4 pair two CUs into a Workgroup Processor (WGP); CU count is listed as the primary unit |
| Compute Capability | `gfx` ISA target (e.g. `gfx1100`) | The actual ROCm/LLVM compilation target — closest functional equivalent. Architecture family (GCN/RDNA/CDNA generation) is a separate column since `gfx` numbering isn't as cleanly sequential as NVIDIA's |
| Max Threads/SM | Max Threads/CU | Computed as wavefront size × architectural max resident wavefronts/CU |
| Max Blocks/SM | *(omitted)* | AMD doesn't publish a fixed hardware ceiling on concurrent workgroups per CU the way NVIDIA does for blocks/SM — it's resource-dependent, so including a number here would imply false precision |
| Max Shared Mem/SM | LDS/CU | Local Data Share, AMD's shared-memory equivalent |

## AMD GPU specification table

| Year | Card | Architecture | gfx ISA | Stream Processors | Compute Units | Memory | Max Threads/CU | LDS/CU | Peak FP32 TFLOPS | Mem Bandwidth | L2 Cache (+Infinity Cache) | Mem Bus & Type | TDP |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 2011 | HD 7970 | GCN 1 | gfx600 | 2,048 | 32 | 3 GB | 2,560 | 64 KB | 3.79 | 264 GB/s | 768 KB | 384-bit GDDR5 | 250 W |
| 2013 | R9 290X | GCN 2 | gfx702 | 2,816 | 44 | 4 GB | 2,560 | 64 KB | 5.6 | 320 GB/s | 1 MB | 512-bit GDDR5 | 290 W |
| 2015 | R9 Fury X | GCN 3 | gfx803 | 4,096 | 64 | 4 GB HBM1 | 2,560 | 64 KB | 8.6 | 512 GB/s | 2 MB | 4096-bit HBM1 | 275 W |
| 2016 | RX 480 | GCN 4 | gfx803 | 2,304 | 36 | 8 GB | 2,560 | 64 KB | 5.8 | 256 GB/s | 2 MB | 256-bit GDDR5 | 150 W |
| 2017 | RX 580 | GCN 4 | gfx803 | 2,304 | 36 | 8 GB | 2,560 | 64 KB | 6.17 | 256 GB/s | 2 MB | 256-bit GDDR5 | 185 W |
| 2017 | Vega 56 | GCN 5 | gfx900 | 3,584 | 56 | 8 GB HBM2 | 2,560 | 64 KB | 10.5 | 410 GB/s | 4 MB | 2048-bit HBM2 | 210 W |
| 2017 | Vega 64 | GCN 5 | gfx900 | 4,096 | 64 | 8 GB HBM2 | 2,560 | 64 KB | 12.66 | 484 GB/s | 4 MB | 2048-bit HBM2 | 295 W |
| 2019 | Radeon VII | GCN 5.1 | gfx906 | 3,840 | 60 | 16 GB HBM2 | 2,560 | 64 KB | 13.8 | 1,024 GB/s | 4 MB | 4096-bit HBM2 | 300 W |
| 2020 | Instinct MI100 | CDNA 1 | gfx908 | 7,680 | 120 | 32 GB HBM2 | 2,560 | 64 KB | 23.1 (vector) | 1.2 TB/s | 8 MB | 4096-bit HBM2 | 300 W |
| 2019 | RX 5700 | RDNA 1 | gfx1010 | 2,304 | 36 | 8 GB | 1,280 | 128 KB/WGP | 7.95 | 448 GB/s | 4 MB | 256-bit GDDR6 | 180 W |
| 2019 | RX 5700 XT | RDNA 1 | gfx1010 | 2,560 | 40 | 8 GB | 1,280 | 128 KB/WGP | 9.75 | 448 GB/s | 4 MB | 256-bit GDDR6 | 225 W |
| 2022 | Instinct MI210 | CDNA 2 | gfx90a | 6,656 | 104 | 64 GB HBM2e | 2,048 | 64 KB | 22.6 (vector) | 1.6 TB/s | 8 MB | 4096-bit HBM2e | 300 W |
| 2021 | Instinct MI250 | CDNA 2 | gfx90a | 13,312 | 208 | 128 GB HBM2e | 2,048 | 64 KB | 45.3 (vector) | 3.2 TB/s | 16 MB | 8192-bit HBM2e | 500 W |
| 2021 | Instinct MI250X | CDNA 2 | gfx90a | 14,080 | 220 | 128 GB HBM2e | 2,048 | 64 KB | 47.9 (vector) | 3.2 TB/s | 16 MB | 8192-bit HBM2e | 560 W |
| 2021 | RX 6600 | RDNA 2 | gfx1032 | 1,792 | 28 | 8 GB | 1,280 | 128 KB/WGP | 8.93 | 224 GB/s | 2 MB (+32 MB) | 128-bit GDDR6 | 132 W |
| 2021 | RX 6600 XT | RDNA 2 | gfx1032 | 2,048 | 32 | 8 GB | 1,280 | 128 KB/WGP | 10.6 | 256 GB/s | 2 MB (+32 MB) | 128-bit GDDR6 | 160 W |
| 2021 | RX 6700 XT | RDNA 2 | gfx1031 | 2,560 | 40 | 12 GB | 1,280 | 128 KB/WGP | 13.2 | 384 GB/s | 3 MB (+96 MB) | 192-bit GDDR6 | 230 W |
| 2020 | RX 6800 | RDNA 2 | gfx1030 | 3,840 | 60 | 16 GB | 1,280 | 128 KB/WGP | 16.2 | 512 GB/s | 4 MB (+128 MB) | 256-bit GDDR6 | 250 W |
| 2020 | RX 6800 XT | RDNA 2 | gfx1030 | 4,608 | 72 | 16 GB | 1,280 | 128 KB/WGP | 20.7 | 512 GB/s | 4 MB (+128 MB) | 256-bit GDDR6 | 300 W |
| 2020 | RX 6900 XT | RDNA 2 | gfx1030 | 5,120 | 80 | 16 GB | 1,280 | 128 KB/WGP | 23.04 | 512 GB/s | 4 MB (+128 MB) | 256-bit GDDR6 | 300 W |
| 2022 | RX 6950 XT | RDNA 2 | gfx1030 | 5,120 | 80 | 16 GB | 1,280 | 128 KB/WGP | 23.7 | 576 GB/s | 4 MB (+128 MB) | 256-bit GDDR6 | 335 W |
| 2023 | RX 7600 | RDNA 3 | gfx1102 | 2,048 | 32 | 8 GB | 1,280 | 128 KB/WGP | 21.75 | 288 GB/s | 2 MB (+32 MB) | 128-bit GDDR6 | 165 W |
| 2023 | RX 7700 XT | RDNA 3 | gfx1101 | 3,456 | 54 | 12 GB | 1,280 | 128 KB/WGP | 35.2 | 432 GB/s | 2 MB (+48 MB) | 192-bit GDDR6 | 245 W |
| 2023 | RX 7800 XT | RDNA 3 | gfx1101 | 3,840 | 60 | 16 GB | 1,280 | 128 KB/WGP | 37.3 | 624 GB/s | 4 MB (+64 MB) | 256-bit GDDR6 | 263 W |
| 2023 | RX 7900 GRE | RDNA 3 | gfx1100 | 5,120 | 80 | 16 GB | 1,280 | 128 KB/WGP | 46.0 | 576 GB/s | 6 MB (+64 MB) | 256-bit GDDR6 | 260 W |
| 2022 | RX 7900 XT | RDNA 3 | gfx1100 | 5,376 | 84 | 20 GB | 1,280 | 128 KB/WGP | 51.6 | 800 GB/s | 6 MB (+80 MB) | 320-bit GDDR6 | 315 W |
| 2022 | RX 7900 XTX | RDNA 3 | gfx1100 | 6,144 | 96 | 24 GB | 1,280 | 128 KB/WGP | 61.4 | 960 GB/s | 6 MB (+96 MB) | 384-bit GDDR6 | 355 W |
| 2023 | Instinct MI300X | CDNA 3 | gfx942 | 19,456 | 304 | 192 GB HBM3 | 2,048* | 64 KB | 163.4 | 5.3 TB/s | 32 MB (+256 MB) | 8192-bit HBM3 | 750 W |
| 2025 | RX 9060 XT | RDNA 4 | gfx1200 | 2,048 | 32 | 8/16 GB | 1,280 | 128 KB/WGP | 25.6 | 320 GB/s | 4 MB (+32 MB) | 128-bit GDDR6 | 150/160 W |
| 2025 | RX 9070 | RDNA 4 | gfx1201 | 3,584 | 56 | 16 GB | 1,280 | 128 KB/WGP | 36.1 | 640 GB/s | 8 MB (+64 MB) | 256-bit GDDR6 | 220 W |
| 2025 | RX 9070 XT | RDNA 4 | gfx1201 | 4,096 | 64 | 16 GB | 1,280 | 128 KB/WGP | 48.7 | 640 GB/s | 8 MB (+64 MB) | 256-bit GDDR6 | 304 W |

## Methodology notes

- **Max Threads/CU** = wavefront size (64 for GCN/CDNA; wave32 or wave64, selectable, for RDNA) × architectural max resident wavefronts/CU. GCN/CDNA1 hold 40 wavefronts/CU (4 SIMD16 × 10 wave slots); CDNA2 drops to 32 (4×8) per AMD's own ROCm docs. RDNA's WGP holds 4×20 wave32 slots = 80 wave32-equivalents per WGP, i.e. 1,280 per CU. Treat these as architectural ceilings, not typical achieved occupancy.
- **LDS/CU**: GCN/CDNA have a fixed 64 KB LDS per CU. RDNA's LDS is physically 128 KB per WGP (shared across its 2 CUs) — listed as such rather than divided in half, since a single workgroup can use the full 128 KB.
- **CDNA "Peak FP32 (vector)"** is explicitly labeled because AMD's data-center parts have separate, much higher "matrix FP32" figures on CDNA2 (e.g., MI250X: 47.9 TFLOPS vector vs 95.7 TFLOPS matrix). CDNA3 (MI300X) unified these into a single 163.4 TFLOPS figure per AMD's own datasheet.
- **Instinct MI300X (CDNA 3) Max Threads/CU is marked uncertain (`2,048*`)** — this carries over CDNA2's 32-waveslots/CU occupancy model, but AMD hasn't published CDNA3's waveslot count explicitly; some GFX9-family guides suggest CDNA3 may retain the 40-waveslots/CU (2,560) model used by GCN/CDNA1 instead. Treat as unconfirmed pending an authoritative source.
- RDNA4 TFLOPS/Mem Bandwidth/TDP figures (RX 9060 XT/9070/9070 XT) have been verified against AMD's official product pages; RX 9060 XT's TDP differs by memory configuration (150 W for 8GB, 160 W for 16GB).
- All other figures are sourced from AMD's official product pages/datasheets (amd.com), AMD's ROCm GPU hardware specification docs, and cross-checked GPU databases.
