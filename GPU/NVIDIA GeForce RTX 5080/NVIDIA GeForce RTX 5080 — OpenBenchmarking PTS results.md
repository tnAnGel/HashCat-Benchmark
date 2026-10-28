# NVIDIA GeForce RTX 5080 — OpenBenchmarking Hashcat measurements (partial, no stdout)

- **Evidence:** PTS-published individual benchmark values; no raw Hashcat console stdout is available from these result exports.
- **PTS runner:** profile executes `hashcat -b --benchmark-min=30` with the per-mode arguments below.
- **Values:** exact PTS mean in H/s and exact repeat values when PTS publishes them. A PTS repeat is not a copied `Speed.#N` console line.
- **Hardware:** exact PTS graphics descriptor is kept per row; aliases are explained in the note below.

| Date | Hashcat | Mode | Benchmark | Mean (H/s) | Readable speed | PTS repeat values (H/s) | PTS GPU label | CPU host context | Args | Result |
|---|---|---:|---|---:|---:|---|---|---|---|---|
| 2026-08-14 | 7.1.2 | 1000 | Benchmark: NTLM | 196733333333 | 196.7 GH/s | 196600000000, 196800000000, 196800000000 | Gigabyte NVIDIA GeForce RTX 5080 16GB | AMD Ryzen 9 9950X3D2 16-Core @ 5.67GHz (16 Cores / 32 Threads) | `-m 1000` | [2608130-NE-SUPERCOMP73](https://openbenchmarking.org/result/2608130-NE-SUPERCOMP73) |
| 2026-08-14 | 7.1.2 | 1700 | Benchmark: SHA-512 | 4982033333 | 4.982 GH/s | 4986200000, 4981200000, 4978700000 | Gigabyte NVIDIA GeForce RTX 5080 16GB | AMD Ryzen 9 9950X3D2 16-Core @ 5.67GHz (16 Cores / 32 Threads) | `-m 1700` | [2608130-NE-SUPERCOMP73](https://openbenchmarking.org/result/2608130-NE-SUPERCOMP73) |
| 2026-08-19 | 7.1.2 | 1000 | Benchmark: NTLM | 195466666667 | 195.5 GH/s | 195700000000, 195000000000, 195700000000 | Gigabyte NVIDIA GeForce RTX 5080 16GB | AMD Ryzen 9 9950X3D2 16-Core @ 5.67GHz (16 Cores / 32 Threads) | `-m 1000` | [2608193-NE-SUPERCOMP30](https://openbenchmarking.org/result/2608193-NE-SUPERCOMP30) |
| 2026-08-19 | 7.1.2 | 1700 | Benchmark: SHA-512 | 4967166667 | 4.967 GH/s | 4964900000, 4968800000, 4967800000 | Gigabyte NVIDIA GeForce RTX 5080 16GB | AMD Ryzen 9 9950X3D2 16-Core @ 5.67GHz (16 Cores / 32 Threads) | `-m 1700` | [2608193-NE-SUPERCOMP30](https://openbenchmarking.org/result/2608193-NE-SUPERCOMP30) |

**Measurements in this card:** 4 PTS rows. CPU host is shown only as system context; these rows do not constitute CPU-only benchmarks.
