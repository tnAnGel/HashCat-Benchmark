# NVIDIA RTX PRO 6000 Blackwell Max-Q Workstation Edition — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| NVIDIA RTX PRO 6000 Blackwell Max-Q Workstation Edition | 7.1.2 | 7-Zip | 2879175 | 2.8792 MH/s | 95th | 7 | 143969 | [hashcat-1.3.x / dd3830ac8f396d5aeb2c788ccf63196ccfe6b785](https://openbenchmarking.org/test/pts/hashcat%26eval%3Ddd3830ac8f396d5aeb2c788ccf63196ccfe6b785) |
| NVIDIA RTX PRO 6000 Blackwell Max-Q Workstation Edition | 7.1.2 | Kerberos 5 + etype 23 + TGS-REP | 3875569047 | 3.8756 GH/s | 95th | 7 | 157571966 | [hashcat-1.3.x / 89adea9de254c520e2999634807af2397c2da2c3](https://openbenchmarking.org/test/pts/hashcat%26eval%3D89adea9de254c520e2999634807af2397c2da2c3) |
| NVIDIA RTX PRO 6000 Blackwell Max-Q Workstation Edition | 7.1.2 | LUKS v2 argon2id + SHA-256 + AES | 71 | 71 H/s | 97th | 7 | 1 | [hashcat-1.3.x / 0b5d0c3db0c27a2a6e025024f7e154886882d515](https://openbenchmarking.org/test/pts/hashcat%26eval%3D0b5d0c3db0c27a2a6e025024f7e154886882d515) |
| NVIDIA RTX PRO 6000 Blackwell Max-Q Workstation Edition | 7.1.2 | LastPass | 97842 | 97.842 kH/s | 94th | 7 | 1859 | [hashcat-1.3.x / 82bc713652e59980e398283abaaf76352af9bb0c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D82bc713652e59980e398283abaaf76352af9bb0c) |
| NVIDIA RTX PRO 6000 Blackwell Max-Q Workstation Edition | 7.1.2 | MD5 | 177915000000 | 177.91 GH/s | 97th | 4 | 2850841981 | [hashcat-1.3.x / 2f1e49c858bdaf551168a2c36422c3bcd6dbf083](https://openbenchmarking.org/test/pts/hashcat%26eval%3D2f1e49c858bdaf551168a2c36422c3bcd6dbf083) |
| NVIDIA RTX PRO 6000 Blackwell Max-Q Workstation Edition | 7.1.2 | NTLM | 290809523809 | 290.81 GH/s | 95th | 7 | 9103061436 | [hashcat-1.3.x / a21d6e2b0f86d6fd008776a0dbcd84258d25b266](https://openbenchmarking.org/test/pts/hashcat%26eval%3Da21d6e2b0f86d6fd008776a0dbcd84258d25b266) |
| NVIDIA RTX PRO 6000 Blackwell Max-Q Workstation Edition | 7.1.2 | SHA-256 | 23566580476 | 23.567 GH/s | 95th | 7 | 406242002 | [hashcat-1.3.x / bb70ab4002871eaf41c4c257184d478de05cb604](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dbb70ab4002871eaf41c4c257184d478de05cb604) |
| NVIDIA RTX PRO 6000 Blackwell Max-Q Workstation Edition | 7.1.2 | SHA-512 | 7588090952 | 7.5881 GH/s | 94th | 7 | 40234472 | [hashcat-1.3.x / ec680f525d7a44fb1c765bf8f3508874a039743e](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dec680f525d7a44fb1c765bf8f3508874a039743e) |
| NVIDIA RTX PRO 6000 Blackwell Max-Q Workstation Edition | 7.1.2 | SHA1 | 60273848095 | 60.274 GH/s | 94th | 7 | 2427029762 | [hashcat-1.3.x / eff31b43dba5f679500a7b4a9d777e74ae74d575](https://openbenchmarking.org/test/pts/hashcat%26eval%3Deff31b43dba5f679500a7b4a9d777e74ae74d575) |
| NVIDIA RTX PRO 6000 Blackwell Max-Q Workstation Edition | 7.1.2 | TrueCrypt RIPEMD160 + XTS | 2265359 | 2.2654 MH/s | 96th | 7 | 50903 | [hashcat-1.3.x / 152ac6b8c7471c32a080a40569d381f6f87925f7](https://openbenchmarking.org/test/pts/hashcat%26eval%3D152ac6b8c7471c32a080a40569d381f6f87925f7) |
| NVIDIA RTX PRO 6000 Blackwell Max-Q Workstation Edition | 7.1.2 | WPA-PBKDF2-PMKID+EAPOL | 2948636 | 2.9486 MH/s | 94th | 7 | 106949 | [hashcat-1.3.x / 6ec0566c352e7ce9cee334cd480808fd993aa913](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6ec0566c352e7ce9cee334cd480808fd993aa913) |
| NVIDIA RTX PRO 6000 Blackwell Max-Q Workstation Edition | 7.1.2 | bcrypt | 259993 | 259.99 kH/s | 91st | 7 | 3807 | [hashcat-1.3.x / e0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd](https://openbenchmarking.org/test/pts/hashcat%26eval%3De0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd) |

**Aggregate rows in this card:** 12. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
