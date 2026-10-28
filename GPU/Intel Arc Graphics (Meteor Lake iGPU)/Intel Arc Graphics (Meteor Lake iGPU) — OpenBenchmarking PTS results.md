# Intel Arc Graphics (Meteor Lake iGPU) — OpenBenchmarking Hashcat measurements (partial, no stdout)

- **Evidence:** PTS-published individual benchmark values; no raw Hashcat console stdout is available from these result exports.
- **PTS runner:** profile executes `hashcat -b --benchmark-min=30` with the per-mode arguments below.
- **Values:** exact PTS mean in H/s and exact repeat values when PTS publishes them. A PTS repeat is not a copied `Speed.#N` console line.
- **Hardware:** exact PTS graphics descriptor is kept per row; aliases are explained in the note below.

> PTS identifies a Meteor Lake integrated Arc graphics device, not a discrete retail SKU.

| Date | Hashcat | Mode | Benchmark | Mean (H/s) | Readable speed | PTS repeat values (H/s) | PTS GPU label | CPU host context | Args | Result |
|---|---|---:|---|---:|---:|---|---|---|---|---|
| 2026-02-15 | 7.1.2 | 0 | Benchmark: MD5 | 10099016667 | 10.1 GH/s | 10343700000, 10161400000, 10072800000, 9945500000, 9982700000, 10088000000 | Intel Arc MTL 15GB | Intel Core Ultra 7 155H @ 4.80GHz (16 Cores / 22 Threads) | `-m 0` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-15 | 7.1.2 | 100 | Benchmark: SHA1 | 3619200000 | 3.619 GH/s | 3771700000, 3600100000, 3506400000, 3640100000, 3618800000, 3578100000 | Intel Arc MTL 15GB | Intel Core Ultra 7 155H @ 4.80GHz (16 Cores / 22 Threads) | `-m 100` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-15 | 7.1.2 | 1000 | Benchmark: NTLM | 17626766667 | 17.63 GH/s | 17917400000, 17493600000, 17675300000, 17633600000, 17584400000, 17456300000 | Intel Arc MTL 15GB | Intel Core Ultra 7 155H @ 4.80GHz (16 Cores / 22 Threads) | `-m 1000` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-15 | 7.1.2 | 1400 | Benchmark: SHA-256 | 1620300000 | 1.62 GH/s | 1671200000, 1600800000, 1621300000, 1627600000, 1580600000 | Intel Arc MTL 15GB | Intel Core Ultra 7 155H @ 4.80GHz (16 Cores / 22 Threads) | `-m 1400` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-15 | 7.1.2 | 1700 | Benchmark: SHA-512 | 282525000 | 282.5 MH/s | 291000000, 285100000, 278500000, 275500000 | Intel Arc MTL 15GB | Intel Core Ultra 7 155H @ 4.80GHz (16 Cores / 22 Threads) | `-m 1700` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-15 | 7.1.2 | 3200 | Benchmark: bcrypt | 4221 | 4.221 kH/s | 4219, 4220, 4219, 4224, 4225 | Intel Arc MTL 15GB | Intel Core Ultra 7 155H @ 4.80GHz (16 Cores / 22 Threads) | `-m 3200` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-15 | 7.1.2 | 6211 | Benchmark: TrueCrypt RIPEMD160 + XTS | 87157 | 87.16 kH/s | 93929, 88558, 88969, 82370, 87309, 82973, 87998, 86292, 88400, 87428, 87765, 82911, 86244, 87908, 88299 | Intel Arc MTL 15GB | Intel Core Ultra 7 155H @ 4.80GHz (16 Cores / 22 Threads) | `-m 6211` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-15 | 7.1.2 | 6800 | Benchmark: LastPass | 5340 | 5.34 kH/s | 5427, 5268, 5329, 5334 | Intel Arc MTL 15GB | Intel Core Ultra 7 155H @ 4.80GHz (16 Cores / 22 Threads) | `-m 6800` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-15 | 7.1.2 | 11600 | Benchmark: 7-Zip | 53351 | 53.35 kH/s | 51986, 52679, 54313, 53522, 54256 | Intel Arc MTL 15GB | Intel Core Ultra 7 155H @ 4.80GHz (16 Cores / 22 Threads) | `-m 11600` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-15 | 7.1.2 | 13100 | Benchmark: Kerberos 5 + etype 23 + TGS-REP | 77321243 | 77.32 MH/s | 77194200, 77524900, 77342300, 77360200, 77379400, 77301000, 77146700 | Intel Arc MTL 15GB | Intel Core Ultra 7 155H @ 4.80GHz (16 Cores / 22 Threads) | `-m 13100` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-15 | 7.1.2 | 22000 | Benchmark: WPA-PBKDF2-PMKID+EAPOL | 170833 | 170.8 kH/s | 177900, 183900, 167200, 183400, 169200, 169900, 168000, 169900, 170900, 168500, 165300, 166200, 168700, 167300, 166200 | Intel Arc MTL 15GB | Intel Core Ultra 7 155H @ 4.80GHz (16 Cores / 22 Threads) | `-m 22000` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |
| 2026-02-15 | 7.1.2 | 34100 | Benchmark: LUKS v2 argon2id + SHA-256 + AES | 0 | 0 H/s | not provided (single PTS value) | Intel Arc MTL 15GB | Intel Core Ultra 7 155H @ 4.80GHz (16 Cores / 22 Threads) | `-m 34100` | [2602155-NE-2602153NE79](https://openbenchmarking.org/result/2602155-NE-2602153NE79) |

**Measurements in this card:** 12 PTS rows. CPU host is shown only as system context; these rows do not constitute CPU-only benchmarks.
