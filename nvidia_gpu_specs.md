# NVIDIA GPU Specifications

Master reference table of NVIDIA GPUs spanning Kepler through Blackwell, including compute-capability architectural limits, peak throughput, and memory subsystem details.

## Master GPU specification table

| Year | Card | Architecture | CC | CUDA Cores | SMs | Memory | Max Threads/SM | Max Blocks/SM | Max Shared Mem/SM | Peak FP32 TFLOPS | Mem Bandwidth | L2 Cache | Mem Bus & Type | TDP |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 2012 | GTX 680 | Kepler | 3.0 | 1,536 | 8 | 2 GB | 2,048 | 16 | 48 KB | 3.25 | 192 GB/s | 512 KB | 256-bit GDDR5 | 195 W |
| 2013 | GTX 780 | Kepler | 3.5 | 2,304 | 12 | 3 GB | 2,048 | 16 | 48 KB | 4.16 | 288 GB/s | 1.5 MB | 384-bit GDDR5 | 250 W |
| 2013 | GTX 780 Ti | Kepler | 3.5 | 2,880 | 15 | 3 GB | 2,048 | 16 | 48 KB | 5.35 | 336 GB/s | 1.5 MB | 384-bit GDDR5 | 250 W |
| 2014 | GTX Titan Black | Kepler | 3.5 | 2,880 | 15 | 6 GB | 2,048 | 16 | 48 KB | 5.65 | 336 GB/s | 1.5 MB | 384-bit GDDR5 | 250 W |
| 2014 | GTX 970 | Maxwell | 5.2 | 1,664 | 13 | 4 GB | 2,048 | 32 | 96 KB | 3.92 | 196 GB/s | 1.75 MB | 224-bit GDDR5 | 145 W |
| 2014 | GTX 980 | Maxwell | 5.2 | 2,048 | 16 | 4 GB | 2,048 | 32 | 96 KB | 4.98 | 224 GB/s | 2 MB | 256-bit GDDR5 | 165 W |
| 2015 | GTX 980 Ti | Maxwell | 5.2 | 2,816 | 22 | 6 GB | 2,048 | 32 | 96 KB | 6.06 | 336 GB/s | 3 MB | 384-bit GDDR5 | 250 W |
| 2015 | GTX Titan X | Maxwell | 5.2 | 3,072 | 24 | 12 GB | 2,048 | 32 | 96 KB | 6.60 | 336 GB/s | 3 MB | 384-bit GDDR5 | 250 W |
| 2016 | Tesla P100 | Pascal | 6.0 | 3,584 | 56 | 16 GB HBM2 | 2,048 | 32 | 64 KB | ~10.6 | 732 GB/s | 4 MB | 4096-bit HBM2 | 300 W |
| 2016 | GTX 1060 | Pascal | 6.1 | 1,152–1,280 | 9–10 | 3/6 GB | 2,048 | 32 | 96 KB | 4.37 | 192 GB/s | 1.5 MB | 192-bit GDDR5 | 120 W |
| 2016 | GTX 1070 | Pascal | 6.1 | 1,920 | 15 | 8 GB | 2,048 | 32 | 96 KB | 6.46 | 256 GB/s | 2 MB | 256-bit GDDR5 | 150 W |
| 2017 | GTX 1070 Ti | Pascal | 6.1 | 2,432 | 19 | 8 GB | 2,048 | 32 | 96 KB | 8.19 | 256 GB/s | 2 MB | 256-bit GDDR5 | 180 W |
| 2016 | GTX 1080 | Pascal | 6.1 | 2,560 | 20 | 8 GB | 2,048 | 32 | 96 KB | 8.87 | 320 GB/s | 2 MB | 256-bit GDDR5X | 180 W |
| 2017 | GTX 1080 Ti | Pascal | 6.1 | 3,584 | 28 | 11 GB | 2,048 | 32 | 96 KB | 11.34 | 484 GB/s | 2.75 MB | 352-bit GDDR5X | 250 W |
| 2017 | Tesla V100 | Volta | 7.0 | 5,120 | 80 | 16/32 GB HBM2 | 2,048 | 32 | 96 KB | 14–15 | 900 GB/s | 6 MB | 4096-bit HBM2 | 300/350 W |
| 2019 | RTX 2060 | Turing | 7.5 | 1,920 | 30 | 6 GB | 1,024 | 16 | 64 KB | 6.45 | 336 GB/s | 3 MB | 192-bit GDDR6 | 160 W |
| 2019 | RTX 2060 Super | Turing | 7.5 | 2,176 | 34 | 8 GB | 1,024 | 16 | 64 KB | 7.18 | 448 GB/s | 4 MB | 256-bit GDDR6 | 175 W |
| 2018 | RTX 2070 | Turing | 7.5 | 2,304 | 36 | 8 GB | 1,024 | 16 | 64 KB | 7.46 | 448 GB/s | 4 MB | 256-bit GDDR6 | 175 W |
| 2019 | RTX 2070 Super | Turing | 7.5 | 2,560 | 40 | 8 GB | 1,024 | 16 | 64 KB | 9.06 | 448 GB/s | 4 MB | 256-bit GDDR6 | 215 W |
| 2018 | RTX 2080 | Turing | 7.5 | 2,944 | 46 | 8 GB | 1,024 | 16 | 64 KB | 10.07 | 448 GB/s | 4 MB | 256-bit GDDR6 | 215 W |
| 2019 | RTX 2080 Super | Turing | 7.5 | 3,072 | 48 | 8 GB | 1,024 | 16 | 64 KB | 11.15 | 496 GB/s | 4 MB | 256-bit GDDR6 | 250 W |
| 2018 | RTX 2080 Ti | Turing | 7.5 | 4,352 | 68 | 11 GB | 1,024 | 16 | 64 KB | 13.45 | 616 GB/s | 5.5 MB | 352-bit GDDR6 | 250 W |
| 2020 | A100 | Ampere | 8.0 | 6,912 | 108 | 40 GB HBM2 / 80 GB HBM2e | 2,048 | 32 | 164 KB | 19.5 | 1,555–2,039 GB/s | 40 MB | 5120-bit HBM2/HBM2e | 250/300/400 W |
| 2021 | RTX 3060 | Ampere | 8.6 | 3,584 | 28 | 12 GB | 1,536 | 16 | 100 KB | 12.74 | 360 GB/s | 3 MB | 192-bit GDDR6 | 170 W |
| 2020 | RTX 3060 Ti | Ampere | 8.6 | 4,864 | 38 | 8 GB | 1,536 | 16 | 100 KB | 16.20 | 448 GB/s | 4 MB | 256-bit GDDR6 | 200 W |
| 2020 | RTX 3070 | Ampere | 8.6 | 5,888 | 46 | 8 GB | 1,536 | 16 | 100 KB | 20.31 | 448 GB/s | 4 MB | 256-bit GDDR6 | 220 W |
| 2021 | RTX 3070 Ti | Ampere | 8.6 | 6,144 | 48 | 8 GB | 1,536 | 16 | 100 KB | 21.75 | 608 GB/s | 4 MB | 256-bit GDDR6X | 290 W |
| 2020 | RTX 3080 (10GB) | Ampere | 8.6 | 8,704 | 68 | 10 GB | 1,536 | 16 | 100 KB | 29.77 | 760 GB/s | 5 MB | 320-bit GDDR6X | 320 W |
| 2021 | RTX 3080 (12GB) | Ampere | 8.6 | 8,960 | 70 | 12 GB | 1,536 | 16 | 100 KB | 30.65 | 912 GB/s | 6 MB | 384-bit GDDR6X | 350 W |
| 2021 | RTX 3080 Ti | Ampere | 8.6 | 10,240 | 80 | 12 GB | 1,536 | 16 | 100 KB | 34.10 | 912 GB/s | 6 MB | 384-bit GDDR6X | 350 W |
| 2020 | RTX 3090 | Ampere | 8.6 | 10,496 | 82 | 24 GB | 1,536 | 16 | 100 KB | 35.58 | 936 GB/s | 6 MB | 384-bit GDDR6X | 350 W |
| 2022 | RTX 3090 Ti | Ampere | 8.6 | 10,752 | 84 | 24 GB | 1,536 | 16 | 100 KB | 40.00 | 1,008 GB/s | 6 MB | 384-bit GDDR6X | 450 W |
| 2023 | RTX 4060 | Ada Lovelace | 8.9 | 3,072 | 24 | 8 GB | 1,536 | 24 | 100 KB | 15.11 | 272 GB/s | 24 MB | 128-bit GDDR6 | 115 W |
| 2023 | RTX 4060 Ti | Ada Lovelace | 8.9 | 4,352 | 34 | 8/16 GB | 1,536 | 24 | 100 KB | 22.06 | 288 GB/s | 32 MB | 128-bit GDDR6 | 160 W |
| 2023 | RTX 4070 | Ada Lovelace | 8.9 | 5,888 | 46 | 12 GB | 1,536 | 24 | 100 KB | 29.15 | 504 GB/s | 36 MB | 192-bit GDDR6X | 200 W |
| 2024 | RTX 4070 Super | Ada Lovelace | 8.9 | 7,168 | 56 | 12 GB | 1,536 | 24 | 100 KB | 35.48 | 504 GB/s | 48 MB | 192-bit GDDR6X | 220 W |
| 2023 | RTX 4070 Ti | Ada Lovelace | 8.9 | 7,680 | 60 | 12 GB | 1,536 | 24 | 100 KB | 40.09 | 504 GB/s | 48 MB | 192-bit GDDR6X | 285 W |
| 2024 | RTX 4070 Ti Super | Ada Lovelace | 8.9 | 8,448 | 66 | 16 GB | 1,536 | 24 | 100 KB | 44.10 | 672 GB/s | 48 MB | 256-bit GDDR6X | 285 W |
| 2022 | RTX 4080 | Ada Lovelace | 8.9 | 9,728 | 76 | 16 GB | 1,536 | 24 | 100 KB | 48.74 | 717 GB/s | 64 MB | 256-bit GDDR6X | 320 W |
| 2024 | RTX 4080 Super | Ada Lovelace | 8.9 | 10,240 | 80 | 16 GB | 1,536 | 24 | 100 KB | 52.22 | 736 GB/s | 64 MB | 256-bit GDDR6X | 320 W |
| 2022 | RTX 4090 | Ada Lovelace | 8.9 | 16,384 | 128 | 24 GB | 1,536 | 24 | 100 KB | 82.58 | 1,008 GB/s | 72 MB | 384-bit GDDR6X | 450 W |
| 2022 | H100 (SXM) | Hopper | 9.0 | 16,896 | 132 | 80 GB HBM3 | 2,048 | 32 | 228 KB | 67 | 3,350 GB/s | 50 MB | 5120-bit HBM3 | 700 W |
| 2024/25 | B200 | Blackwell | 10.0 | ~16,896–18,432* | ~132–148* | 180–192 GB HBM3e | 2,048 | 32 | 228 KB | ~62–90* | ~4,100–8,000 GB/s* | ~50–96 MB* (NVIDIA cites 126 MB for GB200) | 4096/8192-bit HBM3e* | 1,000 W |
| 2025 | RTX 5060 | Blackwell | 12.0 | 3,840 | 30 | 8 GB | 1,536 | 32 | 128 KB | 19.18 | 448 GB/s | 32 MB | 128-bit GDDR7 | 145 W |
| 2025 | RTX 5060 Ti | Blackwell | 12.0 | 4,608 | 36 | 8/16 GB | 1,536 | 32 | 128 KB | 23.70 | 448 GB/s | 32 MB | 128-bit GDDR7 | 180 W |
| 2025 | RTX 5070 | Blackwell | 12.0 | 6,144 | 48 | 12 GB | 1,536 | 32 | 128 KB | 30.87 | 672 GB/s | 48 MB | 192-bit GDDR7 | 250 W |
| 2025 | RTX 5070 Ti | Blackwell | 12.0 | 8,960 | 70 | 16 GB | 1,536 | 32 | 128 KB | 43.95 | 896 GB/s | 48 MB | 256-bit GDDR7 | 300 W |
| 2025 | RTX 5080 | Blackwell | 12.0 | 10,752 | 84 | 16 GB | 1,536 | 32 | 128 KB | 56.29 | 960 GB/s | 64 MB | 256-bit GDDR7 | 360 W |
| 2025 | RTX 5090 | Blackwell | 12.0 | 21,760 | 170 | 32 GB | 1,536 | 32 | 128 KB | 104.75 | 1,792 GB/s | 96 MB | 512-bit GDDR7 | 575 W |

