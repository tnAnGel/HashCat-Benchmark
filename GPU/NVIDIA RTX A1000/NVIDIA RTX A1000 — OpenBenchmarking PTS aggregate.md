# NVIDIA RTX A1000 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| NVIDIA RTX A1000 | 6.2.4 | 7-Zip | 219405 | 219.41 kH/s | 6th | 7 | 1133 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| NVIDIA RTX A1000 | 6.2.4 | MD5 | 12973616667 | 12.974 GH/s | 12th | 7 | 115781944 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| NVIDIA RTX A1000 | 6.2.4 | SHA-512 | 537495238 | 537.5 MH/s | 14th | 7 | 3891749 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| NVIDIA RTX A1000 | 6.2.4 | SHA1 | 4293100000 | 4.2931 GH/s | 11th | 7 | 31217516 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| NVIDIA RTX A1000 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 153844 | 153.84 kH/s | 6th | 7 | 8199 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |
| NVIDIA RTX A1000 | 7.0 | 7-Zip | 224413 | 224.41 kH/s | 9th | 4 | 2098 | [hashcat-1.2.x / 80b710251c56bf8e93ef06fbc970f443076e22e0](https://openbenchmarking.org/test/pts/hashcat%26eval%3D80b710251c56bf8e93ef06fbc970f443076e22e0) |
| NVIDIA RTX A1000 | 7.0 | Kerberos 5 + etype 23 + TGS-REP | 257540000 | 257.54 MH/s | 26th | 5 | 5020757 | [hashcat-1.2.x / 6b1954debb13211e8b6d1b098290c5accf0e374f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6b1954debb13211e8b6d1b098290c5accf0e374f) |
| NVIDIA RTX A1000 | 7.0 | MD5 | 12948862500 | 12.949 GH/s | 12th | 4 | 116744060 | [hashcat-1.2.x / 7b7b45c3848e0a5482fb82f220518d5233961430](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7b7b45c3848e0a5482fb82f220518d5233961430) |
| NVIDIA RTX A1000 | 7.0 | SHA-256 | 1823177333 | 1.8232 GH/s | 10th | 5 | 43444559 | [hashcat-1.2.x / 71ae6c8974b17ccdfcf3f872aab62d85c629e59e](https://openbenchmarking.org/test/pts/hashcat%26eval%3D71ae6c8974b17ccdfcf3f872aab62d85c629e59e) |
| NVIDIA RTX A1000 | 7.0 | SHA-512 | 613390667 | 613.39 MH/s | 20th | 5 | 5130981 | [hashcat-1.2.x / 32167b15bfd2349e12bfacbadc31e8396cd4f785](https://openbenchmarking.org/test/pts/hashcat%26eval%3D32167b15bfd2349e12bfacbadc31e8396cd4f785) |
| NVIDIA RTX A1000 | 7.0 | SHA1 | 4376473333 | 4.3765 GH/s | 11th | 5 | 217985449 | [hashcat-1.2.x / 00d12c5cd061174be3e1233b616aaff5e3f9bd4f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D00d12c5cd061174be3e1233b616aaff5e3f9bd4f) |
| NVIDIA RTX A1000 | 7.0 | TrueCrypt RIPEMD160 + XTS | 164715 | 164.72 kH/s | 8th | 5 | 1479 | [hashcat-1.2.x / 44bfe79903c83521447b7e56f6f948edf4dbc1cf](https://openbenchmarking.org/test/pts/hashcat%26eval%3D44bfe79903c83521447b7e56f6f948edf4dbc1cf) |
| NVIDIA RTX A1000 | 7.1.2 | 7-Zip | 224455 | 224.46 kH/s | 24th | 3 | 991 | [hashcat-1.3.x / dd3830ac8f396d5aeb2c788ccf63196ccfe6b785](https://openbenchmarking.org/test/pts/hashcat%26eval%3Ddd3830ac8f396d5aeb2c788ccf63196ccfe6b785) |
| NVIDIA RTX A1000 | 7.1.2 | Kerberos 5 + etype 23 + TGS-REP | 269833333 | 269.83 MH/s | 26th | 3 | 230940 | [hashcat-1.3.x / 89adea9de254c520e2999634807af2397c2da2c3](https://openbenchmarking.org/test/pts/hashcat%26eval%3D89adea9de254c520e2999634807af2397c2da2c3) |
| NVIDIA RTX A1000 | 7.1.2 | LastPass | 7589 | 7.589 kH/s | 21st | 3 | 27 | [hashcat-1.3.x / 82bc713652e59980e398283abaaf76352af9bb0c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D82bc713652e59980e398283abaaf76352af9bb0c) |
| NVIDIA RTX A1000 | 7.1.2 | NTLM | 21315322222 | 21.315 GH/s | 20th | 3 | 33149528 | [hashcat-1.3.x / a21d6e2b0f86d6fd008776a0dbcd84258d25b266](https://openbenchmarking.org/test/pts/hashcat%26eval%3Da21d6e2b0f86d6fd008776a0dbcd84258d25b266) |
| NVIDIA RTX A1000 | 7.1.2 | SHA-256 | 1769453333 | 1.7695 GH/s | 19th | 3 | 4110734 | [hashcat-1.3.x / bb70ab4002871eaf41c4c257184d478de05cb604](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dbb70ab4002871eaf41c4c257184d478de05cb604) |
| NVIDIA RTX A1000 | 7.1.2 | SHA-512 | 615206667 | 615.21 MH/s | 24th | 3 | 773649 | [hashcat-1.3.x / ec680f525d7a44fb1c765bf8f3508874a039743e](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dec680f525d7a44fb1c765bf8f3508874a039743e) |
| NVIDIA RTX A1000 | 7.1.2 | SHA1 | 4786555555 | 4.7866 GH/s | 19th | 3 | 8525539 | [hashcat-1.3.x / eff31b43dba5f679500a7b4a9d777e74ae74d575](https://openbenchmarking.org/test/pts/hashcat%26eval%3Deff31b43dba5f679500a7b4a9d777e74ae74d575) |
| NVIDIA RTX A1000 | 7.1.2 | TrueCrypt RIPEMD160 + XTS | 165600 | 165.6 kH/s | 19th | 3 | 693 | [hashcat-1.3.x / 152ac6b8c7471c32a080a40569d381f6f87925f7](https://openbenchmarking.org/test/pts/hashcat%26eval%3D152ac6b8c7471c32a080a40569d381f6f87925f7) |
| NVIDIA RTX A1000 | 7.1.2 | WPA-PBKDF2-PMKID+EAPOL | 226827 | 226.83 kH/s | 19th | 3 | 843 | [hashcat-1.3.x / 6ec0566c352e7ce9cee334cd480808fd993aa913](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6ec0566c352e7ce9cee334cd480808fd993aa913) |
| NVIDIA RTX A1000 | 7.1.2 | bcrypt | 23497 | 23.497 kH/s | 33rd | 3 | 98 | [hashcat-1.3.x / e0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd](https://openbenchmarking.org/test/pts/hashcat%26eval%3De0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd) |

**Aggregate rows in this card:** 22. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
