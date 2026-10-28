# Intel Arc A770 — OpenBenchmarking Hashcat measurements (partial, no stdout)

- **Evidence:** PTS-published individual benchmark values; no raw Hashcat console stdout is available from these result exports.
- **PTS runner:** profile executes `hashcat -b --benchmark-min=30` with the per-mode arguments below.
- **Values:** exact PTS mean in H/s and exact repeat values when PTS publishes them. A PTS repeat is not a copied `Speed.#N` console line.
- **Hardware:** exact PTS graphics descriptor is kept per row; aliases are explained in the note below.

| Date | Hashcat | Mode | Benchmark | Mean (H/s) | Readable speed | PTS repeat values (H/s) | PTS GPU label | CPU host context | Args | Result |
|---|---|---:|---|---:|---:|---|---|---|---|---|
| 2026-04-06 | 7.1.2 | 0 | Hashcat | 42298466667 | 42.3 GH/s | 42334900000, 42247300000, 42313200000 | Arc A770 | AMD Ryzen Threadripper 9980X 64-Cores @ 5.48GHz (64 Cores / 128 Threads) | `-m 0` | [2604083-NE-INTELARCP47](https://openbenchmarking.org/result/2604083-NE-INTELARCP47) |
| 2026-04-06 | 7.1.2 | 100 | Hashcat | 15803733333 | 15.8 GH/s | 15805000000, 15807500000, 15798700000 | Arc A770 | AMD Ryzen Threadripper 9980X 64-Cores @ 5.48GHz (64 Cores / 128 Threads) | `-m 100` | [2604083-NE-INTELARCP47](https://openbenchmarking.org/result/2604083-NE-INTELARCP47) |
| 2026-04-06 | 7.1.2 | 1000 | Hashcat | 70711200000 | 70.71 GH/s | 70812700000, 70692500000, 70628400000 | Arc A770 | AMD Ryzen Threadripper 9980X 64-Cores @ 5.48GHz (64 Cores / 128 Threads) | `-m 1000` | [2604083-NE-INTELARCP47](https://openbenchmarking.org/result/2604083-NE-INTELARCP47) |
| 2026-04-06 | 7.1.2 | 1400 | Hashcat | 7078233333 | 7.078 GH/s | 7100100000, 7070400000, 7064200000 | Arc A770 | AMD Ryzen Threadripper 9980X 64-Cores @ 5.48GHz (64 Cores / 128 Threads) | `-m 1400` | [2604083-NE-INTELARCP47](https://openbenchmarking.org/result/2604083-NE-INTELARCP47) |
| 2026-04-06 | 7.1.2 | 1700 | Hashcat | 1199066667 | 1.199 GH/s | 1202600000, 1198700000, 1195900000 | Arc A770 | AMD Ryzen Threadripper 9980X 64-Cores @ 5.48GHz (64 Cores / 128 Threads) | `-m 1700` | [2604083-NE-INTELARCP47](https://openbenchmarking.org/result/2604083-NE-INTELARCP47) |
| 2026-04-06 | 7.1.2 | 3200 | Hashcat | 9364 | 9.364 kH/s | 9364, 9363, 9364 | Arc A770 | AMD Ryzen Threadripper 9980X 64-Cores @ 5.48GHz (64 Cores / 128 Threads) | `-m 3200` | [2604083-NE-INTELARCP47](https://openbenchmarking.org/result/2604083-NE-INTELARCP47) |
| 2026-04-06 | 7.1.2 | 6211 | Hashcat | 381833 | 381.8 kH/s | 383000, 381500, 381000 | Arc A770 | AMD Ryzen Threadripper 9980X 64-Cores @ 5.48GHz (64 Cores / 128 Threads) | `-m 6211` | [2604083-NE-INTELARCP47](https://openbenchmarking.org/result/2604083-NE-INTELARCP47) |
| 2026-04-06 | 7.1.2 | 6800 | Hashcat | 23721 | 23.72 kH/s | 23773, 23697, 23692 | Arc A770 | AMD Ryzen Threadripper 9980X 64-Cores @ 5.48GHz (64 Cores / 128 Threads) | `-m 6800` | [2604083-NE-INTELARCP47](https://openbenchmarking.org/result/2604083-NE-INTELARCP47) |
| 2026-04-06 | 7.1.2 | 11600 | Hashcat | 236200 | 236.2 kH/s | 236000, 236300, 236300 | Arc A770 | AMD Ryzen Threadripper 9980X 64-Cores @ 5.48GHz (64 Cores / 128 Threads) | `-m 11600` | [2604083-NE-INTELARCP47](https://openbenchmarking.org/result/2604083-NE-INTELARCP47) |
| 2026-04-06 | 7.1.2 | 13100 | Hashcat | 403266667 | 403.3 MH/s | 407400000, 401200000, 401200000 | Arc A770 | AMD Ryzen Threadripper 9980X 64-Cores @ 5.48GHz (64 Cores / 128 Threads) | `-m 13100` | [2604083-NE-INTELARCP47](https://openbenchmarking.org/result/2604083-NE-INTELARCP47) |
| 2026-04-06 | 7.1.2 | 22000 | Hashcat | 809867 | 809.9 kH/s | 810900, 809500, 809200 | Arc A770 | AMD Ryzen Threadripper 9980X 64-Cores @ 5.48GHz (64 Cores / 128 Threads) | `-m 22000` | [2604083-NE-INTELARCP47](https://openbenchmarking.org/result/2604083-NE-INTELARCP47) |
| 2026-04-06 | 7.1.2 | 34100 | Hashcat | 2 | 2 H/s | 2, 2, 2 | Arc A770 | AMD Ryzen Threadripper 9980X 64-Cores @ 5.48GHz (64 Cores / 128 Threads) | `-m 34100` | [2604083-NE-INTELARCP47](https://openbenchmarking.org/result/2604083-NE-INTELARCP47) |

**Measurements in this card:** 12 PTS rows. CPU host is shown only as system context; these rows do not constitute CPU-only benchmarks.
