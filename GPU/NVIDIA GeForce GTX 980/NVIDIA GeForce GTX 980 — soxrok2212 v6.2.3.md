# NVIDIA GeForce GTX 980

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce GTX 980
- **Версия hashcat / Version:** v6.2.3
- **Источник / Source:** [soxrok2212](https://gist.github.com/soxrok2212/52df2d6e45764591eeb614ed4fc25bc5)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 11374.4 MH/s |
| 100 | SHA1 | 4398.0 MH/s |
| 1400 | SHA2-256 | 1497.4 MH/s |
| 1700 | SHA2-512 | 490.2 MH/s |
| 1000 | NTLM | 23239.9 MH/s |
| 3200 | bcrypt | 11374 H/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 186.2 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
CUDA API (CUDA 11.4)
====================
* Device #1: NVIDIA GeForce GTX 980, 3966/4043 MB, 16MCU

Benchmark relevant options:
===========================
* --benchmark-all
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#2.........: 11374.4 MH/s (88.10ms) @ Accel:64 Loops:1024 Thr:1024 Vec:8

Hashmode: 100 - SHA1

Speed.#2.........:  4398.0 MH/s (60.71ms) @ Accel:64 Loops:256 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#2.........: 23239.9 MH/s (45.84ms) @ Accel:64 Loops:1024 Thr:1024 Vec:8

Hashmode: 1400 - SHA2-256

Speed.#2.........:  1497.4 MH/s (86.86ms) @ Accel:16 Loops:512 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#2.........:   490.2 MH/s (68.08ms) @ Accel:64 Loops:32 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#2.........:    11374 H/s (65.54ms) @ Accel:8 Loops:16 Thr:12 Vec:1

Hashmode: 22000 - WPA-PBKDF2-PMKID+EAPOL (Iterations: 4095)

Speed.#2.........:   186.2 kH/s (84.40ms) @ Accel:32 Loops:128 Thr:1024 Vec:1

Hashmode: 22100 - BitLocker (Iterations: 1048576)

Speed.#2.........:      639 H/s (96.84ms) @ Accel:1 Loops:4096 Thr:1024 Vec:1
```
