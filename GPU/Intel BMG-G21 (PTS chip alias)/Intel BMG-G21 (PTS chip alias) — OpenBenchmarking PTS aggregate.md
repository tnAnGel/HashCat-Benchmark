# Intel BMG-G21 (PTS chip alias) — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| ASUS Intel BMG G21 | 6.2.4 | 7-Zip | 292994 | 292.99 kH/s | 14th | 4 | 39013 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| ASUS Intel BMG G21 | 6.2.4 | MD5 | 27993025000 | 27.993 GH/s | 31st | 4 | 1524150000 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| Intel BMG G21 | 6.2.4 | MD5 | 23038650333 | 23.039 GH/s | 20th | 10 | 3177206249 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| ASUS Intel BMG G21 | 6.2.4 | SHA-512 | 464531250 | 464.53 MH/s | 11th | 4 | 23787500 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| ASUS Intel BMG G21 | 6.2.4 | SHA1 | 8837029167 | 8.837 GH/s | 26th | 4 | 668252778 | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| ASUS Intel BMG G21 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 425205 | 425.2 kH/s | 38th | 4 | 27710 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |
| ASUS Intel BMG G21 | 7.0 | 7-Zip | 284100 | 284.1 kH/s | 27th | 3 | 265 | [hashcat-1.2.x / 80b710251c56bf8e93ef06fbc970f443076e22e0](https://openbenchmarking.org/test/pts/hashcat%26eval%3D80b710251c56bf8e93ef06fbc970f443076e22e0) |
| ASUS Intel BMG G21 | 7.0 | Kerberos 5 + etype 23 + TGS-REP | 162929317 | 162.93 MH/s | 12th | 3 | 250553 | [hashcat-1.2.x / 6b1954debb13211e8b6d1b098290c5accf0e374f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6b1954debb13211e8b6d1b098290c5accf0e374f) |
| ASUS Intel BMG G21 | 7.0 | MD5 | 27104333333 | 27.104 GH/s | 32nd | 3 | 16500101 | [hashcat-1.2.x / 7b7b45c3848e0a5482fb82f220518d5233961430](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7b7b45c3848e0a5482fb82f220518d5233961430) |
| ASUS Intel BMG G21 | 7.0 | SHA-256 | 4692333333 | 4.6923 GH/s | 40th | 3 | 56840332 | [hashcat-1.2.x / 71ae6c8974b17ccdfcf3f872aab62d85c629e59e](https://openbenchmarking.org/test/pts/hashcat%26eval%3D71ae6c8974b17ccdfcf3f872aab62d85c629e59e) |
| ASUS Intel BMG G21 | 7.0 | SHA-512 | 717266667 | 717.27 MH/s | 28th | 3 | 38164949 | [hashcat-1.2.x / 32167b15bfd2349e12bfacbadc31e8396cd4f785](https://openbenchmarking.org/test/pts/hashcat%26eval%3D32167b15bfd2349e12bfacbadc31e8396cd4f785) |
| ASUS Intel BMG G21 | 7.0 | SHA1 | 14437433333 | 14.437 GH/s | 61st | 3 | 8422787 | [hashcat-1.2.x / 00d12c5cd061174be3e1233b616aaff5e3f9bd4f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D00d12c5cd061174be3e1233b616aaff5e3f9bd4f) |
| ASUS Intel BMG G21 | 7.0 | TrueCrypt RIPEMD160 + XTS | 432733 | 432.73 kH/s | 58th | 3 | 351 | [hashcat-1.2.x / 44bfe79903c83521447b7e56f6f948edf4dbc1cf](https://openbenchmarking.org/test/pts/hashcat%26eval%3D44bfe79903c83521447b7e56f6f948edf4dbc1cf) |
| ASUS Intel BMG G21 | 6.2.6 | Kerberos 5 + etype 23 + TGS-REP | 110499083 | 110.5 MH/s | 76th | 3 | 31988 | [system/hashcat-1.0.x / cd916f36b8c30ecb8bba03c995e8556340b601cc](https://openbenchmarking.org/performance/test/system/hashcat/cd916f36b8c30ecb8bba03c995e8556340b601cc) |
| ASUS Intel BMG G21 | 6.2.6 | LastPass | 3482267 | 3.4823 MH/s | 73rd | 3 | 1692 | [system/hashcat-1.0.x / 36e98a1da0aec289b751c5459a2ae700943a442f](https://openbenchmarking.org/performance/test/system/hashcat/36e98a1da0aec289b751c5459a2ae700943a442f) |
| ASUS Intel BMG G21 | 6.2.6 | SHA-256 | 6042766667 | 6.0428 GH/s | 76th | 3 | 67869753 | [system/hashcat-1.0.x / b6311a7833fd22620b186e0667dd2600d1980264](https://openbenchmarking.org/performance/test/system/hashcat/b6311a7833fd22620b186e0667dd2600d1980264) |
| ASUS Intel BMG G21 | 6.2.6 | SHA-512 | 728500000 | 728.5 MH/s | 76th | 3 | 793725 | [system/hashcat-1.0.x / b882cb3d8fda94c160446db96187fe1e1fa2496f](https://openbenchmarking.org/performance/test/system/hashcat/b882cb3d8fda94c160446db96187fe1e1fa2496f) |
| ASUS Intel BMG G21 | 6.2.6 | SHA1 | 14648266667 | 14.648 GH/s | 76th | 3 | 2956913 | [system/hashcat-1.0.x / 7836cc88bb368389170458a6b54b3c1fc53304de](https://openbenchmarking.org/performance/test/system/hashcat/7836cc88bb368389170458a6b54b3c1fc53304de) |

**Aggregate rows in this card:** 18. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
