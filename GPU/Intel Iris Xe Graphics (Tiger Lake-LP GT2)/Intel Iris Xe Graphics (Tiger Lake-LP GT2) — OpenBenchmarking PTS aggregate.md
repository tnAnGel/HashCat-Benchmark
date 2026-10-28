# Intel Iris Xe Graphics (Tiger Lake-LP GT2) — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| Intel Iris Xe TGL GT2 | 7.1.2 | 7-Zip | 34647 | 34.647 kH/s | 2nd | 4 | 350 | [hashcat-1.3.x / dd3830ac8f396d5aeb2c788ccf63196ccfe6b785](https://openbenchmarking.org/test/pts/hashcat%26eval%3Ddd3830ac8f396d5aeb2c788ccf63196ccfe6b785) |
| Intel Iris Xe TGL GT2 | 7.1.2 | Kerberos 5 + etype 23 + TGS-REP | 35820827 | 35.821 MH/s | 3rd | 4 | 56305 | [hashcat-1.3.x / 89adea9de254c520e2999634807af2397c2da2c3](https://openbenchmarking.org/test/pts/hashcat%26eval%3D89adea9de254c520e2999634807af2397c2da2c3) |
| Intel Iris Xe TGL GT2 | 7.1.2 | LastPass | 1728 | 1.728 kH/s | 4th | 4 | 42 | [hashcat-1.3.x / 82bc713652e59980e398283abaaf76352af9bb0c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D82bc713652e59980e398283abaaf76352af9bb0c) |
| Intel Iris Xe TGL GT2 | 7.1.2 | MD5 | 3044741667 | 3.0447 GH/s | 4th | 4 | 1629673 | [hashcat-1.3.x / 2f1e49c858bdaf551168a2c36422c3bcd6dbf083](https://openbenchmarking.org/test/pts/hashcat%26eval%3D2f1e49c858bdaf551168a2c36422c3bcd6dbf083) |
| Intel Iris Xe TGL GT2 | 7.1.2 | NTLM | 5102554167 | 5.1026 GH/s | 4th | 4 | 3452867 | [hashcat-1.3.x / a21d6e2b0f86d6fd008776a0dbcd84258d25b266](https://openbenchmarking.org/test/pts/hashcat%26eval%3Da21d6e2b0f86d6fd008776a0dbcd84258d25b266) |
| Intel Iris Xe TGL GT2 | 7.1.2 | SHA-256 | 542285000 | 542.28 MH/s | 4th | 4 | 513128 | [hashcat-1.3.x / bb70ab4002871eaf41c4c257184d478de05cb604](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dbb70ab4002871eaf41c4c257184d478de05cb604) |
| Intel Iris Xe TGL GT2 | 7.1.2 | SHA-512 | 98354330 | 98.354 MH/s | 5th | 4 | 3817149 | [hashcat-1.3.x / ec680f525d7a44fb1c765bf8f3508874a039743e](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dec680f525d7a44fb1c765bf8f3508874a039743e) |
| Intel Iris Xe TGL GT2 | 7.1.2 | SHA1 | 1217815000 | 1.2178 GH/s | 4th | 4 | 13963069 | [hashcat-1.3.x / eff31b43dba5f679500a7b4a9d777e74ae74d575](https://openbenchmarking.org/test/pts/hashcat%26eval%3Deff31b43dba5f679500a7b4a9d777e74ae74d575) |
| Intel Iris Xe TGL GT2 | 7.1.2 | TrueCrypt RIPEMD160 + XTS | 31378 | 31.378 kH/s | 4th | 4 | 290 | [hashcat-1.3.x / 152ac6b8c7471c32a080a40569d381f6f87925f7](https://openbenchmarking.org/test/pts/hashcat%26eval%3D152ac6b8c7471c32a080a40569d381f6f87925f7) |
| Intel Iris Xe TGL GT2 | 7.1.2 | WPA-PBKDF2-PMKID+EAPOL | 59955 | 59.955 kH/s | 4th | 4 | 3005 | [hashcat-1.3.x / 6ec0566c352e7ce9cee334cd480808fd993aa913](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6ec0566c352e7ce9cee334cd480808fd993aa913) |
| Intel Iris Xe TGL GT2 | 7.1.2 | bcrypt | 2773 | 2.773 kH/s | 5th | 4 | 1 | [hashcat-1.3.x / e0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd](https://openbenchmarking.org/test/pts/hashcat%26eval%3De0c0e260fcfd3a3b16a774e5a8a1993364e8f2bd) |
| Intel Iris Xe TGL GT2 | 6.2.6 | Kerberos 5 + etype 23 + TGS-REP | 15259178 | 15.259 MH/s | 23rd | 7 | 417896 | [system/hashcat-1.0.x / cd916f36b8c30ecb8bba03c995e8556340b601cc](https://openbenchmarking.org/performance/test/system/hashcat/cd916f36b8c30ecb8bba03c995e8556340b601cc) |
| Intel Iris Xe TGL GT2 | 6.2.6 | LastPass | 359823 | 359.82 kH/s | 23rd | 7 | 9086 | [system/hashcat-1.0.x / 36e98a1da0aec289b751c5459a2ae700943a442f](https://openbenchmarking.org/performance/test/system/hashcat/36e98a1da0aec289b751c5459a2ae700943a442f) |
| Intel Iris Xe TGL GT2 | 6.2.6 | SHA-256 | 250485714 | 250.49 MH/s | 16th | 7 | 13663629 | [system/hashcat-1.0.x / b6311a7833fd22620b186e0667dd2600d1980264](https://openbenchmarking.org/performance/test/system/hashcat/b6311a7833fd22620b186e0667dd2600d1980264) |
| Intel Iris Xe TGL GT2 | 6.2.6 | SHA-512 | 92403829 | 92.404 MH/s | 33rd | 7 | 3611522 | [system/hashcat-1.0.x / b882cb3d8fda94c160446db96187fe1e1fa2496f](https://openbenchmarking.org/performance/test/system/hashcat/b882cb3d8fda94c160446db96187fe1e1fa2496f) |
| Intel Iris Xe TGL GT2 | 6.2.6 | SHA1 | 1112952381 | 1.113 GH/s | 23rd | 7 | 53699227 | [system/hashcat-1.0.x / 7836cc88bb368389170458a6b54b3c1fc53304de](https://openbenchmarking.org/performance/test/system/hashcat/7836cc88bb368389170458a6b54b3c1fc53304de) |

**Aggregate rows in this card:** 16. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
