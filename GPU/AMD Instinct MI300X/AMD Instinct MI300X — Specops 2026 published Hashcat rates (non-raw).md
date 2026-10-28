# AMD Instinct MI300X — Specops 2026 published Hashcat rates

- **Evidence type:** independently published Hashcat performance table; **not raw Hashcat stdout** and not a PTS aggregate.
- **Run details:** the article identifies Hashcat and five algorithms, but does not publish the Hashcat version, command line, device count, or console output. Treat these as reported rates, not reproducible `hashcat -b` output.
- **GPU identification:** AMD Instinct MI300X, as named in the report.
- **Source:** [BleepingComputer report on Specops research (2026-04-08)](https://www.bleepingcomputer.com/news/security/is-a-30-000-gpu-good-at-password-cracking/)

| Hash type | Hashcat mode (where unambiguous) | Reported speed |
|---|---:|---:|
| MD5 | 0 | 164.1 GH/s |
| NTLM | 1000 | 268.5 GH/s |
| bcrypt | 3200 | 142.3 kH/s |
| SHA-256 | 1400 | 24,673.6 MH/s |
| SHA-512 | 1700 | 8,771.4 MH/s |

**Classification:** published algorithm-rate results, but no raw text, exact benchmark flags, or per-device `Speed.#N` lines. Do not merge with the separate MI300X v6.2.6 raw run in this folder.
