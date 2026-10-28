# AMD Radeon RX 5700 — OpenBenchmarking Hashcat measurements (partial, no stdout)

- **Evidence:** PTS-published individual benchmark values; no raw Hashcat console stdout is available from these result exports.
- **PTS runner:** profile executes `hashcat -b --benchmark-min=30` with the per-mode arguments below.
- **Values:** exact PTS mean in H/s and exact repeat values when PTS publishes them. A PTS repeat is not a copied `Speed.#N` console line.
- **Hardware:** exact PTS graphics descriptor is kept per row; aliases are explained in the note below.

| Date | Hashcat | Mode | Benchmark | Mean (H/s) | Readable speed | PTS repeat values (H/s) | PTS GPU label | CPU host context | Args | Result |
|---|---|---:|---|---:|---:|---|---|---|---|---|
| 2026-04-24 | 7.1.2 | 0 | Benchmark: MD5 | 15285966667 | 15.29 GH/s | 15331800000, 15323100000, 15203000000 | Gigabyte AMD Radeon RX 5700 8GB | Intel Core i7-6700K @ 4.20GHz (4 Cores / 8 Threads) | `-m 0` | [2604244-NE-NORMAL87152](https://openbenchmarking.org/result/2604244-NE-NORMAL87152) |
| 2026-04-24 | 7.1.2 | 100 | Benchmark: SHA1 | 5633600000 | 5.634 GH/s | 5699200000, 5695400000, 5506200000 | Gigabyte AMD Radeon RX 5700 8GB | Intel Core i7-6700K @ 4.20GHz (4 Cores / 8 Threads) | `-m 100` | [2604244-NE-NORMAL87152](https://openbenchmarking.org/result/2604244-NE-NORMAL87152) |
| 2026-04-24 | 7.1.2 | 1000 | Benchmark: NTLM | 25766900000 | 25.77 GH/s | 25794600000, 25745200000, 25760900000 | Gigabyte AMD Radeon RX 5700 8GB | Intel Core i7-6700K @ 4.20GHz (4 Cores / 8 Threads) | `-m 1000` | [2604244-NE-NORMAL87152](https://openbenchmarking.org/result/2604244-NE-NORMAL87152) |
| 2026-04-24 | 7.1.2 | 1400 | Benchmark: SHA-256 | 2220266667 | 2.22 GH/s | 2220400000, 2220800000, 2219600000 | Gigabyte AMD Radeon RX 5700 8GB | Intel Core i7-6700K @ 4.20GHz (4 Cores / 8 Threads) | `-m 1400` | [2604244-NE-NORMAL87152](https://openbenchmarking.org/result/2604244-NE-NORMAL87152) |
| 2026-04-24 | 7.1.2 | 1700 | Benchmark: SHA-512 | 468933333 | 468.9 MH/s | 469500000, 469100000, 468200000 | Gigabyte AMD Radeon RX 5700 8GB | Intel Core i7-6700K @ 4.20GHz (4 Cores / 8 Threads) | `-m 1700` | [2604244-NE-NORMAL87152](https://openbenchmarking.org/result/2604244-NE-NORMAL87152) |
| 2026-04-24 | 7.1.2 | 3200 | Benchmark: bcrypt | 18281 | 18.28 kH/s | 18383, 18229, 18231 | Gigabyte AMD Radeon RX 5700 8GB | Intel Core i7-6700K @ 4.20GHz (4 Cores / 8 Threads) | `-m 3200` | [2604244-NE-NORMAL87152](https://openbenchmarking.org/result/2604244-NE-NORMAL87152) |
| 2026-04-24 | 7.1.2 | 6211 | Benchmark: TrueCrypt RIPEMD160 + XTS | 198467 | 198.5 kH/s | 198500, 198500, 198400 | Gigabyte AMD Radeon RX 5700 8GB | Intel Core i7-6700K @ 4.20GHz (4 Cores / 8 Threads) | `-m 6211` | [2604244-NE-NORMAL87152](https://openbenchmarking.org/result/2604244-NE-NORMAL87152) |
| 2026-04-24 | 7.1.2 | 6800 | Benchmark: LastPass | 9690 | 9.69 kH/s | 9688, 9691, 9690 | Gigabyte AMD Radeon RX 5700 8GB | Intel Core i7-6700K @ 4.20GHz (4 Cores / 8 Threads) | `-m 6800` | [2604244-NE-NORMAL87152](https://openbenchmarking.org/result/2604244-NE-NORMAL87152) |
| 2026-04-24 | 7.1.2 | 11600 | Benchmark: 7-Zip | 297400 | 297.4 kH/s | 296500, 298800, 296900 | Gigabyte AMD Radeon RX 5700 8GB | Intel Core i7-6700K @ 4.20GHz (4 Cores / 8 Threads) | `-m 11600` | [2604244-NE-NORMAL87152](https://openbenchmarking.org/result/2604244-NE-NORMAL87152) |
| 2026-04-24 | 7.1.2 | 13100 | Benchmark: Kerberos 5 + etype 23 + TGS-REP | 200033333 | 200 MH/s | 199800000, 199900000, 200400000 | Gigabyte AMD Radeon RX 5700 8GB | Intel Core i7-6700K @ 4.20GHz (4 Cores / 8 Threads) | `-m 13100` | [2604244-NE-NORMAL87152](https://openbenchmarking.org/result/2604244-NE-NORMAL87152) |
| 2026-04-24 | 7.1.2 | 22000 | Benchmark: WPA-PBKDF2-PMKID+EAPOL | 278133 | 278.1 kH/s | 274600, 274700, 285100 | Gigabyte AMD Radeon RX 5700 8GB | Intel Core i7-6700K @ 4.20GHz (4 Cores / 8 Threads) | `-m 22000` | [2604244-NE-NORMAL87152](https://openbenchmarking.org/result/2604244-NE-NORMAL87152) |
| 2026-04-24 | 7.1.2 | 34100 | Benchmark: LUKS v2 argon2id + SHA-256 + AES | 0 | 0 H/s | not provided (single PTS value) | Gigabyte AMD Radeon RX 5700 8GB | Intel Core i7-6700K @ 4.20GHz (4 Cores / 8 Threads) | `-m 34100` | [2604244-NE-NORMAL87152](https://openbenchmarking.org/result/2604244-NE-NORMAL87152) |

**Measurements in this card:** 12 PTS rows. CPU host is shown only as system context; these rows do not constitute CPU-only benchmarks.
