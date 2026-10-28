# NVIDIA GeForce RTX 4070 Laptop GPU — OpenBenchmarking Hashcat measurements (partial, no stdout)

- **Evidence:** PTS-published individual benchmark values; no raw Hashcat console stdout is available from these result exports.
- **PTS runner:** profile executes `hashcat -b --benchmark-min=30` with the per-mode arguments below.
- **Values:** exact PTS mean in H/s and exact repeat values when PTS publishes them. A PTS repeat is not a copied `Speed.#N` console line.
- **Hardware:** exact PTS graphics descriptor is kept per row; aliases are explained in the note below.

| Date | Hashcat | Mode | Benchmark | Mean (H/s) | Readable speed | PTS repeat values (H/s) | PTS GPU label | CPU host context | Args | Result |
|---|---|---:|---|---:|---:|---|---|---|---|---|
| 2026-04-16 | 7.1.2 | 1700 | Benchmark: SHA-512 | 1719366667 | 1.719 GH/s | 1696800000, 1730800000, 1730500000 | MSI NVIDIA GeForce RTX 4070 Laptop GPU 8GB | Intel Core i7-13700H @ 4.80GHz (14 Cores / 20 Threads) | `-m 1700` | [2604161-NE-HASHTESTT88](https://openbenchmarking.org/result/2604161-NE-HASHTESTT88) |

**Measurements in this card:** 1 PTS rows. CPU host is shown only as system context; these rows do not constitute CPU-only benchmarks.
