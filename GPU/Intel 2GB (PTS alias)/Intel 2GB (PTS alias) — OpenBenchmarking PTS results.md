# Intel 2GB (PTS alias) — OpenBenchmarking Hashcat measurements (partial, no stdout)

- **Evidence:** PTS-published individual benchmark values; no raw Hashcat console stdout is available from these result exports.
- **PTS runner:** profile executes `hashcat -b --benchmark-min=30` with the per-mode arguments below.
- **Values:** exact PTS mean in H/s and exact repeat values when PTS publishes them. A PTS repeat is not a copied `Speed.#N` console line.
- **Hardware:** exact PTS graphics descriptor is kept per row; aliases are explained in the note below.

> PTS reports only “Intel 2GB”; exact integrated GPU SKU is not identifiable from the result.

| Date | Hashcat | Mode | Benchmark | Mean (H/s) | Readable speed | PTS repeat values (H/s) | PTS GPU label | CPU host context | Args | Result |
|---|---|---:|---|---:|---:|---|---|---|---|---|
| 2026-06-11 | 7.1.2 | 0 | Benchmark: MD5 | 4367333333 | 4.367 GH/s | 4385300000, 4435300000, 4281400000 | Intel 2GB | Intel Core Ultra 7 366H @ 2.00GHz (16 Cores) | `-m 0` | [2606110-NE-HASHCATBE36](https://openbenchmarking.org/result/2606110-NE-HASHCATBE36) |
| 2026-06-11 | 7.1.2 | 100 | Benchmark: SHA1 | 1801000000 | 1.801 GH/s | 1799400000, 1790200000, 1813400000 | Intel 2GB | Intel Core Ultra 7 366H @ 2.00GHz (16 Cores) | `-m 100` | [2606110-NE-HASHCATBE36](https://openbenchmarking.org/result/2606110-NE-HASHCATBE36) |
| 2026-06-11 | 7.1.2 | 1000 | Benchmark: NTLM | 7698166667 | 7.698 GH/s | 7657900000, 7720700000, 7715900000 | Intel 2GB | Intel Core Ultra 7 366H @ 2.00GHz (16 Cores) | `-m 1000` | [2606110-NE-HASHCATBE36](https://openbenchmarking.org/result/2606110-NE-HASHCATBE36) |
| 2026-06-11 | 7.1.2 | 1400 | Benchmark: SHA-256 | 771100000 | 771.1 MH/s | 763500000, 774900000, 774900000 | Intel 2GB | Intel Core Ultra 7 366H @ 2.00GHz (16 Cores) | `-m 1400` | [2606110-NE-HASHCATBE36](https://openbenchmarking.org/result/2606110-NE-HASHCATBE36) |
| 2026-06-11 | 7.1.2 | 1700 | Benchmark: SHA-512 | 80540333 | 80.54 MH/s | 80582900, 80476600, 80561500 | Intel 2GB | Intel Core Ultra 7 366H @ 2.00GHz (16 Cores) | `-m 1700` | [2606110-NE-HASHCATBE36](https://openbenchmarking.org/result/2606110-NE-HASHCATBE36) |
| 2026-06-11 | 7.1.2 | 3200 | Benchmark: bcrypt | 3108 | 3.108 kH/s | 3091, 3116, 3116 | Intel 2GB | Intel Core Ultra 7 366H @ 2.00GHz (16 Cores) | `-m 3200` | [2606110-NE-HASHCATBE36](https://openbenchmarking.org/result/2606110-NE-HASHCATBE36) |
| 2026-06-11 | 7.1.2 | 6211 | Benchmark: TrueCrypt RIPEMD160 + XTS | 73957 | 73.96 kH/s | 74786, 62895, 74807, 76337, 76652, 76522, 76404, 76019, 75008, 75796, 75985, 75198, 61939, 75411, 75598 | Intel 2GB | Intel Core Ultra 7 366H @ 2.00GHz (16 Cores) | `-m 6211` | [2606110-NE-HASHCATBE36](https://openbenchmarking.org/result/2606110-NE-HASHCATBE36) |
| 2026-06-11 | 7.1.2 | 6800 | Benchmark: LastPass | 3981 | 3.981 kH/s | 3966, 3986, 3992 | Intel 2GB | Intel Core Ultra 7 366H @ 2.00GHz (16 Cores) | `-m 6800` | [2606110-NE-HASHCATBE36](https://openbenchmarking.org/result/2606110-NE-HASHCATBE36) |
| 2026-06-11 | 7.1.2 | 11600 | Benchmark: 7-Zip | 59829 | 59.83 kH/s | 59900, 59549, 60038 | Intel 2GB | Intel Core Ultra 7 366H @ 2.00GHz (16 Cores) | `-m 11600` | [2606110-NE-HASHCATBE36](https://openbenchmarking.org/result/2606110-NE-HASHCATBE36) |
| 2026-06-11 | 7.1.2 | 13100 | Benchmark: Kerberos 5 + etype 23 + TGS-REP | 39219067 | 39.22 MH/s | 38851500, 39475600, 39330100 | Intel 2GB | Intel Core Ultra 7 366H @ 2.00GHz (16 Cores) | `-m 13100` | [2606110-NE-HASHCATBE36](https://openbenchmarking.org/result/2606110-NE-HASHCATBE36) |
| 2026-06-11 | 7.1.2 | 22000 | Benchmark: WPA-PBKDF2-PMKID+EAPOL | 91200 | 91.2 kH/s | 92796, 90539, 90264 | Intel 2GB | Intel Core Ultra 7 366H @ 2.00GHz (16 Cores) | `-m 22000` | [2606110-NE-HASHCATBE36](https://openbenchmarking.org/result/2606110-NE-HASHCATBE36) |
| 2026-06-11 | 7.1.2 | 34100 | Benchmark: LUKS v2 argon2id + SHA-256 + AES | 1 | 1 H/s | not provided (single PTS value) | Intel 2GB | Intel Core Ultra 7 366H @ 2.00GHz (16 Cores) | `-m 34100` | [2606110-NE-HASHCATBE36](https://openbenchmarking.org/result/2606110-NE-HASHCATBE36) |

**Measurements in this card:** 12 PTS rows. CPU host is shown only as system context; these rows do not constitute CPU-only benchmarks.
