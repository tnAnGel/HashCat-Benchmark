# AMD Radeon 8060S — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| AMD Radeon 8060S | 7.0 | 7-Zip | 695267 | 695.27 kH/s | 52nd | 4 | 75562 | [hashcat-1.2.x / 80b710251c56bf8e93ef06fbc970f443076e22e0](https://openbenchmarking.org/test/pts/hashcat%26eval%3D80b710251c56bf8e93ef06fbc970f443076e22e0) |
| AMD Radeon 8060S | 7.0 | Kerberos 5 + etype 23 + TGS-REP | 489541667 | 489.54 MH/s | 51st | 4 | 4473244 | [hashcat-1.2.x / 6b1954debb13211e8b6d1b098290c5accf0e374f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6b1954debb13211e8b6d1b098290c5accf0e374f) |
| AMD Radeon 8060S | 7.0 | MD5 | 31493941667 | 31.494 GH/s | 50th | 4 | 2793642089 | [hashcat-1.2.x / 7b7b45c3848e0a5482fb82f220518d5233961430](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7b7b45c3848e0a5482fb82f220518d5233961430) |
| AMD Radeon 8060S | 7.0 | SHA-256 | 5403741667 | 5.4037 GH/s | 50th | 4 | 149335894 | [hashcat-1.2.x / 71ae6c8974b17ccdfcf3f872aab62d85c629e59e](https://openbenchmarking.org/test/pts/hashcat%26eval%3D71ae6c8974b17ccdfcf3f872aab62d85c629e59e) |
| AMD Radeon 8060S | 7.0 | SHA-512 | 1163183334 | 1.1632 GH/s | 48th | 4 | 30212341 | [hashcat-1.2.x / 32167b15bfd2349e12bfacbadc31e8396cd4f785](https://openbenchmarking.org/test/pts/hashcat%26eval%3D32167b15bfd2349e12bfacbadc31e8396cd4f785) |
| AMD Radeon 8060S | 7.0 | SHA1 | 12828575000 | 12.829 GH/s | 42nd | 4 | 740239539 | [hashcat-1.2.x / 00d12c5cd061174be3e1233b616aaff5e3f9bd4f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D00d12c5cd061174be3e1233b616aaff5e3f9bd4f) |
| AMD Radeon 8060S | 7.0 | TrueCrypt RIPEMD160 + XTS | 433733 | 433.73 kH/s | 59th | 4 | 14988 | [hashcat-1.2.x / 44bfe79903c83521447b7e56f6f948edf4dbc1cf](https://openbenchmarking.org/test/pts/hashcat%26eval%3D44bfe79903c83521447b7e56f6f948edf4dbc1cf) |
| AMD Radeon 8060S | 7.1.2 | MD5 | 26675544445 | 26.676 GH/s | 39th | 3 | 2205708320 | [hashcat-1.3.x / 2f1e49c858bdaf551168a2c36422c3bcd6dbf083](https://openbenchmarking.org/test/pts/hashcat%26eval%3D2f1e49c858bdaf551168a2c36422c3bcd6dbf083) |
| AMD Radeon 8060S | 7.1.2 | bcrypt | 38617 | 38.617 kH/s | 45th | 3 | 1887 | [hashcat-1.3.x / e0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd](https://openbenchmarking.org/test/pts/hashcat%26eval%3De0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd) |

**Aggregate rows in this card:** 9. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
