# NVIDIA GH200 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| NVIDIA GH200 144G HBM3e | 6.2.6 | Kerberos 5 + etype 23 + TGS-REP | 3247333333 | 3.2473 GH/s | 86th | 3 | 321455 | [system/hashcat-1.0.x / cd916f36b8c30ecb8bba03c995e8556340b601cc](https://openbenchmarking.org/performance/test/system/hashcat/cd916f36b8c30ecb8bba03c995e8556340b601cc) |
| NVIDIA GH200 144G HBM3e | 6.2.6 | LastPass | 13842700 | 13.843 MH/s | 83rd | 3 | 3236 | [system/hashcat-1.0.x / 36e98a1da0aec289b751c5459a2ae700943a442f](https://openbenchmarking.org/performance/test/system/hashcat/36e98a1da0aec289b751c5459a2ae700943a442f) |
| NVIDIA GH200 144G HBM3e | 6.2.6 | SHA-256 | 14882133333 | 14.882 GH/s | 87th | 3 | 1550269 | [system/hashcat-1.0.x / b6311a7833fd22620b186e0667dd2600d1980264](https://openbenchmarking.org/performance/test/system/hashcat/b6311a7833fd22620b186e0667dd2600d1980264) |
| NVIDIA GH200 144G HBM3e | 6.2.6 | SHA-512 | 4463533333 | 4.4635 GH/s | 86th | 3 | 15179043 | [system/hashcat-1.0.x / b882cb3d8fda94c160446db96187fe1e1fa2496f](https://openbenchmarking.org/performance/test/system/hashcat/b882cb3d8fda94c160446db96187fe1e1fa2496f) |
| NVIDIA GH200 144G HBM3e | 6.2.6 | SHA1 | 38985666667 | 38.986 GH/s | 83rd | 3 | 16908676 | [system/hashcat-1.0.x / 7836cc88bb368389170458a6b54b3c1fc53304de](https://openbenchmarking.org/performance/test/system/hashcat/7836cc88bb368389170458a6b54b3c1fc53304de) |

**Aggregate rows in this card:** 5. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
