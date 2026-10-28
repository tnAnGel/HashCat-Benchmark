# AMD Radeon RX 470-590 (PTS combined alias) — OpenBenchmarking Hashcat measurements (partial, no stdout)

- **Evidence:** PTS-published individual benchmark values; no raw Hashcat console stdout is available from these result exports.
- **PTS runner:** profile executes `hashcat -b --benchmark-min=30` with the per-mode arguments below.
- **Values:** exact PTS mean in H/s and exact repeat values when PTS publishes them. A PTS repeat is not a copied `Speed.#N` console line.
- **Hardware:** exact PTS graphics descriptor is kept per row; aliases are explained in the note below.

> PTS groups RX 470/480/570/570X/580/580X/590 into one system label. These results cannot be assigned to an individual SKU; retained as a combined alias only.

| Date | Hashcat | Mode | Benchmark | Mean (H/s) | Readable speed | PTS repeat values (H/s) | PTS GPU label | CPU host context | Args | Result |
|---|---|---:|---|---:|---:|---|---|---|---|---|
| 2026-06-03 | 7.1.2 | 0 | Benchmark: MD5 | 9454733333 | 9.455 GH/s | 9452600000, 9452800000, 9458800000 | AMD Radeon RX 470/480/570/570X/580/580X/590 | Intel Core i5-8600K @ 4.30GHz (6 Cores) | `-m 0` | [2606026-NE-HASHCATTN39](https://openbenchmarking.org/result/2606026-NE-HASHCATTN39) |
| 2026-06-03 | 7.1.2 | 100 | Benchmark: SHA1 | 2913600000 | 2.914 GH/s | 2916200000, 2910600000, 2914000000 | AMD Radeon RX 470/480/570/570X/580/580X/590 | Intel Core i5-8600K @ 4.30GHz (6 Cores) | `-m 100` | [2606026-NE-HASHCATTN39](https://openbenchmarking.org/result/2606026-NE-HASHCATTN39) |
| 2026-06-03 | 7.1.2 | 1000 | Benchmark: NTLM | 15323733333 | 15.32 GH/s | 15308100000, 15354800000, 15308300000 | AMD Radeon RX 470/480/570/570X/580/580X/590 | Intel Core i5-8600K @ 4.30GHz (6 Cores) | `-m 1000` | [2606026-NE-HASHCATTN39](https://openbenchmarking.org/result/2606026-NE-HASHCATTN39) |
| 2026-06-03 | 7.1.2 | 1400 | Benchmark: SHA-256 | 1156033333 | 1.156 GH/s | 1156500000, 1156700000, 1154900000 | AMD Radeon RX 470/480/570/570X/580/580X/590 | Intel Core i5-8600K @ 4.30GHz (6 Cores) | `-m 1400` | [2606026-NE-HASHCATTN39](https://openbenchmarking.org/result/2606026-NE-HASHCATTN39) |
| 2026-06-03 | 7.1.2 | 1700 | Benchmark: SHA-512 | 163500000 | 163.5 MH/s | 163600000, 163500000, 163400000 | AMD Radeon RX 470/480/570/570X/580/580X/590 | Intel Core i5-8600K @ 4.30GHz (6 Cores) | `-m 1700` | [2606026-NE-HASHCATTN39](https://openbenchmarking.org/result/2606026-NE-HASHCATTN39) |
| 2026-06-03 | 7.1.2 | 3200 | Benchmark: bcrypt | 9178 | 9.178 kH/s | 9143, 9153, 9237 | AMD Radeon RX 470/480/570/570X/580/580X/590 | Intel Core i5-8600K @ 4.30GHz (6 Cores) | `-m 3200` | [2606026-NE-HASHCATTN39](https://openbenchmarking.org/result/2606026-NE-HASHCATTN39) |
| 2026-06-03 | 7.1.2 | 6211 | Benchmark: TrueCrypt RIPEMD160 + XTS | 106033 | 106 kH/s | 106000, 106100, 106000 | AMD Radeon RX 470/480/570/570X/580/580X/590 | Intel Core i5-8600K @ 4.30GHz (6 Cores) | `-m 6211` | [2606026-NE-HASHCATTN39](https://openbenchmarking.org/result/2606026-NE-HASHCATTN39) |
| 2026-06-03 | 7.1.2 | 6800 | Benchmark: LastPass | 4978 | 4.978 kH/s | 4978, 4978, 4977 | AMD Radeon RX 470/480/570/570X/580/580X/590 | Intel Core i5-8600K @ 4.30GHz (6 Cores) | `-m 6800` | [2606026-NE-HASHCATTN39](https://openbenchmarking.org/result/2606026-NE-HASHCATTN39) |
| 2026-06-03 | 7.1.2 | 11600 | Benchmark: 7-Zip | 162400 | 162.4 kH/s | 162600, 162300, 162300 | AMD Radeon RX 470/480/570/570X/580/580X/590 | Intel Core i5-8600K @ 4.30GHz (6 Cores) | `-m 11600` | [2606026-NE-HASHCATTN39](https://openbenchmarking.org/result/2606026-NE-HASHCATTN39) |
| 2026-06-03 | 7.1.2 | 13100 | Benchmark: Kerberos 5 + etype 23 + TGS-REP | 91322500 | 91.32 MH/s | 91468900, 90947600, 91551000 | AMD Radeon RX 470/480/570/570X/580/580X/590 | Intel Core i5-8600K @ 4.30GHz (6 Cores) | `-m 13100` | [2606026-NE-HASHCATTN39](https://openbenchmarking.org/result/2606026-NE-HASHCATTN39) |
| 2026-06-03 | 7.1.2 | 22000 | Benchmark: WPA-PBKDF2-PMKID+EAPOL | 138933 | 138.9 kH/s | 138900, 139000, 138900 | AMD Radeon RX 470/480/570/570X/580/580X/590 | Intel Core i5-8600K @ 4.30GHz (6 Cores) | `-m 22000` | [2606026-NE-HASHCATTN39](https://openbenchmarking.org/result/2606026-NE-HASHCATTN39) |
| 2026-06-03 | 7.1.2 | 34100 | Benchmark: LUKS v2 argon2id + SHA-256 + AES | 0 | 0 H/s | not provided (single PTS value) | AMD Radeon RX 470/480/570/570X/580/580X/590 | Intel Core i5-8600K @ 4.30GHz (6 Cores) | `-m 34100` | [2606026-NE-HASHCATTN39](https://openbenchmarking.org/result/2606026-NE-HASHCATTN39) |

**Measurements in this card:** 12 PTS rows. CPU host is shown only as system context; these rows do not constitute CPU-only benchmarks.
