# Intel Iris Xe Graphics (Alder Lake GT2) — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| MSI Intel Iris Xe ADL GT2 | 7.1.2 | 7-Zip | 55083 | 55.083 kH/s | 7th | 3 | 6850 | [hashcat-1.3.x / dd3830ac8f396d5aeb2c788ccf63196ccfe6b785](https://openbenchmarking.org/test/pts/hashcat%26eval%3Ddd3830ac8f396d5aeb2c788ccf63196ccfe6b785) |
| MSI Intel Iris Xe ADL GT2 | 7.1.2 | Kerberos 5 + etype 23 + TGS-REP | 38570689 | 38.571 MH/s | 5th | 3 | 141759 | [hashcat-1.3.x / 89adea9de254c520e2999634807af2397c2da2c3](https://openbenchmarking.org/test/pts/hashcat%26eval%3D89adea9de254c520e2999634807af2397c2da2c3) |
| MSI Intel Iris Xe ADL GT2 | 7.1.2 | LastPass | 1815 | 1.815 kH/s | 5th | 3 | 251 | [hashcat-1.3.x / 82bc713652e59980e398283abaaf76352af9bb0c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D82bc713652e59980e398283abaaf76352af9bb0c) |
| MSI Intel Iris Xe ADL GT2 | 7.1.2 | MD5 | 2851766667 | 2.8518 GH/s | 4th | 3 | 392598183 | [hashcat-1.3.x / 2f1e49c858bdaf551168a2c36422c3bcd6dbf083](https://openbenchmarking.org/test/pts/hashcat%26eval%3D2f1e49c858bdaf551168a2c36422c3bcd6dbf083) |
| MSI Intel Iris Xe ADL GT2 | 7.1.2 | NTLM | 5048697778 | 5.0487 GH/s | 3rd | 3 | 449382506 | [hashcat-1.3.x / a21d6e2b0f86d6fd008776a0dbcd84258d25b266](https://openbenchmarking.org/test/pts/hashcat%26eval%3Da21d6e2b0f86d6fd008776a0dbcd84258d25b266) |
| MSI Intel Iris Xe ADL GT2 | 7.1.2 | SHA-256 | 500688889 | 500.69 MH/s | 4th | 3 | 60371593 | [hashcat-1.3.x / bb70ab4002871eaf41c4c257184d478de05cb604](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dbb70ab4002871eaf41c4c257184d478de05cb604) |
| MSI Intel Iris Xe ADL GT2 | 7.1.2 | SHA-512 | 93879258 | 93.879 MH/s | 3rd | 3 | 6080141 | [hashcat-1.3.x / ec680f525d7a44fb1c765bf8f3508874a039743e](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dec680f525d7a44fb1c765bf8f3508874a039743e) |
| MSI Intel Iris Xe ADL GT2 | 7.1.2 | SHA1 | 1123591111 | 1.1236 GH/s | 3rd | 3 | 165418550 | [hashcat-1.3.x / eff31b43dba5f679500a7b4a9d777e74ae74d575](https://openbenchmarking.org/test/pts/hashcat%26eval%3Deff31b43dba5f679500a7b4a9d777e74ae74d575) |
| MSI Intel Iris Xe ADL GT2 | 7.1.2 | WPA-PBKDF2-PMKID+EAPOL | 59486 | 59.486 kH/s | 4th | 3 | 7511 | [hashcat-1.3.x / 6ec0566c352e7ce9cee334cd480808fd993aa913](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6ec0566c352e7ce9cee334cd480808fd993aa913) |
| MSI Intel Iris Xe ADL GT2 | 7.1.2 | bcrypt | 2993 | 2.993 kH/s | 6th | 3 | 1 | [hashcat-1.3.x / e0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd](https://openbenchmarking.org/test/pts/hashcat%26eval%3De0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd) |
| MSI Intel Iris Xe ADL GT2 | 6.2.6 | Kerberos 5 + etype 23 + TGS-REP | 17223633 | 17.224 MH/s | 39th | 3 | 4924 | [system/hashcat-1.0.x / cd916f36b8c30ecb8bba03c995e8556340b601cc](https://openbenchmarking.org/performance/test/system/hashcat/cd916f36b8c30ecb8bba03c995e8556340b601cc) |
| MSI Intel Iris Xe ADL GT2 | 6.2.6 | LastPass | 425500 | 425.5 kH/s | 39th | 3 | 4431 | [system/hashcat-1.0.x / 36e98a1da0aec289b751c5459a2ae700943a442f](https://openbenchmarking.org/performance/test/system/hashcat/36e98a1da0aec289b751c5459a2ae700943a442f) |
| MSI Intel Iris Xe ADL GT2 | 6.2.6 | SHA-256 | 286766667 | 286.77 MH/s | 36th | 3 | 1616581 | [system/hashcat-1.0.x / b6311a7833fd22620b186e0667dd2600d1980264](https://openbenchmarking.org/performance/test/system/hashcat/b6311a7833fd22620b186e0667dd2600d1980264) |
| MSI Intel Iris Xe ADL GT2 | 6.2.6 | SHA-512 | 108600000 | 108.6 MH/s | 55th | 3 | 360555 | [system/hashcat-1.0.x / b882cb3d8fda94c160446db96187fe1e1fa2496f](https://openbenchmarking.org/performance/test/system/hashcat/b882cb3d8fda94c160446db96187fe1e1fa2496f) |
| MSI Intel Iris Xe ADL GT2 | 6.2.6 | SHA1 | 1304733333 | 1.3047 GH/s | 39th | 3 | 28478823 | [system/hashcat-1.0.x / 7836cc88bb368389170458a6b54b3c1fc53304de](https://openbenchmarking.org/performance/test/system/hashcat/7836cc88bb368389170458a6b54b3c1fc53304de) |

**Aggregate rows in this card:** 15. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
