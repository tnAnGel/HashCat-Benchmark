# Apple M1 (8-core GPU)

- **Вендор / Vendor:** Apple
- **Видеокарта / GPU:** Apple M1
- **Конфигурация / Setup:** 8-core GPU
- **Версия hashcat / Version:** v6.2.5-85-g0abdcb1ae+
- **Источник / Source:** [matrix](https://gist.github.com/matrix/c56402f6eb47a2f882838f6b4b326875)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 2822.0 MH/s |
| 100 | SHA1 | 1000.8 MH/s |
| 1400 | SHA2-256 | 300.0 MH/s |
| 1700 | SHA2-512 | 97643.3 kH/s |
| 1000 | NTLM | 4790.0 MH/s |
| 3200 | bcrypt | 2140 H/s |
| 1800 | sha512crypt | — |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 48852 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.5-85-g0abdcb1ae+) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #2: Apple's OpenCL drivers (GPU) are known to be unreliable.
             You have been warned.

METAL API (Metal 258.18)
========================
* Device #1: Apple M1, 5408/10922 MB, 8MCU

OpenCL API (OpenCL 1.2 (Dec 17 2021 16:38:41)) - Platform #1 [Apple]
====================================================================
* Device #2: Apple M1, skipped

Benchmark relevant options:
===========================
* --benchmark-all
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:  2822.0 MH/s (93.73ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  1000.8 MH/s (65.71ms) @ Accel:256 Loops:1024 Thr:32 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:  4790.0 MH/s (54.66ms) @ Accel:2048 Loops:512 Thr:32 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:   300.0 MH/s (54.65ms) @ Accel:256 Loops:128 Thr:64 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........: 97643.3 kH/s (84.59ms) @ Accel:64 Loops:128 Thr:128 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

* Device #1: Skipping (hash-mode 1800)
             This is due to a known Metal runtime and/or device driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:     2140 H/s (54.84ms) @ Accel:4 Loops:16 Thr:8 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:    48852 H/s (82.96ms) @ Accel:512 Loops:128 Thr:32 Vec:1
```
