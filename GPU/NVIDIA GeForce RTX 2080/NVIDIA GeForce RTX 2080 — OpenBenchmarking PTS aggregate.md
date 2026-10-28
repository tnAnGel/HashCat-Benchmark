# NVIDIA GeForce RTX 2080 — OpenBenchmarking Hashcat profile data (aggregate)

- **Evidence type:** PTS profile-level community aggregate; not one machine, not a per-card raw run, and not Hashcat stdout.
- **Meaning:** mean speed across the number of compatible public result uploads shown in the table. Percentile is the profile ranking; standard deviation is included when published.
- **Use:** supplementary comparison only. Do not merge these values with raw `Speed.#N` readings or treat `result_count` as number of GPUs in a rig.

| PTS device label | Hashcat | Metric | Mean (H/s) | Readable speed | Percentile | Public results | Std. dev. (H/s) | PTS profile/evaluation |
|---|---|---|---:|---:|---:|---:|---:|---|
| Zotac NVIDIA GeForce RTX 2080 | 6.1.1 | 7-Zip | 636451 | 636.45 kH/s | 50th | 15 | 6712 | [hashcat-1.0.x / 4d816a470aafc62c63dfd70a8fde19b749c15898](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4d816a470aafc62c63dfd70a8fde19b749c15898) |
| Zotac NVIDIA GeForce RTX 2080 | 6.1.1 | MD5 | 38449675556 | 38.45 GH/s | 55th | 15 | 617212257 | [hashcat-1.0.x / 56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9](https://openbenchmarking.org/test/pts/hashcat%26eval%3D56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9) |
| Zotac NVIDIA GeForce RTX 2080 | 6.1.1 | SHA-512 | 1589012381 | 1.589 GH/s | 54th | 15 | 71874414 | [hashcat-1.0.x / 7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5](https://openbenchmarking.org/test/pts/hashcat%26eval%3D7c298d6a1bb8e4160c9dff6f5cfb44bfe364beb5) |
| Zotac NVIDIA GeForce RTX 2080 | 6.1.1 | SHA1 | 12214805397 | 12.215 GH/s | 53rd | 15 | 155477433 | [hashcat-1.0.x / b5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24](https://openbenchmarking.org/test/pts/hashcat%26eval%3Db5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24) |
| Zotac NVIDIA GeForce RTX 2080 | 6.1.1 | TrueCrypt RIPEMD160 + XTS | 457505 | 457.5 kH/s | 50th | 15 | 4387 | [hashcat-1.0.x / 4845413fe722aca0126f6f9941bf32d6f8aaf6be](https://openbenchmarking.org/test/pts/hashcat%26eval%3D4845413fe722aca0126f6f9941bf32d6f8aaf6be) |
| ASUS NVIDIA GeForce RTX 2080 | 6.2.4 | 7-Zip | 650867 | 650.87 kH/s | 39th | 4 | — | [hashcat-1.1.x / 33b0bf9587fcd49c8aad648c3272bbb26334df9c](https://openbenchmarking.org/test/pts/hashcat%26eval%3D33b0bf9587fcd49c8aad648c3272bbb26334df9c) |
| ASUS NVIDIA GeForce RTX 2080 | 6.2.4 | SHA-512 | 1674700000 | 1.6747 GH/s | 46th | 4 | — | [hashcat-1.1.x / 5ed72b49492c93ebaea7b21a1a301f6ab7c80661](https://openbenchmarking.org/test/pts/hashcat%26eval%3D5ed72b49492c93ebaea7b21a1a301f6ab7c80661) |
| ASUS NVIDIA GeForce RTX 2080 | 6.2.4 | SHA1 | 13992775000 | 13.993 GH/s | 45th | 4 | — | [hashcat-1.1.x / 306f31f896ee6afac758df6db7589b6a2a232723](https://openbenchmarking.org/test/pts/hashcat%26eval%3D306f31f896ee6afac758df6db7589b6a2a232723) |
| ASUS NVIDIA GeForce RTX 2080 | 6.2.4 | TrueCrypt RIPEMD160 + XTS | 503840 | 503.84 kH/s | 47th | 4 | — | [hashcat-1.1.x / cf1f40f49c867caac33dcb3ab905e9d065a9cb4a](https://openbenchmarking.org/test/pts/hashcat%26eval%3Dcf1f40f49c867caac33dcb3ab905e9d065a9cb4a) |

**Aggregate rows in this card:** 9. The PTS label is preserved verbatim; vendor/model normalization is used only for this folder name.
