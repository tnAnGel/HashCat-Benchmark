# Apple M3 (Source run covers MD5/SHA1/SHA2-256 only)

- **Вендор / Vendor:** Apple
- **Видеокарта / GPU:** Apple M3
- **Конфигурация / Setup:** Source run covers MD5/SHA1/SHA2-256 only
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [Chw41](https://github.com/Chw41/chw41.github.io)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 3268.4 MH/s |
| 100 | SHA1 | 911.7 MH/s |
| 1400 | SHA2-256 | 536.3 MH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #2: Apple's OpenCL drivers (GPU) are known to be unreliable.
             You have been warned.

METAL API (Metal 367.6)
=======================
* Device #1: Apple M3, 8160/16384 MB, 10MCU

OpenCL API (OpenCL 1.2 (Dec 13 2024 23:09:21)) - Platform #1 [Apple]
====================================================================
* Device #2: Apple M3, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:  3268.4 MH/s (101.74ms) @ Accel:1024 Loops:256 Thr:128 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:   911.7 MH/s (90.38ms) @ Accel:256 Loops:1024 Thr:32 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:   536.3 MH/s (77.45ms) @ Accel:32 Loops:1024 Thr:128 Vec:1
```
