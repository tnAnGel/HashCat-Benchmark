# NVIDIA RTX PRO 5000 Blackwell — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| NVIDIA RTX PRO 5000 Blackwell | 7.1.2 | 7-Zip | 2249078 | 2.2491 MH/s | 92nd | 6 | 13470 | [hashcat-1.3.x / dd3830ac8f396d5aeb2c788ccf63196ccfe6b785](https://openbenchmarking.org/test/pts/hashcat%26eval%3Ddd3830ac8f396d5aeb2c788ccf63196ccfe6b785) |
| NVIDIA RTX PRO 5000 Blackwell | 7.1.2 | Kerberos 5 + etype 23 + TGS-REP | 2743480952 | 2.7435 GH/s | 86th | 6 | 627054 | [hashcat-1.3.x / 89adea9de254c520e2999634807af2397c2da2c3](https://openbenchmarking.org/test/pts/hashcat%26eval%3D89adea9de254c520e2999634807af2397c2da2c3) |
| NVIDIA RTX PRO 5000 Blackwell | 7.1.2 | LastPass | 72267 | 72.267 kH/s | 87th | 6 | 2 | [hashcat-1.3.x / 82bc713652e59980e398283abaaf76352af9bb0c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D82bc713652e59980e398283abaaf76352af9bb0c) |
| NVIDIA RTX PRO 5000 Blackwell | 7.1.2 | NTLM | 219733333333 | 219.73 GH/s | 90th | 6 | 77459667 | [hashcat-1.3.x / a21d6e2b0f86d6fd008776a0dbcd84258d25b266](https://openbenchmarking.org/test/pts/hashcat%26eval%3Da21d6e2b0f86d6fd008776a0dbcd84258d25b266) |
| NVIDIA RTX PRO 5000 Blackwell | 7.1.2 | SHA-256 | 16719627778 | 16.72 GH/s | 86th | 6 | 7263996 | [hashcat-1.3.x / bb70ab4002871eaf41c4c257184d478de05cb604](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dbb70ab4002871eaf41c4c257184d478de05cb604) |
| NVIDIA RTX PRO 5000 Blackwell | 7.1.2 | SHA-512 | 5748442222 | 5.7484 GH/s | 87th | 6 | 4583891 | [hashcat-1.3.x / ec680f525d7a44fb1c765bf8f3508874a039743e](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dec680f525d7a44fb1c765bf8f3508874a039743e) |
| NVIDIA RTX PRO 5000 Blackwell | 7.1.2 | SHA1 | 46256888889 | 46.257 GH/s | 91st | 6 | 8090232 | [hashcat-1.3.x / eff31b43dba5f679500a7b4a9d777e74ae74d575](https://openbenchmarking.org/test/pts/hashcat%26eval%3Deff31b43dba5f679500a7b4a9d777e74ae74d575) |
| NVIDIA RTX PRO 5000 Blackwell | 7.1.2 | TrueCrypt RIPEMD160 + XTS | 1668960 | 1.669 MH/s | 91st | 6 | 248 | [hashcat-1.3.x / 152ac6b8c7471c32a080a40569d381f6f87925f7](https://openbenchmarking.org/test/pts/hashcat%26eval%3D152ac6b8c7471c32a080a40569d381f6f87925f7) |
| NVIDIA RTX PRO 5000 Blackwell | 7.1.2 | WPA-PBKDF2-PMKID+EAPOL | 2250745 | 2.2507 MH/s | 91st | 6 | 2134 | [hashcat-1.3.x / 6ec0566c352e7ce9cee334cd480808fd993aa913](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6ec0566c352e7ce9cee334cd480808fd993aa913) |
| NVIDIA RTX PRO 5000 Blackwell | 7.1.2 | bcrypt | 166539 | 166.54 kH/s | 86th | 6 | 43 | [hashcat-1.3.x / e0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd](https://openbenchmarking.org/test/pts/hashcat%26eval%3De0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd) |

**Aggregate rows in this card:** 10. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
