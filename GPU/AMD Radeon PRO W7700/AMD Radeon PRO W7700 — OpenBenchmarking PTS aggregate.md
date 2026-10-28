# AMD Radeon PRO W7700 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| AMD Radeon PRO W7700 | 6.2.4 | 7-Zip | 685809 | 685.81 kH/s | 41st | 7 | 4935 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| AMD Radeon PRO W7700 | 6.2.4 | MD5 | 33350840000 | 33.351 GH/s | 39th | 7 | 37332242 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| AMD Radeon PRO W7700 | 6.2.4 | SHA-512 | 822158601 | 822.16 MH/s | 20th | 7 | 4604956 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| AMD Radeon PRO W7700 | 6.2.4 | SHA1 | 14150885714 | 14.151 GH/s | 46th | 7 | 48138046 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| AMD Radeon PRO W7700 | 7.0 | 7-Zip | 658089 | 658.09 kH/s | 48th | 3 | 2174 | [hashcat-1.2.x / 80b710251c56bf8e93ef06fbc970f443076e22e0](https://openbenchmarking.org/test/pts/hashcat%26eval%3D80b710251c56bf8e93ef06fbc970f443076e22e0) |
| AMD Radeon PRO W7700 | 7.0 | Kerberos 5 + etype 23 + TGS-REP | 626287500 | 626.29 MH/s | 66th | 4 | 2625952 | [hashcat-1.2.x / 6b1954debb13211e8b6d1b098290c5accf0e374f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6b1954debb13211e8b6d1b098290c5accf0e374f) |
| AMD Radeon PRO W7700 | 7.0 | MD5 | 30492555556 | 30.493 GH/s | 45th | 3 | 207364256 | [hashcat-1.2.x / 7b7b45c3848e0a5482fb82f220518d5233961430](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7b7b45c3848e0a5482fb82f220518d5233961430) |
| AMD Radeon PRO W7700 | 7.0 | SHA-256 | 5649212500 | 5.6492 GH/s | 53rd | 4 | 11912539 | [hashcat-1.2.x / 71ae6c8974b17ccdfcf3f872aab62d85c629e59e](https://openbenchmarking.org/test/pts/hashcat%26eval%3D71ae6c8974b17ccdfcf3f872aab62d85c629e59e) |
| AMD Radeon PRO W7700 | 7.0 | SHA-512 | 1474629167 | 1.4746 GH/s | 61st | 4 | 1217646 | [hashcat-1.2.x / 32167b15bfd2349e12bfacbadc31e8396cd4f785](https://openbenchmarking.org/test/pts/hashcat%26eval%3D32167b15bfd2349e12bfacbadc31e8396cd4f785) |
| AMD Radeon PRO W7700 | 7.0 | SHA1 | 13107233333 | 13.107 GH/s | 43rd | 4 | 40570893 | [hashcat-1.2.x / 00d12c5cd061174be3e1233b616aaff5e3f9bd4f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D00d12c5cd061174be3e1233b616aaff5e3f9bd4f) |
| AMD Radeon PRO W7700 | 7.0 | TrueCrypt RIPEMD160 + XTS | 413171 | 413.17 kH/s | 51st | 4 | 181 | [hashcat-1.2.x / 44bfe79903c83521447b7e56f6f948edf4dbc1cf](https://openbenchmarking.org/test/pts/hashcat%26eval%3D44bfe79903c83521447b7e56f6f948edf4dbc1cf) |

**Aggregate rows in this card:** 11. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
