# AMD Radeon PRO W7900 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| AMD Radeon PRO W7900 | 7.0 | 7-Zip | 1280186 | 1.2802 MH/s | 74th | 7 | 8851 | [hashcat-1.2.x / 80b710251c56bf8e93ef06fbc970f443076e22e0](https://openbenchmarking.org/test/pts/hashcat%26eval%3D80b710251c56bf8e93ef06fbc970f443076e22e0) |
| AMD Radeon PRO W7900 | 7.0 | Kerberos 5 + etype 23 + TGS-REP | 1321079592 | 1.3211 GH/s | 82nd | 7 | 14102508 | [hashcat-1.2.x / 6b1954debb13211e8b6d1b098290c5accf0e374f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6b1954debb13211e8b6d1b098290c5accf0e374f) |
| AMD Radeon PRO W7900 | 7.0 | MD5 | 60685216667 | 60.685 GH/s | 73rd | 7 | 226310010 | [hashcat-1.2.x / 7b7b45c3848e0a5482fb82f220518d5233961430](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7b7b45c3848e0a5482fb82f220518d5233961430) |
| AMD Radeon PRO W7900 | 7.0 | SHA-256 | 11126416667 | 11.126 GH/s | 81st | 7 | 68235876 | [hashcat-1.2.x / 71ae6c8974b17ccdfcf3f872aab62d85c629e59e](https://openbenchmarking.org/test/pts/hashcat%26eval%3D71ae6c8974b17ccdfcf3f872aab62d85c629e59e) |
| AMD Radeon PRO W7900 | 7.0 | SHA-512 | 2943231429 | 2.9432 GH/s | 80th | 7 | 4339660 | [hashcat-1.2.x / 32167b15bfd2349e12bfacbadc31e8396cd4f785](https://openbenchmarking.org/test/pts/hashcat%26eval%3D32167b15bfd2349e12bfacbadc31e8396cd4f785) |
| AMD Radeon PRO W7900 | 7.0 | SHA1 | 26138209524 | 26.138 GH/s | 79th | 7 | 99846848 | [hashcat-1.2.x / 00d12c5cd061174be3e1233b616aaff5e3f9bd4f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D00d12c5cd061174be3e1233b616aaff5e3f9bd4f) |
| AMD Radeon PRO W7900 | 7.0 | TrueCrypt RIPEMD160 + XTS | 828811 | 828.81 kH/s | 78th | 7 | 3787 | [hashcat-1.2.x / 44bfe79903c83521447b7e56f6f948edf4dbc1cf](https://openbenchmarking.org/test/pts/hashcat%26eval%3D44bfe79903c83521447b7e56f6f948edf4dbc1cf) |
| AMD Radeon PRO W7900 | 7.1.2 | 7-Zip | 1269535 | 1.2695 MH/s | 75th | 4 | 4371 | [hashcat-1.3.x / dd3830ac8f396d5aeb2c788ccf63196ccfe6b785](https://openbenchmarking.org/test/pts/hashcat%26eval%3Ddd3830ac8f396d5aeb2c788ccf63196ccfe6b785) |
| AMD Radeon PRO W7900 | 7.1.2 | Kerberos 5 + etype 23 + TGS-REP | 1356428572 | 1.3564 GH/s | 71st | 5 | 4909942 | [hashcat-1.3.x / 89adea9de254c520e2999634807af2397c2da2c3](https://openbenchmarking.org/test/pts/hashcat%26eval%3D89adea9de254c520e2999634807af2397c2da2c3) |
| AMD Radeon PRO W7900 | 7.1.2 | LastPass | 46212 | 46.212 kH/s | 75th | 5 | 142 | [hashcat-1.3.x / 82bc713652e59980e398283abaaf76352af9bb0c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D82bc713652e59980e398283abaaf76352af9bb0c) |
| AMD Radeon PRO W7900 | 7.1.2 | NTLM | 86211680000 | 86.212 GH/s | 59th | 3 | 777760095 | [hashcat-1.3.x / a21d6e2b0f86d6fd008776a0dbcd84258d25b266](https://openbenchmarking.org/test/pts/hashcat%26eval%3Da21d6e2b0f86d6fd008776a0dbcd84258d25b266) |
| AMD Radeon PRO W7900 | 7.1.2 | SHA-256 | 11071786000 | 11.072 GH/s | 71st | 5 | 121643703 | [hashcat-1.3.x / bb70ab4002871eaf41c4c257184d478de05cb604](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dbb70ab4002871eaf41c4c257184d478de05cb604) |
| AMD Radeon PRO W7900 | 7.1.2 | SHA-512 | 2902280000 | 2.9023 GH/s | 68th | 5 | 20210962 | [hashcat-1.3.x / ec680f525d7a44fb1c765bf8f3508874a039743e](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dec680f525d7a44fb1c765bf8f3508874a039743e) |
| AMD Radeon PRO W7900 | 7.1.2 | SHA1 | 26050551667 | 26.051 GH/s | 70th | 4 | 339791803 | [hashcat-1.3.x / eff31b43dba5f679500a7b4a9d777e74ae74d575](https://openbenchmarking.org/test/pts/hashcat%26eval%3Deff31b43dba5f679500a7b4a9d777e74ae74d575) |
| AMD Radeon PRO W7900 | 7.1.2 | TrueCrypt RIPEMD160 + XTS | 874832 | 874.83 kH/s | 70th | 5 | 4776 | [hashcat-1.3.x / 152ac6b8c7471c32a080a40569d381f6f87925f7](https://openbenchmarking.org/test/pts/hashcat%26eval%3D152ac6b8c7471c32a080a40569d381f6f87925f7) |
| AMD Radeon PRO W7900 | 7.1.2 | WPA-PBKDF2-PMKID+EAPOL | 1310296 | 1.3103 MH/s | 73rd | 5 | 5401 | [hashcat-1.3.x / 6ec0566c352e7ce9cee334cd480808fd993aa913](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6ec0566c352e7ce9cee334cd480808fd993aa913) |
| AMD Radeon PRO W7900 | 7.1.2 | bcrypt | 96774 | 96.774 kH/s | 72nd | 3 | 48 | [hashcat-1.3.x / e0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd](https://openbenchmarking.org/test/pts/hashcat%26eval%3De0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd) |

**Aggregate rows in this card:** 17. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
