# NVIDIA GB10 — Hashcat benchmark fragment

- **GPU:** NVIDIA GB10, DGX Spark / MSI EdgeExpert.
- **Версия:** hashcat v7.1.2-484-g64e1bff93; run date 2026-08-19.
- **Options:** `-b -O -w 4 -d 1`; CUDA 13.0, driver 580.159.03.
- **Источник:** [полный опубликованный лог и сведения о системе](https://gist.github.com/racerxdl/135705540e18126a5360fa04ac0c08b0).
- **Примечание:** `-d 1` выбирает CUDA device #1; та же физическая GB10 также видна как OpenCL device #2, не считать её вторым ускорителем.

| Mode | Hash | Speed.#01 |
|---:|---|---:|
| 900 | MD4 | 81156.5 MH/s |
| 0 | MD5 | 53539.7 MH/s |
| 100 | SHA1 | 16698.0 MH/s |
| 1400 | SHA2-256 | 6709.1 MH/s |
| 1700 | SHA2-512 | 2448.8 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 842.4 kH/s |
| 1000 | NTLM | 80000.9 MH/s |
| 3200 | bcrypt | 74820 H/s |

```text
* Device #1: NVIDIA GB10
* --optimized-kernel-enable
* --workload-profile=4

* Hash-Mode 0 (MD5)
Speed.#01........: 53539.7 MH/s (264.14ms) @ Accel:288 Loops:1024 Thr:1024 Vec:4

* Hash-Mode 1400 (SHA2-256)
Speed.#01........: 6709.1 MH/s (477.02ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1

* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
Speed.#01........: 842.4 kH/s (479.71ms) @ Accel:38 Loops:1024 Thr:896 Vec:1

* Hash-Mode 1000 (NTLM)
Speed.#01........: 80000.9 MH/s (161.96ms) @ Accel:320 Loops:1024 Thr:896 Vec:8

* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
Speed.#01........: 74820 H/s (473.01ms) @ Accel:32 Loops:32 Thr:24 Vec:1
```
