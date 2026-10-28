# NVIDIA GeForce RTX 5060 Ti — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| NVIDIA GeForce RTX 5060 Ti | 7.1.2 | 7-Zip | 783944 | 783.94 kH/s | 54th | 3 | 8294 | [hashcat-1.3.x / dd3830ac8f396d5aeb2c788ccf63196ccfe6b785](https://openbenchmarking.org/test/pts/hashcat%26eval%3Ddd3830ac8f396d5aeb2c788ccf63196ccfe6b785) |
| NVIDIA GeForce RTX 5060 Ti | 7.1.2 | Kerberos 5 + etype 23 + TGS-REP | 926444444 | 926.44 MH/s | 56th | 3 | 846780 | [hashcat-1.3.x / 89adea9de254c520e2999634807af2397c2da2c3](https://openbenchmarking.org/test/pts/hashcat%26eval%3D89adea9de254c520e2999634807af2397c2da2c3) |
| NVIDIA GeForce RTX 5060 Ti | 7.1.2 | LUKS v2 argon2id + SHA-256 + AES | 13 | 13 H/s | 62nd | 3 | 1 | [hashcat-1.3.x / 0b5d0c3db0c27a2a6e025024f7e154886882d515](https://openbenchmarking.org/test/pts/hashcat%26eval%3D0b5d0c3db0c27a2a6e025024f7e154886882d515) |
| NVIDIA GeForce RTX 5060 Ti | 7.1.2 | LastPass | 26810 | 26.81 kH/s | 49th | 3 | 42 | [hashcat-1.3.x / 82bc713652e59980e398283abaaf76352af9bb0c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D82bc713652e59980e398283abaaf76352af9bb0c) |
| NVIDIA GeForce RTX 5060 Ti | 7.1.2 | MD5 | 49875833333 | 49.876 GH/s | 71st | 3 | 65991136 | [hashcat-1.3.x / 2f1e49c858bdaf551168a2c36422c3bcd6dbf083](https://openbenchmarking.org/test/pts/hashcat%26eval%3D2f1e49c858bdaf551168a2c36422c3bcd6dbf083) |
| NVIDIA GeForce RTX 5060 Ti | 7.1.2 | NTLM | 86700314286 | 86.7 GH/s | 63rd | 3 | 100384716 | [hashcat-1.3.x / a21d6e2b0f86d6fd008776a0dbcd84258d25b266](https://openbenchmarking.org/test/pts/hashcat%26eval%3Da21d6e2b0f86d6fd008776a0dbcd84258d25b266) |
| NVIDIA GeForce RTX 5060 Ti | 7.1.2 | SHA-256 | 6470911111 | 6.4709 GH/s | 44th | 3 | 11643230 | [hashcat-1.3.x / bb70ab4002871eaf41c4c257184d478de05cb604](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dbb70ab4002871eaf41c4c257184d478de05cb604) |
| NVIDIA GeForce RTX 5060 Ti | 7.1.2 | SHA-512 | 2136555556 | 2.1366 GH/s | 54th | 3 | 3569950 | [hashcat-1.3.x / ec680f525d7a44fb1c765bf8f3508874a039743e](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dec680f525d7a44fb1c765bf8f3508874a039743e) |
| NVIDIA GeForce RTX 5060 Ti | 7.1.2 | SHA1 | 16983744444 | 16.984 GH/s | 48th | 3 | 27087350 | [hashcat-1.3.x / eff31b43dba5f679500a7b4a9d777e74ae74d575](https://openbenchmarking.org/test/pts/hashcat%26eval%3Deff31b43dba5f679500a7b4a9d777e74ae74d575) |
| NVIDIA GeForce RTX 5060 Ti | 7.1.2 | TrueCrypt RIPEMD160 + XTS | 648889 | 648.89 kH/s | 60th | 3 | 1029 | [hashcat-1.3.x / 152ac6b8c7471c32a080a40569d381f6f87925f7](https://openbenchmarking.org/test/pts/hashcat%26eval%3D152ac6b8c7471c32a080a40569d381f6f87925f7) |
| NVIDIA GeForce RTX 5060 Ti | 7.1.2 | WPA-PBKDF2-PMKID+EAPOL | 864056 | 864.06 kH/s | 56th | 3 | 1492 | [hashcat-1.3.x / 6ec0566c352e7ce9cee334cd480808fd993aa913](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6ec0566c352e7ce9cee334cd480808fd993aa913) |
| NVIDIA GeForce RTX 5060 Ti | 7.1.2 | bcrypt | 59965 | 59.965 kH/s | 57th | 3 | 70 | [hashcat-1.3.x / e0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd](https://openbenchmarking.org/test/pts/hashcat%26eval%3De0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd) |

**Aggregate rows in this card:** 12. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
