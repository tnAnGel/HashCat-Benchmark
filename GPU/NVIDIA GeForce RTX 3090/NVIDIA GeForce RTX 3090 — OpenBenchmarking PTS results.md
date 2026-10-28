# NVIDIA GeForce RTX 3090 — OpenBenchmarking Hashcat measurements (partial, no stdout)

- **Evidence:** PTS-published individual benchmark values; no raw Hashcat console stdout is available from these result exports.
- **PTS runner:** profile executes `hashcat -b --benchmark-min=30` with the per-mode arguments below.
- **Values:** exact PTS mean in H/s and exact repeat values when PTS publishes them. A PTS repeat is not a copied `Speed.#N` console line.
- **Hardware:** exact PTS graphics descriptor is kept per row; aliases are explained in the note below.

| Date | Hashcat | Mode | Benchmark | Mean (H/s) | Readable speed | PTS repeat values (H/s) | PTS GPU label | CPU host context | Args | Result |
|---|---|---:|---|---:|---:|---|---|---|---|---|
| 2026-09-01 | v7.1.2 | 0 | Benchmark: MD5 | 62744866667 | 62.74 GH/s | 63023100000, 62682200000, 62529300000 | ASUS NVIDIA GeForce RTX 3090 24GB | AMD Ryzen 9 7945HX3D @ 5.46GHz (16 Cores / 32 Threads) | `-m 0` | [2609012-NE-LOCALRIGV86](https://openbenchmarking.org/result/2609012-NE-LOCALRIGV86) |
| 2026-09-01 | v7.1.2 | 100 | Benchmark: SHA1 | 19647133333 | 19.65 GH/s | 19711400000, 19606900000, 19623100000 | ASUS NVIDIA GeForce RTX 3090 24GB | AMD Ryzen 9 7945HX3D @ 5.46GHz (16 Cores / 32 Threads) | `-m 100` | [2609012-NE-LOCALRIGV86](https://openbenchmarking.org/result/2609012-NE-LOCALRIGV86) |
| 2026-09-01 | v7.1.2 | 1400 | Benchmark: SHA-256 | 8672400000 | 8.672 GH/s | 8677800000, 8669400000, 8670000000 | ASUS NVIDIA GeForce RTX 3090 24GB | AMD Ryzen 9 7945HX3D @ 5.46GHz (16 Cores / 32 Threads) | `-m 1400` | [2609012-NE-LOCALRIGV86](https://openbenchmarking.org/result/2609012-NE-LOCALRIGV86) |
| 2026-09-01 | v7.1.2 | 1700 | Benchmark: SHA-512 | 2859900000 | 2.86 GH/s | 2861700000, 2860700000, 2857300000 | ASUS NVIDIA GeForce RTX 3090 24GB | AMD Ryzen 9 7945HX3D @ 5.46GHz (16 Cores / 32 Threads) | `-m 1700` | [2609012-NE-LOCALRIGV86](https://openbenchmarking.org/result/2609012-NE-LOCALRIGV86) |
| 2026-09-01 | v7.1.2 | 3200 | Benchmark: bcrypt | 100367 | 100.4 kH/s | 100400, 100400, 100300 | ASUS NVIDIA GeForce RTX 3090 24GB | AMD Ryzen 9 7945HX3D @ 5.46GHz (16 Cores / 32 Threads) | `-m 3200` | [2609012-NE-LOCALRIGV86](https://openbenchmarking.org/result/2609012-NE-LOCALRIGV86) |
| 2026-09-01 | v7.1.2 | 6211 | Benchmark: TrueCrypt RIPEMD160 + XTS | 753133 | 753.1 kH/s | 754200, 753100, 752100 | ASUS NVIDIA GeForce RTX 3090 24GB | AMD Ryzen 9 7945HX3D @ 5.46GHz (16 Cores / 32 Threads) | `-m 6211` | [2609012-NE-LOCALRIGV86](https://openbenchmarking.org/result/2609012-NE-LOCALRIGV86) |
| 2026-09-01 | v7.1.2 | 11600 | Benchmark: 7-Zip | 983333 | 983.3 kH/s | 983500, 981600, 984900 | ASUS NVIDIA GeForce RTX 3090 24GB | AMD Ryzen 9 7945HX3D @ 5.46GHz (16 Cores / 32 Threads) | `-m 11600` | [2609012-NE-LOCALRIGV86](https://openbenchmarking.org/result/2609012-NE-LOCALRIGV86) |
| 2026-09-01 | v7.1.2 | 13100 | Benchmark: Kerberos 5 + etype 23 + TGS-REP | 1351866667 | 1.352 GH/s | 1349600000, 1353800000, 1352200000 | ASUS NVIDIA GeForce RTX 3090 24GB | AMD Ryzen 9 7945HX3D @ 5.46GHz (16 Cores / 32 Threads) | `-m 13100` | [2609012-NE-LOCALRIGV86](https://openbenchmarking.org/result/2609012-NE-LOCALRIGV86) |

**Measurements in this card:** 8 PTS rows. CPU host is shown only as system context; these rows do not constitute CPU-only benchmarks.
