# AMD Radeon HD FirePro D700 — Mac Pro v2.01 benchmark fragment

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** 2× FirePro D700, Devices #2 and #3 (Mac Pro 6,1)
- **Версия / Version:** oclHashcat v2.01 (`g952c20e`)
- **Источник / Source:** [Hashcat Forum — benchmark, post #29](https://hashcat.net/forum/post-28623.html)
- **Evidence:** benchmark-mode excerpt. Host Xeon E5-1620 v2 explicitly skipped; per-device rows kept distinct from two-GPU aggregate.
- **Ограничение / Limitation:** partial excerpt of the full mode list; two GPUs are one host/run, not one-device throughput.

| Hash type | Device #2 | Device #3 | Two-GPU aggregate |
|---|---:|---:|---:|
| MD4 | 5153.4 MH/s | 5251.6 MH/s | 10405.1 MH/s |
| MD5 | 4375.7 MH/s | 4409.4 MH/s | 8785.2 MH/s |
| Half MD5 | 3187.2 MH/s | 3187.3 MH/s | 6374.4 MH/s |
| SHA1 | 1910.7 MH/s | 1910.7 MH/s | 3821.4 MH/s |
| SHA256 | 837.5 MH/s | 850.3 MH/s | 1687.8 MH/s |
| SHA512 | 250.7 MH/s | 256.3 MH/s | 507.0 MH/s |
| NTLM | 5181.8 MH/s | 5185.7 MH/s | 10367.5 MH/s |
| bcrypt | 469.6 kH/s | 470.6 kH/s | 940.1 kH/s |

Many more modes appear in the source, including PBKDF2, Office, PDF, LastPass,
1Password and wallet formats. This record supplements the earlier two-mode
excerpt from the same thread; it is a separate run and its values are not merged.
