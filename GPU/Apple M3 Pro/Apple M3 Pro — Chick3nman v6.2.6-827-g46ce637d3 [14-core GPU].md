# Apple M3 Pro (14-core GPU)

- **Вендор / Vendor:** Apple
- **Видеокарта / GPU:** Apple M3 Pro
- **Конфигурация / Setup:** 14-core GPU
- **Версия hashcat / Version:** v6.2.6-827-g46ce637d3
- **Источник / Source:** [Chick3nman](https://gist.github.com/Chick3nman/fdf7f9ddcc0a65f6725aefede99ada4e)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 6801.5 MH/s |
| 100 | SHA1 | 3019.9 MH/s |
| 1400 | SHA2-256 | 1069.1 MH/s |
| 1700 | SHA2-512 | 219.9 MH/s |
| 1000 | NTLM | 11693.9 MH/s |
| 3200 | bcrypt | 6032 H/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 145.7 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6-827-g46ce637d3) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

METAL API (Metal 341.29)
========================
* Device #1: Apple M3 Pro, 6112/12288 MB, 14MCU

OpenCL API (OpenCL 1.2 (Sep 28 2023 02:31:39)) - Platform #1 [Apple]
====================================================================
* Device #2: Apple M3 Pro, skipped

Benchmark relevant options:
===========================
* --benchmark-all
* --backend-devices=1
* --backend-devices-virtual=1
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:  6801.5 MH/s (68.54ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  3019.9 MH/s (77.24ms) @ Accel:512 Loops:1024 Thr:32 Vec:1

------------------------
* Hash-Mode 1000 (NTLM)
------------------------

Speed.#1.........: 11693.9 MH/s (79.78ms) @ Accel:2048 Loops:1024 Thr:32 Vec:1

----------------------------
* Hash-Mode 1400 (SHA2-256)
----------------------------

Speed.#1.........:  1069.1 MH/s (54.35ms) @ Accel:256 Loops:256 Thr:64 Vec:1

----------------------------
* Hash-Mode 1700 (SHA2-512)
----------------------------

Speed.#1.........:   219.9 MH/s (66.22ms) @ Accel:256 Loops:64 Thr:64 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:     6032 H/s (72.51ms) @ Accel:16 Loops:8 Thr:8 Vec:1

--------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
--------------------------------------------------------------

Speed.#1.........:   145.7 kH/s (48.74ms) @ Accel:256 Loops:128 Thr:64 Vec:1
```
