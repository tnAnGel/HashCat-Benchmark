# NVIDIA RTX A2000 (6GB desktop)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA RTX A2000
- **Конфигурация / Setup:** 6GB desktop
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [blurbdust](https://gist.github.com/blurbdust/dc575687fe2ec6b66f5fb4ee2dcdcfc4)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 17261.7 MH/s |
| 100 | SHA1 | 5659.5 MH/s |
| 1400 | SHA2-256 | 2433.5 MH/s |
| 1700 | SHA2-512 | 818.5 MH/s |
| 1000 | NTLM | 28582.6 MH/s |
| 3200 | bcrypt | 31319 H/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 289.2 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #1: WARNING! Kernel exec timeout is not disabled.
             This may cause "CL_OUT_OF_RESOURCES" or related errors.
             To disable the timeout, see: https://hashcat.net/q/timeoutpatch
* Device #2: WARNING! Kernel exec timeout is not disabled.
             This may cause "CL_OUT_OF_RESOURCES" or related errors.
             To disable the timeout, see: https://hashcat.net/q/timeoutpatch
CUDA API (CUDA 12.0)
====================
* Device #1: NVIDIA RTX A2000, 5142/6137 MB, 26MCU

OpenCL API (OpenCL 3.0 CUDA 12.0.147) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #2: NVIDIA RTX A2000, skipped

Benchmark relevant options:
===========================
* --benchmark-all
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 17261.7 MH/s (49.66ms) @ Accel:512 Loops:512 Thr:128 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  5659.5 MH/s (76.24ms) @ Accel:128 Loops:512 Thr:256 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 28582.6 MH/s (59.92ms) @ Accel:512 Loops:1024 Thr:128 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  2433.5 MH/s (88.87ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:   818.5 MH/s (65.90ms) @ Accel:16 Loops:512 Thr:256 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    31319 H/s (72.30ms) @ Accel:8 Loops:16 Thr:24 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   289.2 kH/s (90.35ms) @ Accel:32 Loops:512 Thr:256 Vec:1
```
