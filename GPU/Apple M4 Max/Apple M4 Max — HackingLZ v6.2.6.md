# Apple M4 Max

- **Вендор / Vendor:** Apple
- **Видеокарта / GPU:** Apple M4 Max
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [HackingLZ](https://gist.github.com/HackingLZ/7ac6bba4ce1ae069b1081d78b9535987)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 22122.7 MH/s |
| 100 | SHA1 | 9774.5 MH/s |
| 1400 | SHA2-256 | 3567.2 MH/s |
| 1700 | SHA2-512 | 708.0 MH/s |
| 1000 | NTLM | 37702.4 MH/s |
| 3200 | bcrypt | 21270 H/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 485.9 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #2: Apple's OpenCL drivers (GPU) are known to be unreliable.
             You have been warned.

METAL API (Metal 367.4)
=======================
* Device #1: Apple M4 Max, 24512/49152 MB, 40MCU

OpenCL API (OpenCL 1.2 (Sep 21 2024 00:08:22)) - Platform #1 [Apple]
====================================================================
* Device #2: Apple M4 Max, skipped

Benchmark relevant options:
===========================
* --benchmark-all
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 22122.7 MH/s (60.15ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  9774.5 MH/s (68.13ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 37702.4 MH/s (70.67ms) @ Accel:2048 Loops:1024 Thr:32 Vec:1

* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  3567.2 MH/s (93.53ms) @ Accel:256 Loops:512 Thr:64 Vec:1

* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:   708.0 MH/s (58.79ms) @ Accel:128 Loops:128 Thr:64 Vec:1

* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    21270 H/s (57.76ms) @ Accel:4 Loops:32 Thr:8 Vec:1

* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   485.9 kH/s (83.40ms) @ Accel:256 Loops:256 Thr:64 Vec:1
```
