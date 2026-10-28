# NVIDIA GeForce RTX 2080 SUPER — OpenBenchmarking Hashcat measurements (partial, no stdout)

- **Evidence:** PTS-published individual benchmark values; no raw Hashcat console stdout is available from these result exports.
- **PTS runner:** profile executes `hashcat -b --benchmark-min=30` with the per-mode arguments below.
- **Values:** exact PTS mean in H/s and exact repeat values when PTS publishes them. A PTS repeat is not a copied `Speed.#N` console line.
- **Hardware:** exact PTS graphics descriptor is kept per row; aliases are explained in the note below.

| Date | Hashcat | Mode | Benchmark | Mean (H/s) | Readable speed | PTS repeat values (H/s) | PTS GPU label | CPU host context | Args | Result |
|---|---|---:|---|---:|---:|---|---|---|---|---|
| 2026-06-12 | 7.1.2 | 0 | Benchmark: MD5 | 43375633333 | 43.38 GH/s | 43507800000, 43366000000, 43253100000 | Gigabyte NVIDIA GeForce RTX 2080 SUPER 8GB | Intel Core i7-9700K @ 4.90GHz (8 Cores) | `-m 0` | [2606128-ALEX-OVERALL14](https://openbenchmarking.org/result/2606128-ALEX-OVERALL14) |
| 2026-06-12 | 7.1.2 | 100 | Benchmark: SHA1 | 13415066667 | 13.42 GH/s | 13435300000, 13422200000, 13387700000 | Gigabyte NVIDIA GeForce RTX 2080 SUPER 8GB | Intel Core i7-9700K @ 4.90GHz (8 Cores) | `-m 100` | [2606128-ALEX-OVERALL14](https://openbenchmarking.org/result/2606128-ALEX-OVERALL14) |
| 2026-06-12 | 7.1.2 | 1000 | Benchmark: NTLM | 75535166667 | 75.54 GH/s | 75726100000, 75583400000, 75296000000 | Gigabyte NVIDIA GeForce RTX 2080 SUPER 8GB | Intel Core i7-9700K @ 4.90GHz (8 Cores) | `-m 1000` | [2606128-ALEX-OVERALL14](https://openbenchmarking.org/result/2606128-ALEX-OVERALL14) |
| 2026-06-12 | 7.1.2 | 1400 | Benchmark: SHA-256 | 5681333333 | 5.681 GH/s | 5674900000, 5684200000, 5684900000 | Gigabyte NVIDIA GeForce RTX 2080 SUPER 8GB | Intel Core i7-9700K @ 4.90GHz (8 Cores) | `-m 1400` | [2606128-ALEX-OVERALL14](https://openbenchmarking.org/result/2606128-ALEX-OVERALL14) |
| 2026-06-12 | 7.1.2 | 1700 | Benchmark: SHA-512 | 1902066667 | 1.902 GH/s | 1904800000, 1902200000, 1899200000 | Gigabyte NVIDIA GeForce RTX 2080 SUPER 8GB | Intel Core i7-9700K @ 4.90GHz (8 Cores) | `-m 1700` | [2606128-ALEX-OVERALL14](https://openbenchmarking.org/result/2606128-ALEX-OVERALL14) |
| 2026-06-12 | 7.1.2 | 3200 | Benchmark: bcrypt | 31027 | 31.03 kH/s | 31008, 31036, 31037 | Gigabyte NVIDIA GeForce RTX 2080 SUPER 8GB | Intel Core i7-9700K @ 4.90GHz (8 Cores) | `-m 3200` | [2606128-ALEX-OVERALL14](https://openbenchmarking.org/result/2606128-ALEX-OVERALL14) |
| 2026-06-12 | 7.1.2 | 6211 | Benchmark: TrueCrypt RIPEMD160 + XTS | 505233 | 505.2 kH/s | 506500, 504500, 504700 | Gigabyte NVIDIA GeForce RTX 2080 SUPER 8GB | Intel Core i7-9700K @ 4.90GHz (8 Cores) | `-m 6211` | [2606128-ALEX-OVERALL14](https://openbenchmarking.org/result/2606128-ALEX-OVERALL14) |
| 2026-06-12 | 7.1.2 | 6800 | Benchmark: LastPass | 23473 | 23.47 kH/s | 23528, 23439, 23453 | Gigabyte NVIDIA GeForce RTX 2080 SUPER 8GB | Intel Core i7-9700K @ 4.90GHz (8 Cores) | `-m 6800` | [2606128-ALEX-OVERALL14](https://openbenchmarking.org/result/2606128-ALEX-OVERALL14) |
| 2026-06-12 | 7.1.2 | 11600 | Benchmark: 7-Zip | 647800 | 647.8 kH/s | 648600, 647100, 647700 | Gigabyte NVIDIA GeForce RTX 2080 SUPER 8GB | Intel Core i7-9700K @ 4.90GHz (8 Cores) | `-m 11600` | [2606128-ALEX-OVERALL14](https://openbenchmarking.org/result/2606128-ALEX-OVERALL14) |
| 2026-06-12 | 7.1.2 | 13100 | Benchmark: Kerberos 5 + etype 23 + TGS-REP | 631366667 | 631.4 MH/s | 621400000, 646100000, 626600000 | Gigabyte NVIDIA GeForce RTX 2080 SUPER 8GB | Intel Core i7-9700K @ 4.90GHz (8 Cores) | `-m 13100` | [2606128-ALEX-OVERALL14](https://openbenchmarking.org/result/2606128-ALEX-OVERALL14) |
| 2026-06-12 | 7.1.2 | 22000 | Benchmark: WPA-PBKDF2-PMKID+EAPOL | 674100 | 674.1 kH/s | 674200, 674600, 673500 | Gigabyte NVIDIA GeForce RTX 2080 SUPER 8GB | Intel Core i7-9700K @ 4.90GHz (8 Cores) | `-m 22000` | [2606128-ALEX-OVERALL14](https://openbenchmarking.org/result/2606128-ALEX-OVERALL14) |
| 2026-06-12 | 7.1.2 | 34100 | Benchmark: LUKS v2 argon2id + SHA-256 + AES | 0 | 0 H/s | not provided (single PTS value) | Gigabyte NVIDIA GeForce RTX 2080 SUPER 8GB | Intel Core i7-9700K @ 4.90GHz (8 Cores) | `-m 34100` | [2606128-ALEX-OVERALL14](https://openbenchmarking.org/result/2606128-ALEX-OVERALL14) |

**Measurements in this card:** 12 PTS rows. CPU host is shown only as system context; these rows do not constitute CPU-only benchmarks.
