# NVIDIA GeForce RTX 3090 Ti (2x rig)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce RTX 3090 Ti
- **Конфигурация / Setup:** 2x rig
- **Версия hashcat / Version:** v6.2.5
- **Источник / Source:** [shivams](https://gist.github.com/shivams/48a0c9d91dab140d68309c7a93131f08)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 79072.3 MH/s |
| 100 | SHA1 | 24853.9 MH/s |
| 1400 | SHA2-256 | 10774.5 MH/s |
| 1700 | SHA2-512 | 3612.0 MH/s |
| 1000 | NTLM | 142.6 GH/s |
| 3200 | bcrypt | 91040 H/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 1252.9 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.5) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

CUDA API (CUDA 12.4)
====================
* Device #1: NVIDIA GeForce RTX 3090 Ti, 23973/24240 MB, 84MCU
* Device #2: NVIDIA GeForce RTX 3090 Ti, 23973/24240 MB, 84MCU

OpenCL API (OpenCL 3.0 CUDA 12.4.125) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #3: NVIDIA GeForce RTX 3090 Ti, skipped
* Device #4: NVIDIA GeForce RTX 3090 Ti, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 79072.3 MH/s (35.16ms) @ Accel:128 Loops:1024 Thr:256 Vec:8
Speed.#2.........: 79070.6 MH/s (35.14ms) @ Accel:128 Loops:1024 Thr:256 Vec:8
Speed.#*.........:   158.1 GH/s

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........: 24853.9 MH/s (56.20ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#2.........: 24726.6 MH/s (56.54ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#*.........: 49580.5 MH/s

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........: 10774.5 MH/s (64.76ms) @ Accel:64 Loops:256 Thr:512 Vec:1
Speed.#2.........: 10774.5 MH/s (64.75ms) @ Accel:64 Loops:256 Thr:512 Vec:1
Speed.#*.........: 21549.0 MH/s

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  3612.0 MH/s (48.36ms) @ Accel:8 Loops:512 Thr:512 Vec:1
Speed.#2.........:  3588.6 MH/s (48.72ms) @ Accel:8 Loops:512 Thr:512 Vec:1
Speed.#*.........:  7200.6 MH/s

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:  1252.9 kH/s (67.20ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#2.........:  1259.4 kH/s (67.20ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#*.........:  2512.2 kH/s

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:   142.6 GH/s (19.24ms) @ Accel:128 Loops:1024 Thr:256 Vec:8
Speed.#2.........:   143.5 GH/s (19.07ms) @ Accel:128 Loops:1024 Thr:256 Vec:8
Speed.#*.........:   286.0 GH/s

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........: 74028.5 MH/s (18.67ms) @ Accel:128 Loops:1024 Thr:128 Vec:1
Speed.#2.........: 73954.1 MH/s (18.78ms) @ Accel:128 Loops:1024 Thr:128 Vec:1
Speed.#*.........:   148.0 GH/s

-----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
-----------------------------------------------------------------

Speed.#1.........:    91040 H/s (65.42ms) @ Accel:256 Loops:32 Thr:24 Vec:1
Speed.#2.........:    91142 H/s (64.95ms) @ Accel:256 Loops:32 Thr:24 Vec:1
Speed.#*.........:   182.2 kH/s
```
