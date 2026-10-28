# AMD Radeon RX 9060 XT — OpenBenchmarking Hashcat measurements (partial, no stdout)

- **Evidence:** PTS-published individual benchmark values; no raw Hashcat console stdout is available from these result exports.
- **PTS runner:** profile executes `hashcat -b --benchmark-min=30` with the per-mode arguments below.
- **Values:** exact PTS mean in H/s and exact repeat values when PTS publishes them. A PTS repeat is not a copied `Speed.#N` console line.
- **Hardware:** exact PTS graphics descriptor is kept per row; aliases are explained in the note below.

| Date | Hashcat | Mode | Benchmark | Mean (H/s) | Readable speed | PTS repeat values (H/s) | PTS GPU label | CPU host context | Args | Result |
|---|---|---:|---|---:|---:|---|---|---|---|---|
| 2026-07-11 | 7.1.2 | 0 | Benchmark: MD5 | 25522766667 | 25.52 GH/s | 25586200000, 25502700000, 25479400000 | AMD Radeon RX 9060 XT 16GB | AMD Ryzen 7 5700X 8-Core @ 4.67GHz (8 Cores / 16 Threads) | `-m 0` | [2607118-NE-20260711925](https://openbenchmarking.org/result/2607118-NE-20260711925) |
| 2026-07-11 | 7.1.2 | 100 | Benchmark: SHA1 | 12023300000 | 12.02 GH/s | 12019700000, 12028500000, 12021700000 | AMD Radeon RX 9060 XT 16GB | AMD Ryzen 7 5700X 8-Core @ 4.67GHz (8 Cores / 16 Threads) | `-m 100` | [2607118-NE-20260711925](https://openbenchmarking.org/result/2607118-NE-20260711925) |
| 2026-07-11 | 7.1.2 | 1000 | Benchmark: NTLM | 44898266667 | 44.9 GH/s | 45252800000, 44615800000, 44826200000 | AMD Radeon RX 9060 XT 16GB | AMD Ryzen 7 5700X 8-Core @ 4.67GHz (8 Cores / 16 Threads) | `-m 1000` | [2607118-NE-20260711925](https://openbenchmarking.org/result/2607118-NE-20260711925) |
| 2026-07-11 | 7.1.2 | 1400 | Benchmark: SHA-256 | 5157766667 | 5.158 GH/s | 5179800000, 5148300000, 5145200000 | AMD Radeon RX 9060 XT 16GB | AMD Ryzen 7 5700X 8-Core @ 4.67GHz (8 Cores / 16 Threads) | `-m 1400` | [2607118-NE-20260711925](https://openbenchmarking.org/result/2607118-NE-20260711925) |
| 2026-07-11 | 7.1.2 | 1700 | Benchmark: SHA-512 | 1333833333 | 1.334 GH/s | 1336500000, 1333000000, 1332000000 | AMD Radeon RX 9060 XT 16GB | AMD Ryzen 7 5700X 8-Core @ 4.67GHz (8 Cores / 16 Threads) | `-m 1700` | [2607118-NE-20260711925](https://openbenchmarking.org/result/2607118-NE-20260711925) |
| 2026-07-11 | 7.1.2 | 3200 | Benchmark: bcrypt | 33792 | 33.79 kH/s | 33777, 33828, 33770 | AMD Radeon RX 9060 XT 16GB | AMD Ryzen 7 5700X 8-Core @ 4.67GHz (8 Cores / 16 Threads) | `-m 3200` | [2607118-NE-20260711925](https://openbenchmarking.org/result/2607118-NE-20260711925) |
| 2026-07-11 | 7.1.2 | 6211 | Benchmark: TrueCrypt RIPEMD160 + XTS | 393100 | 393.1 kH/s | 395900, 393100, 390300 | AMD Radeon RX 9060 XT 16GB | AMD Ryzen 7 5700X 8-Core @ 4.67GHz (8 Cores / 16 Threads) | `-m 6211` | [2607118-NE-20260711925](https://openbenchmarking.org/result/2607118-NE-20260711925) |
| 2026-07-11 | 7.1.2 | 6800 | Benchmark: LastPass | 21524 | 21.52 kH/s | 21582, 21493, 21496 | AMD Radeon RX 9060 XT 16GB | AMD Ryzen 7 5700X 8-Core @ 4.67GHz (8 Cores / 16 Threads) | `-m 6800` | [2607118-NE-20260711925](https://openbenchmarking.org/result/2607118-NE-20260711925) |
| 2026-07-11 | 7.1.2 | 11600 | Benchmark: 7-Zip | 651467 | 651.5 kH/s | 652800, 655100, 646500 | AMD Radeon RX 9060 XT 16GB | AMD Ryzen 7 5700X 8-Core @ 4.67GHz (8 Cores / 16 Threads) | `-m 11600` | [2607118-NE-20260711925](https://openbenchmarking.org/result/2607118-NE-20260711925) |
| 2026-07-11 | 7.1.2 | 13100 | Benchmark: Kerberos 5 + etype 23 + TGS-REP | 594700000 | 594.7 MH/s | 594800000, 596400000, 592900000 | AMD Radeon RX 9060 XT 16GB | AMD Ryzen 7 5700X 8-Core @ 4.67GHz (8 Cores / 16 Threads) | `-m 13100` | [2607118-NE-20260711925](https://openbenchmarking.org/result/2607118-NE-20260711925) |
| 2026-07-11 | 7.1.2 | 22000 | Benchmark: WPA-PBKDF2-PMKID+EAPOL | 615467 | 615.5 kH/s | 618500, 613100, 614800 | AMD Radeon RX 9060 XT 16GB | AMD Ryzen 7 5700X 8-Core @ 4.67GHz (8 Cores / 16 Threads) | `-m 22000` | [2607118-NE-20260711925](https://openbenchmarking.org/result/2607118-NE-20260711925) |
| 2026-07-11 | 7.1.2 | 34100 | Benchmark: LUKS v2 argon2id + SHA-256 + AES | 15 | 15 H/s | 14, 15, 15, 15, 15, 15, 15, 15 | AMD Radeon RX 9060 XT 16GB | AMD Ryzen 7 5700X 8-Core @ 4.67GHz (8 Cores / 16 Threads) | `-m 34100` | [2607118-NE-20260711925](https://openbenchmarking.org/result/2607118-NE-20260711925) |

**Measurements in this card:** 12 PTS rows. CPU host is shown only as system context; these rows do not constitute CPU-only benchmarks.
