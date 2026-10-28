# Intel HD Graphics 4600 — OpenBenchmarking Hashcat measurements (partial, no stdout)

- **Evidence:** PTS-published individual benchmark values; no raw Hashcat console stdout is available from these result exports.
- **PTS runner:** profile executes `hashcat -b --benchmark-min=30` with the per-mode arguments below.
- **Values:** exact PTS mean in H/s and exact repeat values when PTS publishes them. A PTS repeat is not a copied `Speed.#N` console line.
- **Hardware:** exact PTS graphics descriptor is kept per row; aliases are explained in the note below.

| Date | Hashcat | Mode | Benchmark | Mean (H/s) | Readable speed | PTS repeat values (H/s) | PTS GPU label | CPU host context | Args | Result |
|---|---|---:|---|---:|---:|---|---|---|---|---|
| 2026-05-31 | 7.1.2 | 0 | Benchmark: MD5 | 3789133333 | 3.789 GH/s | 3790200000, 3788700000, 3788500000 | Intel HD 4600 HSW GT2 2GB | Intel Core i7-4720HQ @ 3.60GHz (4 Cores / 8 Threads) | `-m 0` | [2605317-TWEA-TTTT52384](https://openbenchmarking.org/result/2605317-TWEA-TTTT52384) |
| 2026-05-31 | 7.1.2 | 100 | Benchmark: SHA1 | 1282466667 | 1.282 GH/s | 1282500000, 1282500000, 1282400000 | Intel HD 4600 HSW GT2 2GB | Intel Core i7-4720HQ @ 3.60GHz (4 Cores / 8 Threads) | `-m 100` | [2605317-TWEA-TTTT52384](https://openbenchmarking.org/result/2605317-TWEA-TTTT52384) |
| 2026-05-31 | 7.1.2 | 1000 | Benchmark: NTLM | 6580733333 | 6.581 GH/s | 6581600000, 6580500000, 6580100000 | Intel HD 4600 HSW GT2 2GB | Intel Core i7-4720HQ @ 3.60GHz (4 Cores / 8 Threads) | `-m 1000` | [2605317-TWEA-TTTT52384](https://openbenchmarking.org/result/2605317-TWEA-TTTT52384) |
| 2026-05-31 | 7.1.2 | 1400 | Benchmark: SHA-256 | 349033333 | 349 MH/s | 349100000, 349000000, 349000000 | Intel HD 4600 HSW GT2 2GB | Intel Core i7-4720HQ @ 3.60GHz (4 Cores / 8 Threads) | `-m 1400` | [2605317-TWEA-TTTT52384](https://openbenchmarking.org/result/2605317-TWEA-TTTT52384) |
| 2026-05-31 | 7.1.2 | 1700 | Benchmark: SHA-512 | 148566667 | 148.6 MH/s | 148600000, 148500000, 148600000 | Intel HD 4600 HSW GT2 2GB | Intel Core i7-4720HQ @ 3.60GHz (4 Cores / 8 Threads) | `-m 1700` | [2605317-TWEA-TTTT52384](https://openbenchmarking.org/result/2605317-TWEA-TTTT52384) |
| 2026-05-31 | 7.1.2 | 3200 | Benchmark: bcrypt | 1739 | 1.739 kH/s | 1739, 1739, 1739 | Intel HD 4600 HSW GT2 2GB | Intel Core i7-4720HQ @ 3.60GHz (4 Cores / 8 Threads) | `-m 3200` | [2605317-TWEA-TTTT52384](https://openbenchmarking.org/result/2605317-TWEA-TTTT52384) |
| 2026-05-31 | 7.1.2 | 6211 | Benchmark: TrueCrypt RIPEMD160 + XTS | 42193 | 42.19 kH/s | 42203, 42186, 42189 | Intel HD 4600 HSW GT2 2GB | Intel Core i7-4720HQ @ 3.60GHz (4 Cores / 8 Threads) | `-m 6211` | [2605317-TWEA-TTTT52384](https://openbenchmarking.org/result/2605317-TWEA-TTTT52384) |
| 2026-05-31 | 7.1.2 | 6800 | Benchmark: LastPass | 1844 | 1.844 kH/s | 1858, 1858, 1815 | Intel HD 4600 HSW GT2 2GB | Intel Core i7-4720HQ @ 3.60GHz (4 Cores / 8 Threads) | `-m 6800` | [2605317-TWEA-TTTT52384](https://openbenchmarking.org/result/2605317-TWEA-TTTT52384) |
| 2026-05-31 | 7.1.2 | 11600 | Benchmark: 7-Zip | 54456 | 54.46 kH/s | 54455, 54468, 54446 | Intel HD 4600 HSW GT2 2GB | Intel Core i7-4720HQ @ 3.60GHz (4 Cores / 8 Threads) | `-m 11600` | [2605317-TWEA-TTTT52384](https://openbenchmarking.org/result/2605317-TWEA-TTTT52384) |
| 2026-05-31 | 7.1.2 | 13100 | Benchmark: Kerberos 5 + etype 23 + TGS-REP | 35553667 | 35.55 MH/s | 35552000, 35551500, 35557500 | Intel HD 4600 HSW GT2 2GB | Intel Core i7-4720HQ @ 3.60GHz (4 Cores / 8 Threads) | `-m 13100` | [2605317-TWEA-TTTT52384](https://openbenchmarking.org/result/2605317-TWEA-TTTT52384) |
| 2026-05-31 | 7.1.2 | 22000 | Benchmark: WPA-PBKDF2-PMKID+EAPOL | 65993 | 65.99 kH/s | 65596, 66188, 66195 | Intel HD 4600 HSW GT2 2GB | Intel Core i7-4720HQ @ 3.60GHz (4 Cores / 8 Threads) | `-m 22000` | [2605317-TWEA-TTTT52384](https://openbenchmarking.org/result/2605317-TWEA-TTTT52384) |
| 2026-05-31 | 7.1.2 | 34100 | Benchmark: LUKS v2 argon2id + SHA-256 + AES | 1 | 1 H/s | 1, 1, 1 | Intel HD 4600 HSW GT2 2GB | Intel Core i7-4720HQ @ 3.60GHz (4 Cores / 8 Threads) | `-m 34100` | [2605317-TWEA-TTTT52384](https://openbenchmarking.org/result/2605317-TWEA-TTTT52384) |

**Measurements in this card:** 12 PTS rows. CPU host is shown only as system context; these rows do not constitute CPU-only benchmarks.
