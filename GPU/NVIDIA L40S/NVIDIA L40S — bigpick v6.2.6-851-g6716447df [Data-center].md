# NVIDIA L40S (Data-center (Ada))

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA L40S
- **Конфигурация / Setup:** Data-center (Ada)
- **Версия hashcat / Version:** v6.2.6-851-g6716447df
- **Источник / Source:** [bigpick](https://gist.github.com/bigpick/5d2478209ba820a450148256ae708de0)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 148.0 GH/s |
| 100 | SHA1 | 46768.8 MH/s |
| 1400 | SHA2-256 | 20109.1 MH/s |
| 1700 | SHA2-512 | 6737.8 MH/s |
| 1000 | NTLM | 258.8 GH/s |
| 3200 | bcrypt | 177.0 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 2345.9 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6-851-g6716447df) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

CUDA API (CUDA 12.5)
====================
* Device #1: NVIDIA L40S, 45062/45494 MB, 142MCU

Benchmark relevant options:
===========================
* --benchmark-all
* --backend-devices-virtual=1
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:   148.0 GH/s (16.00ms) @ Accel:64 Loops:1024 Thr:256 Vec:8

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........: 46768.8 MH/s (50.74ms) @ Accel:32 Loops:1024 Thr:512 Vec:1

-------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
-------------------------------------------------------------------------------

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:   258.8 GH/s (8.98ms) @ Accel:32 Loops:1024 Thr:512 Vec:8

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........: 20109.1 MH/s (59.06ms) @ Accel:16 Loops:1024 Thr:512 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  6737.8 MH/s (88.20ms) @ Accel:16 Loops:512 Thr:512 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:   177.0 kH/s (54.00ms) @ Accel:4 Loops:32 Thr:24 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:  2345.9 kH/s (60.59ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
```
