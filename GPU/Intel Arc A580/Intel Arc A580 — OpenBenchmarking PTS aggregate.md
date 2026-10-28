# Intel Arc A580 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| Intel Arc A580 DG2 | 6.2.4 | 7-Zip | 248140 | 248.14 kH/s | 12th | 8 | 646 | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| Intel Arc A580 DG2 | 6.2.4 | MD5 | 26264094872 | 26.264 GH/s | 29th | 13 | 102468815 | [hashcat-1.1.x / 8b64c180eac0ce4c97f0d73d774dbb6161bedb5f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D8b64c180eac0ce4c97f0d73d774dbb6161bedb5f) |
| Intel Arc A580 DG2 | 6.2.4 | SHA-512 | 793383333 | 793.38 MH/s | 19th | 14 | 6894160 | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| Intel Arc A580 DG2 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 275907 | 275.91 kH/s | 13th | 14 | 5505 | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |
| ASUS Intel Arc A580 DG2 | 7.0 | 7-Zip | 292542 | 292.54 kH/s | 30th | 4 | 1037 | [hashcat-1.2.x / 80b710251c56bf8e93ef06fbc970f443076e22e0](https://openbenchmarking.org/test/pts/hashcat%26eval%3D80b710251c56bf8e93ef06fbc970f443076e22e0) |
| Intel Arc A580 DG2 | 7.0 | Kerberos 5 + etype 23 + TGS-REP | 297234921 | 297.23 MH/s | 37th | 3 | 551232 | [hashcat-1.2.x / 6b1954debb13211e8b6d1b098290c5accf0e374f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6b1954debb13211e8b6d1b098290c5accf0e374f) |
| ASUS Intel Arc A580 DG2 | 7.0 | Kerberos 5 + etype 23 + TGS-REP | 184406653 | 184.41 MH/s | 18th | 4 | 289888 | [hashcat-1.2.x / 6b1954debb13211e8b6d1b098290c5accf0e374f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D6b1954debb13211e8b6d1b098290c5accf0e374f) |
| ASUS Intel Arc A580 DG2 | 7.0 | MD5 | 30938091667 | 30.938 GH/s | 48th | 4 | 27883453 | [hashcat-1.2.x / 7b7b45c3848e0a5482fb82f220518d5233961430](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7b7b45c3848e0a5482fb82f220518d5233961430) |
| ASUS Intel Arc A580 DG2 | 7.0 | SHA-256 | 6158866667 | 6.1589 GH/s | 60th | 4 | 15055674 | [hashcat-1.2.x / 71ae6c8974b17ccdfcf3f872aab62d85c629e59e](https://openbenchmarking.org/test/pts/hashcat%26eval%3D71ae6c8974b17ccdfcf3f872aab62d85c629e59e) |
| Intel Arc A580 DG2 | 7.0 | SHA-256 | 5331806667 | 5.3318 GH/s | 46th | 3 | 7147596 | [hashcat-1.2.x / 71ae6c8974b17ccdfcf3f872aab62d85c629e59e](https://openbenchmarking.org/test/pts/hashcat%26eval%3D71ae6c8974b17ccdfcf3f872aab62d85c629e59e) |
| ASUS Intel Arc A580 DG2 | 7.0 | SHA-512 | 1023158333 | 1.0232 GH/s | 39th | 4 | 1158663 | [hashcat-1.2.x / 32167b15bfd2349e12bfacbadc31e8396cd4f785](https://openbenchmarking.org/test/pts/hashcat%26eval%3D32167b15bfd2349e12bfacbadc31e8396cd4f785) |
| Intel Arc A580 DG2 | 7.0 | SHA-512 | 882433333 | 882.43 MH/s | 33rd | 3 | 6596227 | [hashcat-1.2.x / 32167b15bfd2349e12bfacbadc31e8396cd4f785](https://openbenchmarking.org/test/pts/hashcat%26eval%3D32167b15bfd2349e12bfacbadc31e8396cd4f785) |
| ASUS Intel Arc A580 DG2 | 7.0 | SHA1 | 13774108334 | 13.774 GH/s | 52nd | 4 | 33281653 | [hashcat-1.2.x / 00d12c5cd061174be3e1233b616aaff5e3f9bd4f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D00d12c5cd061174be3e1233b616aaff5e3f9bd4f) |
| Intel Arc A580 DG2 | 7.0 | SHA1 | 11780322222 | 11.78 GH/s | 31st | 3 | 9651372 | [hashcat-1.2.x / 00d12c5cd061174be3e1233b616aaff5e3f9bd4f](https://openbenchmarking.org/test/pts/hashcat%26eval%3D00d12c5cd061174be3e1233b616aaff5e3f9bd4f) |
| ASUS Intel Arc A580 DG2 | 7.0 | TrueCrypt RIPEMD160 + XTS | 326975 | 326.98 kH/s | 31st | 4 | 507 | [hashcat-1.2.x / 44bfe79903c83521447b7e56f6f948edf4dbc1cf](https://openbenchmarking.org/test/pts/hashcat%26eval%3D44bfe79903c83521447b7e56f6f948edf4dbc1cf) |
| Intel Arc A580 DG2 | 7.0 | TrueCrypt RIPEMD160 + XTS | 277147 | 277.15 kH/s | 22nd | 3 | 115 | [hashcat-1.2.x / 44bfe79903c83521447b7e56f6f948edf4dbc1cf](https://openbenchmarking.org/test/pts/hashcat%26eval%3D44bfe79903c83521447b7e56f6f948edf4dbc1cf) |

**Aggregate rows in this card:** 16. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
