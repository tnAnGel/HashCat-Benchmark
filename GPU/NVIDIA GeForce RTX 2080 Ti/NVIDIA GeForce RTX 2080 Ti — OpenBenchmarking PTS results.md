# NVIDIA GeForce RTX 2080 Ti — OpenBenchmarking Hashcat measurements (partial, no stdout)

- **Evidence:** PTS-published individual benchmark values; no raw Hashcat console stdout is available from these result exports.
- **PTS runner:** profile executes `hashcat -b --benchmark-min=30` with the per-mode arguments below.
- **Values:** exact PTS mean in H/s and exact repeat values when PTS publishes them. A PTS repeat is not a copied `Speed.#N` console line.
- **Hardware:** exact PTS graphics descriptor is kept per row; aliases are explained in the note below.

| Date | Hashcat | Mode | Benchmark | Mean (H/s) | Readable speed | PTS repeat values (H/s) | PTS GPU label | CPU host context | Args | Result |
|---|---|---:|---|---:|---:|---|---|---|---|---|
| 2026-06-06 | 7.1.2 | 1700 | Benchmark: SHA-512 | 14317633333 | 14.32 GH/s | 14430700000, 14305900000, 14216300000 | NVIDIA GeForce RTX 2080 Ti 11GB | 2 x Intel Xeon Platinum 8260 @ 3.90GHz (48 Cores / 96 Threads) | `-m 1700` | [2606069-NE-GPU03994708](https://openbenchmarking.org/result/2606069-NE-GPU03994708) |

**Measurements in this card:** 1 PTS rows. CPU host is shown only as system context; these rows do not constitute CPU-only benchmarks.
