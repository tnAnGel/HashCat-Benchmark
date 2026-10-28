# Intel Arc Pro B50 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| Intel Arc Pro B50 BMG G21 | 7.0 | Kerberos 5 + etype 23 + TGS-REP | 180670635 | 180.67 MH/s | 15th | 3 | 860906 | [hashcat-1.2.x / 6b1954debb13211e8b6d1b098290c5accf0e374f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6b1954debb13211e8b6d1b098290c5accf0e374f) |
| Intel Arc Pro B50 BMG G21 | 7.0 | SHA-256 | 2535022222 | 2.535 GH/s | 20th | 3 | 10702094 | [hashcat-1.2.x / 71ae6c8974b17ccdfcf3f872aab62d85c629e59e](https://openbenchmarking.org/test/pts/hashcat%26eval%3D71ae6c8974b17ccdfcf3f872aab62d85c629e59e) |
| Intel Arc Pro B50 BMG G21 | 7.0 | SHA-512 | 370900000 | 370.9 MH/s | 10th | 3 | 1047616 | [hashcat-1.2.x / 32167b15bfd2349e12bfacbadc31e8396cd4f785](https://openbenchmarking.org/test/pts/hashcat%26eval%3D32167b15bfd2349e12bfacbadc31e8396cd4f785) |
| Intel Arc Pro B50 BMG G21 | 7.0 | SHA1 | 7337622222 | 7.3376 GH/s | 17th | 3 | 105299668 | [hashcat-1.2.x / 00d12c5cd061174be3e1233b616aaff5e3f9bd4f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D00d12c5cd061174be3e1233b616aaff5e3f9bd4f) |
| Intel Arc Pro B50 BMG G21 | 7.0 | TrueCrypt RIPEMD160 + XTS | 211208 | 211.21 kH/s | 11th | 3 | 3997 | [hashcat-1.2.x / 44bfe79903c83521447b7e56f6f948edf4dbc1cf](https://openbenchmarking.org/test/pts/hashcat%26eval%3D44bfe79903c83521447b7e56f6f948edf4dbc1cf) |
| Intel Arc Pro B50 BMG G21 | 7.1.2 | 7-Zip | 134429 | 134.43 kH/s | 17th | 4 | 4508 | [hashcat-1.3.x / dd3830ac8f396d5aeb2c788ccf63196ccfe6b785](https://openbenchmarking.org/test/pts/hashcat%26eval%3Ddd3830ac8f396d5aeb2c788ccf63196ccfe6b785) |
| Intel Arc Pro B50 BMG G21 | 7.1.2 | Kerberos 5 + etype 23 + TGS-REP | 199590000 | 199.59 MH/s | 20th | 4 | 127017 | [hashcat-1.3.x / 89adea9de254c520e2999634807af2397c2da2c3](https://openbenchmarking.org/test/pts/hashcat%26eval%3D89adea9de254c520e2999634807af2397c2da2c3) |
| Intel Arc Pro B50 BMG G21 | 7.1.2 | LastPass | 11116 | 11.116 kH/s | 27th | 4 | 58 | [hashcat-1.3.x / 82bc713652e59980e398283abaaf76352af9bb0c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D82bc713652e59980e398283abaaf76352af9bb0c) |
| Intel Arc Pro B50 BMG G21 | 7.1.2 | NTLM | 29609330000 | 29.609 GH/s | 26th | 4 | 205502055 | [hashcat-1.3.x / a21d6e2b0f86d6fd008776a0dbcd84258d25b266](https://openbenchmarking.org/test/pts/hashcat%26eval%3Da21d6e2b0f86d6fd008776a0dbcd84258d25b266) |
| Intel Arc Pro B50 BMG G21 | 7.1.2 | SHA-256 | 2571556667 | 2.5716 GH/s | 25th | 4 | 16947155 | [hashcat-1.3.x / bb70ab4002871eaf41c4c257184d478de05cb604](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dbb70ab4002871eaf41c4c257184d478de05cb604) |
| Intel Arc Pro B50 BMG G21 | 7.1.2 | SHA1 | 7291356667 | 7.2914 GH/s | 25th | 4 | 73412011 | [hashcat-1.3.x / eff31b43dba5f679500a7b4a9d777e74ae74d575](https://openbenchmarking.org/test/pts/hashcat%26eval%3Deff31b43dba5f679500a7b4a9d777e74ae74d575) |
| Intel Arc Pro B50 BMG G21 | 7.1.2 | TrueCrypt RIPEMD160 + XTS | 212884 | 212.88 kH/s | 24th | 4 | 596 | [hashcat-1.3.x / 152ac6b8c7471c32a080a40569d381f6f87925f7](https://openbenchmarking.org/test/pts/hashcat%26eval%3D152ac6b8c7471c32a080a40569d381f6f87925f7) |
| Intel Arc Pro B50 BMG G21 | 7.1.2 | WPA-PBKDF2-PMKID+EAPOL | 360263 | 360.26 kH/s | 26th | 4 | 274 | [hashcat-1.3.x / 6ec0566c352e7ce9cee334cd480808fd993aa913](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6ec0566c352e7ce9cee334cd480808fd993aa913) |
| Intel Arc Pro B50 BMG G21 | 7.1.2 | bcrypt | 17747 | 17.747 kH/s | 27th | 4 | 9 | [hashcat-1.3.x / e0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd](https://openbenchmarking.org/test/pts/hashcat%26eval%3De0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd) |

**Aggregate rows in this card:** 14. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
