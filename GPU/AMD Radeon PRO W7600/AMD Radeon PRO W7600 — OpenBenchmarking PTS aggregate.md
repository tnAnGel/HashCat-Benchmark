# AMD Radeon PRO W7600 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| AMD Radeon PRO W7600 | 6.2.4 | 7-Zip | 468950 | 468.95 kH/s | 25th | 3 | — | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| AMD Radeon PRO W7600 | 6.2.4 | MD5 | 21318020000 | 21.318 GH/s | 19th | 3 | — | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| AMD Radeon PRO W7600 | 6.2.4 | SHA-512 | 536854756 | 536.85 MH/s | 13th | 3 | — | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| AMD Radeon PRO W7600 | 6.2.4 | SHA1 | 8932200000 | 8.9322 GH/s | 26th | 3 | — | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| AMD Radeon PRO W7600 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 281117 | 281.12 kH/s | 14th | 3 | — | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |
| AMD Radeon PRO W7600 | 7.0 | Kerberos 5 + etype 23 + TGS-REP | 403866666 | 403.87 MH/s | 45th | 3 | 461880 | [hashcat-1.2.x / 6b1954debb13211e8b6d1b098290c5accf0e374f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6b1954debb13211e8b6d1b098290c5accf0e374f) |
| AMD Radeon PRO W7600 | 7.0 | SHA-256 | 3539694444 | 3.5397 GH/s | 28th | 3 | 1799408 | [hashcat-1.2.x / 71ae6c8974b17ccdfcf3f872aab62d85c629e59e](https://openbenchmarking.org/test/pts/hashcat%26eval%3D71ae6c8974b17ccdfcf3f872aab62d85c629e59e) |
| AMD Radeon PRO W7600 | 7.0 | SHA-512 | 915111111 | 915.11 MH/s | 35th | 3 | 789046 | [hashcat-1.2.x / 32167b15bfd2349e12bfacbadc31e8396cd4f785](https://openbenchmarking.org/test/pts/hashcat%26eval%3D32167b15bfd2349e12bfacbadc31e8396cd4f785) |
| AMD Radeon PRO W7600 | 7.0 | SHA1 | 8196761111 | 8.1968 GH/s | 25th | 3 | 3069579 | [hashcat-1.2.x / 00d12c5cd061174be3e1233b616aaff5e3f9bd4f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D00d12c5cd061174be3e1233b616aaff5e3f9bd4f) |
| AMD Radeon PRO W7600 | 7.0 | TrueCrypt RIPEMD160 + XTS | 264289 | 264.29 kH/s | 18th | 3 | 712 | [hashcat-1.2.x / 44bfe79903c83521447b7e56f6f948edf4dbc1cf](https://openbenchmarking.org/test/pts/hashcat%26eval%3D44bfe79903c83521447b7e56f6f948edf4dbc1cf) |

**Aggregate rows in this card:** 10. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
