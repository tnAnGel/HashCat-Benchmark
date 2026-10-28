# Intel Panther Lake Graphics (PTS alias) — OpenBenchmarking Hashcat measurements (partial, no stdout)

- **Evidence:** PTS-published individual benchmark values; no raw Hashcat console stdout is available from these result exports.
- **PTS runner:** profile executes `hashcat -b --benchmark-min=30` with the per-mode arguments below.
- **Values:** exact PTS mean in H/s and exact repeat values when PTS publishes them. A PTS repeat is not a copied `Speed.#N` console line.
- **Hardware:** exact PTS graphics descriptor is kept per row; aliases are explained in the note below.

> PTS reports a Panther Lake device with a shared-memory label; no retail GPU SKU is inferred.

| Date | Hashcat | Mode | Benchmark | Mean (H/s) | Readable speed | PTS repeat values (H/s) | PTS GPU label | CPU host context | Args | Result |
|---|---|---:|---|---:|---:|---|---|---|---|---|
| 2026-02-13 | 7.1.2 | 0 | Benchmark: MD5 | 13546720000 | 13.55 GH/s | 13491900000, 13560500000, 13557100000, 13556000000, 13568100000 | MSI Intel PTL 30GB | Intel Core Ultra X7 358H @ 4.70GHz (16 Cores) | `-m 0` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-13 | 7.1.2 | 100 | Benchmark: SHA1 | 5471640000 | 5.472 GH/s | 5478000000, 5471800000, 5469800000, 5467000000, 5471600000 | MSI Intel PTL 30GB | Intel Core Ultra X7 358H @ 4.70GHz (16 Cores) | `-m 100` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-13 | 7.1.2 | 1000 | Benchmark: NTLM | 24040120000 | 24.04 GH/s | 24072300000, 24024100000, 24020700000, 24041600000, 24041900000 | MSI Intel PTL 30GB | Intel Core Ultra X7 358H @ 4.70GHz (16 Cores) | `-m 1000` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-13 | 7.1.2 | 1400 | Benchmark: SHA-256 | 2341440000 | 2.341 GH/s | 2351900000, 2337000000, 2337000000, 2345500000, 2335800000 | MSI Intel PTL 30GB | Intel Core Ultra X7 358H @ 4.70GHz (16 Cores) | `-m 1400` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-13 | 7.1.2 | 1700 | Benchmark: SHA-512 | 236900000 | 236.9 MH/s | 237000000, 237100000, 236900000, 236600000 | MSI Intel PTL 30GB | Intel Core Ultra X7 358H @ 4.70GHz (16 Cores) | `-m 1700` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-13 | 7.1.2 | 3200 | Benchmark: bcrypt | 6513 | 6.513 kH/s | 6513, 6525, 6525, 6518, 6483 | MSI Intel PTL 30GB | Intel Core Ultra X7 358H @ 4.70GHz (16 Cores) | `-m 3200` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-13 | 7.1.2 | 6211 | Benchmark: TrueCrypt RIPEMD160 + XTS | 177627 | 177.6 kH/s | 185800, 186200, 184100, 182200, 173800, 172000, 177200, 176900, 176000, 175400, 174900, 175700, 174800, 174900, 174500 | MSI Intel PTL 30GB | Intel Core Ultra X7 358H @ 4.70GHz (16 Cores) | `-m 6211` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-13 | 7.1.2 | 6800 | Benchmark: LastPass | 9295 | 9.295 kH/s | 9521, 9478, 9237, 9015, 9222 | MSI Intel PTL 30GB | Intel Core Ultra X7 358H @ 4.70GHz (16 Cores) | `-m 6800` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-13 | 7.1.2 | 11600 | Benchmark: 7-Zip | 237427 | 237.4 kH/s | 251100, 249400, 248900, 248500, 234900, 234300, 232200, 237700, 235300, 234200, 228500, 233800, 231200, 229600, 231800 | MSI Intel PTL 30GB | Intel Core Ultra X7 358H @ 4.70GHz (16 Cores) | `-m 11600` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-13 | 7.1.2 | 13100 | Benchmark: Kerberos 5 + etype 23 + TGS-REP | 177300000 | 177.3 MH/s | 177500000, 176700000, 177000000, 177200000, 178000000, 177400000 | MSI Intel PTL 30GB | Intel Core Ultra X7 358H @ 4.70GHz (16 Cores) | `-m 13100` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-13 | 7.1.2 | 22000 | Benchmark: WPA-PBKDF2-PMKID+EAPOL | 266580 | 266.6 kH/s | 266300, 266500, 265800, 267700, 266600 | MSI Intel PTL 30GB | Intel Core Ultra X7 358H @ 4.70GHz (16 Cores) | `-m 22000` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-13 | 7.1.2 | 34100 | Benchmark: LUKS v2 argon2id + SHA-256 + AES | 1 | 1 H/s | 1, 1, 1, 1 | MSI Intel PTL 30GB | Intel Core Ultra X7 358H @ 4.70GHz (16 Cores) | `-m 34100` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |

**Measurements in this card:** 12 PTS rows. CPU host is shown only as system context; these rows do not constitute CPU-only benchmarks.
