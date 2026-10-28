# NVIDIA GeForce RTX 5080 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| ASUS NVIDIA GeForce RTX 5080 | 6.2.4 | 7-Zip | 1652656 | 1.6527 MH/s | 83rd | 6 | 12981 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| ASUS NVIDIA GeForce RTX 5080 | 6.2.4 | MD5 | 99625400000 | 99.625 GH/s | 89th | 4 | 219854983 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| NVIDIA GeForce RTX 5080 | 6.2.4 | SHA-512 | 4278811111 | 4.2788 GH/s | 87th | 3 | 68281291 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| ASUS NVIDIA GeForce RTX 5080 | 6.2.4 | SHA-512 | 4110183333 | 4.1102 GH/s | 87th | 6 | 223413833 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| ASUS NVIDIA GeForce RTX 5080 | 6.2.4 | SHA1 | 32188780000 | 32.189 GH/s | 85th | 6 | 604693490 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| ASUS NVIDIA GeForce RTX 5080 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 1282622 | 1.2826 MH/s | 86th | 6 | 18325 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |
| Gigabyte NVIDIA GeForce RTX 5080 | 7.1.2 | 7-Zip | 1687600 | 1.6876 MH/s | 81st | 3 | 346 | [hashcat-1.3.x / dd3830ac8f396d5aeb2c788ccf63196ccfe6b785](https://openbenchmarking.org/test/pts/hashcat%26eval%3Ddd3830ac8f396d5aeb2c788ccf63196ccfe6b785) |
| Gigabyte NVIDIA GeForce RTX 5080 | 7.1.2 | Kerberos 5 + etype 23 + TGS-REP | 2087833333 | 2.0878 GH/s | 79th | 3 | 288675 | [hashcat-1.3.x / 89adea9de254c520e2999634807af2397c2da2c3](https://openbenchmarking.org/test/pts/hashcat%26eval%3D89adea9de254c520e2999634807af2397c2da2c3) |
| Gigabyte NVIDIA GeForce RTX 5080 | 7.1.2 | LUKS v2 argon2id + SHA-256 + AES | 13 | 13 H/s | 62nd | 3 | — | [hashcat-1.3.x / 0b5d0c3db0c27a2a6e025024f7e154886882d515](https://openbenchmarking.org/test/pts/hashcat%26eval%3D0b5d0c3db0c27a2a6e025024f7e154886882d515) |
| Gigabyte NVIDIA GeForce RTX 5080 | 7.1.2 | LastPass | 55235 | 55.235 kH/s | 83rd | 3 | 5 | [hashcat-1.3.x / 82bc713652e59980e398283abaaf76352af9bb0c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D82bc713652e59980e398283abaaf76352af9bb0c) |
| Gigabyte NVIDIA GeForce RTX 5080 | 7.1.2 | MD5 | 105300000000 | 105.3 GH/s | 92nd | 3 | — | [hashcat-1.3.x / 2f1e49c858bdaf551168a2c36422c3bcd6dbf083](https://openbenchmarking.org/test/pts/hashcat%26eval%3D2f1e49c858bdaf551168a2c36422c3bcd6dbf083) |
| Gigabyte NVIDIA GeForce RTX 5080 | 7.1.2 | NTLM | 176060000000 | 176.06 GH/s | 83rd | 5 | 18299414077 | [hashcat-1.3.x / a21d6e2b0f86d6fd008776a0dbcd84258d25b266](https://openbenchmarking.org/test/pts/hashcat%26eval%3Da21d6e2b0f86d6fd008776a0dbcd84258d25b266) |
| Gigabyte NVIDIA GeForce RTX 5080 | 7.1.2 | SHA-256 | 13443700000 | 13.444 GH/s | 83rd | 3 | 1039230 | [hashcat-1.3.x / bb70ab4002871eaf41c4c257184d478de05cb604](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dbb70ab4002871eaf41c4c257184d478de05cb604) |
| Gigabyte NVIDIA GeForce RTX 5080 | 7.1.2 | SHA-512 | 4869580000 | 4.8696 GH/s | 84th | 5 | 96014240 | [hashcat-1.3.x / ec680f525d7a44fb1c765bf8f3508874a039743e](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dec680f525d7a44fb1c765bf8f3508874a039743e) |
| Gigabyte NVIDIA GeForce RTX 5080 | 7.1.2 | SHA1 | 32374833333 | 32.375 GH/s | 77th | 3 | 5600298 | [hashcat-1.3.x / eff31b43dba5f679500a7b4a9d777e74ae74d575](https://openbenchmarking.org/test/pts/hashcat%26eval%3Deff31b43dba5f679500a7b4a9d777e74ae74d575) |
| Gigabyte NVIDIA GeForce RTX 5080 | 7.1.2 | TrueCrypt RIPEMD160 + XTS | 1345733 | 1.3457 MH/s | 82nd | 3 | 58 | [hashcat-1.3.x / 152ac6b8c7471c32a080a40569d381f6f87925f7](https://openbenchmarking.org/test/pts/hashcat%26eval%3D152ac6b8c7471c32a080a40569d381f6f87925f7) |
| Gigabyte NVIDIA GeForce RTX 5080 | 7.1.2 | WPA-PBKDF2-PMKID+EAPOL | 1625100 | 1.6251 MH/s | 82nd | 3 | — | [hashcat-1.3.x / 6ec0566c352e7ce9cee334cd480808fd993aa913](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6ec0566c352e7ce9cee334cd480808fd993aa913) |
| Gigabyte NVIDIA GeForce RTX 5080 | 7.1.2 | bcrypt | 140100 | 140.1 kH/s | 85th | 3 | — | [hashcat-1.3.x / e0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd](https://openbenchmarking.org/test/pts/hashcat%26eval%3De0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd) |

**Aggregate rows in this card:** 18. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
