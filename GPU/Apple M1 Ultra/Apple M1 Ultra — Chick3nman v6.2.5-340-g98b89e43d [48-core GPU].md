# Apple M1 Ultra (48-core GPU)

- **Вендор / Vendor:** Apple
- **Видеокарта / GPU:** Apple M1 Ultra
- **Конфигурация / Setup:** 48-core GPU
- **Версия hashcat / Version:** v6.2.5-340-g98b89e43d
- **Источник / Source:** [Chick3nman](https://gist.github.com/Chick3nman/ccfb883d2d267d94770869b09f5b96ed)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 17137.0 MH/s |
| 100 | SHA1 | 6097.5 MH/s |
| 1400 | SHA2-256 | 1818.9 MH/s |
| 1700 | SHA2-512 | 575.0 MH/s |
| 1000 | NTLM | 28630.3 MH/s |
| 3200 | bcrypt | 10077 H/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 297.0 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.5-340-g98b89e43d) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #2: Apple's OpenCL drivers (GPU) are known to be unreliable.
             You have been warned.

METAL API (Metal 258.18)
========================
* Device #1: Apple M1 Ultra, 24512/49152 MB, 48MCU

OpenCL API (OpenCL 1.2 (Dec 17 2021 16:33:08)) - Platform #1 [Apple]
====================================================================
* Device #2: Apple M1 Ultra, skipped

Benchmark relevant options:
===========================
* --benchmark-all
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 17137.0 MH/s (92.76ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  6097.5 MH/s (64.89ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

------------------------
* Hash-Mode 1000 (NTLM)
------------------------

Speed.#1.........: 28630.3 MH/s (55.16ms) @ Accel:2048 Loops:512 Thr:32 Vec:1

----------------------------
* Hash-Mode 1400 (SHA2-256)
----------------------------

Speed.#1.........:  1818.9 MH/s (54.07ms) @ Accel:128 Loops:128 Thr:128 Vec:1

----------------------------
* Hash-Mode 1700 (SHA2-512)
----------------------------

Speed.#1.........:   575.0 MH/s (86.38ms) @ Accel:32 Loops:256 Thr:128 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    10077 H/s (111.55ms) @ Accel:12 Loops:8 Thr:8 Vec:1

--------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
--------------------------------------------------------------

Speed.#1.........:   297.0 kH/s (82.11ms) @ Accel:128 Loops:256 Thr:64 Vec:1
```