## Methodology notes

- **Peak FP32 TFLOPS** is computed as `2 × CUDA cores × boost clock (GHz)` for consumer cards (the standard formula, verified against several official NVIDIA figures where available, e.g. RTX 4090 = 82.6, RTX 2080 Ti = 13.4). Data-center cards (V100/A100/H100) use NVIDIA's directly published figures.
- **B200 row is marked uncertain throughout** — NVIDIA hasn't published an authoritative core/SM/cache breakdown, and third-party sources conflict (some report a 132-SM/50MB-L2/4.1TB/s config, others a 148-SM/96MB-L2/8TB/s config, possibly reflecting different B100/B200/B200A variants or memory configs). Treat this row as a placeholder pending an authoritative source.
- All other figures are sourced from NVIDIA whitepapers, official spec/datasheet pages, and cross-checked GPU databases.
- Registers per SM are 65,536 (32-bit) across every row in this table.
- Max Threads/Block is 1,024 across every row in this table (omitted as a column since it never varies).

## Compute capability legend

| CC | Architecture family |
|---|---|
| 3.0 / 3.5 | Kepler |
| 5.2 | Maxwell |
| 6.0 / 6.1 | Pascal |
| 7.0 | Volta |
| 7.5 | Turing |
| 8.0 | Ampere (data center) |
| 8.6 | Ampere (consumer/professional) |
| 8.9 | Ada Lovelace |
| 9.0 | Hopper |
| 10.0 | Blackwell (data center) |
| 12.0 | Blackwell (consumer) |
