# NVIDIA L4 (Data-center (Ada))

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA L4
- **Конфигурация / Setup:** Data-center (Ada)
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [blurbdust](https://gist.github.com/blurbdust/0a3052ccb7bea3e775089d84baff6dc5)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 39827.9 MH/s |
| 1400 | SHA2-256 | 5370.6 MH/s |
| 1700 | SHA2-512 | 1798.0 MH/s |
| 1000 | NTLM | 68140.9 MH/s |
| 3200 | bcrypt | 59822 H/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 621.5 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

CUDA API (CUDA 12.0)
====================
* Device #1: NVIDIA L4, 22331/22518 MB, 58MCU

OpenCL API (OpenCL 3.0 CUDA 12.0.151) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #2: NVIDIA L4, skipped

Benchmark relevant options:
===========================
* --benchmark-all
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 39827.9 MH/s (48.51ms) @ Accel:128 Loops:1024 Thr:256 Vec:8

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 68140.9 MH/s (28.16ms) @ Accel:128 Loops:1024 Thr:256 Vec:8

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  5370.6 MH/s (90.24ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  1798.0 MH/s (67.31ms) @ Accel:32 Loops:128 Thr:512 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    59822 H/s (66.63ms) @ Accel:4 Loops:32 Thr:24 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   621.5 kH/s (92.91ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
```
