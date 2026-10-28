# Intel Arc B580 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| Intel Arc B580 BMG G21 | 7.0 | Kerberos 5 + etype 23 + TGS-REP | 263742857 | 263.74 MH/s | 29th | 7 | 297266 | [hashcat-1.2.x / 6b1954debb13211e8b6d1b098290c5accf0e374f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6b1954debb13211e8b6d1b098290c5accf0e374f) |
| Intel Arc B580 BMG G21 | 7.0 | MD5 | 26926421429 | 26.926 GH/s | 31st | 7 | 2970674317 | [hashcat-1.2.x / 7b7b45c3848e0a5482fb82f220518d5233961430](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7b7b45c3848e0a5482fb82f220518d5233961430) |
| Intel Arc B580 BMG G21 | 7.0 | SHA-256 | 4252108333 | 4.2521 GH/s | 33rd | 8 | 164138210 | [hashcat-1.2.x / 71ae6c8974b17ccdfcf3f872aab62d85c629e59e](https://openbenchmarking.org/test/pts/hashcat%26eval%3D71ae6c8974b17ccdfcf3f872aab62d85c629e59e) |
| Intel Arc B580 BMG G21 | 7.0 | SHA-512 | 613285833 | 613.29 MH/s | 20th | 8 | 63162484 | [hashcat-1.2.x / 32167b15bfd2349e12bfacbadc31e8396cd4f785](https://openbenchmarking.org/test/pts/hashcat%26eval%3D32167b15bfd2349e12bfacbadc31e8396cd4f785) |
| Intel Arc B580 BMG G21 | 7.0 | SHA1 | 13480516667 | 13.481 GH/s | 45th | 8 | 1925036424 | [hashcat-1.2.x / 00d12c5cd061174be3e1233b616aaff5e3f9bd4f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D00d12c5cd061174be3e1233b616aaff5e3f9bd4f) |
| Intel Arc B580 BMG G21 | 7.0 | TrueCrypt RIPEMD160 + XTS | 398252 | 398.25 kH/s | 42nd | 8 | 36669 | [hashcat-1.2.x / 44bfe79903c83521447b7e56f6f948edf4dbc1cf](https://openbenchmarking.org/test/pts/hashcat%26eval%3D44bfe79903c83521447b7e56f6f948edf4dbc1cf) |
| Intel Arc B580 BMG G21 | 7.1.2 | 7-Zip | 230633 | 230.63 kH/s | 26th | 6 | 1552 | [hashcat-1.3.x / dd3830ac8f396d5aeb2c788ccf63196ccfe6b785](https://openbenchmarking.org/test/pts/hashcat%26eval%3Ddd3830ac8f396d5aeb2c788ccf63196ccfe6b785) |
| Intel Arc B580 BMG G21 | 7.1.2 | Kerberos 5 + etype 23 + TGS-REP | 318322222 | 318.32 MH/s | 30th | 6 | 20460353 | [hashcat-1.3.x / 89adea9de254c520e2999634807af2397c2da2c3](https://openbenchmarking.org/test/pts/hashcat%26eval%3D89adea9de254c520e2999634807af2397c2da2c3) |
| Intel Arc B580 BMG G21 | 7.1.2 | LUKS v2 argon2id + SHA-256 + AES | 2 | 2 H/s | 28th | 3 | — | [hashcat-1.3.x / 0b5d0c3db0c27a2a6e025024f7e154886882d515](https://openbenchmarking.org/test/pts/hashcat%26eval%3D0b5d0c3db0c27a2a6e025024f7e154886882d515) |
| Intel Arc B580 BMG G21 | 7.1.2 | LastPass | 20714 | 20.714 kH/s | 39th | 6 | 126 | [hashcat-1.3.x / 82bc713652e59980e398283abaaf76352af9bb0c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D82bc713652e59980e398283abaaf76352af9bb0c) |
| Intel Arc B580 BMG G21 | 7.1.2 | MD5 | 28062516667 | 28.063 GH/s | 41st | 4 | 97899361 | [hashcat-1.3.x / 2f1e49c858bdaf551168a2c36422c3bcd6dbf083](https://openbenchmarking.org/test/pts/hashcat%26eval%3D2f1e49c858bdaf551168a2c36422c3bcd6dbf083) |
| Intel Arc B580 BMG G21 | 7.1.2 | NTLM | 47699877778 | 47.7 GH/s | 34th | 6 | 51185713 | [hashcat-1.3.x / a21d6e2b0f86d6fd008776a0dbcd84258d25b266](https://openbenchmarking.org/test/pts/hashcat%26eval%3Da21d6e2b0f86d6fd008776a0dbcd84258d25b266) |
| Intel Arc B580 BMG G21 | 7.1.2 | SHA-256 | 4304411111 | 4.3044 GH/s | 32nd | 6 | 3568297 | [hashcat-1.3.x / bb70ab4002871eaf41c4c257184d478de05cb604](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dbb70ab4002871eaf41c4c257184d478de05cb604) |
| Intel Arc B580 BMG G21 | 7.1.2 | SHA1 | 14104388889 | 14.104 GH/s | 41st | 6 | 47547518 | [hashcat-1.3.x / eff31b43dba5f679500a7b4a9d777e74ae74d575](https://openbenchmarking.org/test/pts/hashcat%26eval%3Deff31b43dba5f679500a7b4a9d777e74ae74d575) |
| Intel Arc B580 BMG G21 | 7.1.2 | TrueCrypt RIPEMD160 + XTS | 412478 | 412.48 kH/s | 36th | 6 | 345 | [hashcat-1.3.x / 152ac6b8c7471c32a080a40569d381f6f87925f7](https://openbenchmarking.org/test/pts/hashcat%26eval%3D152ac6b8c7471c32a080a40569d381f6f87925f7) |
| Intel Arc B580 BMG G21 | 7.1.2 | WPA-PBKDF2-PMKID+EAPOL | 688611 | 688.61 kH/s | 41st | 6 | 2829 | [hashcat-1.3.x / 6ec0566c352e7ce9cee334cd480808fd993aa913](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6ec0566c352e7ce9cee334cd480808fd993aa913) |
| Intel Arc B580 BMG G21 | 7.1.2 | bcrypt | 22225 | 22.225 kH/s | 32nd | 6 | 30 | [hashcat-1.3.x / e0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd](https://openbenchmarking.org/test/pts/hashcat%26eval%3De0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd) |

**Aggregate rows in this card:** 17. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
