# NVIDIA GeForce RTX 3050 Laptop GPU

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce RTX 3050 Laptop GPU
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [HexRx — gist](https://gist.github.com/HexRx/ac9b967aa78748a3488e20bd37776929)

> Ubuntu, ядро 6.8.0, драйвер NVIDIA 535, CUDA 12.2. Device #2 — та же карта через OpenCL (skipped).

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 11450.6 MH/s |
| 100 | SHA1 | 3635.2 MH/s |
| 1400 | SHA2-256 | 1552.0 MH/s |
| 1700 | SHA2-512 | 516.7 MH/s |
| 1000 | NTLM | 19822.7 MH/s |
| 3200 | bcrypt | 16933 H/s |
| 1800 | sha512crypt | 69548 H/s |
| 500 | md5crypt | 4171.8 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 177.8 kH/s |
| 7500 | Kerberos AS-REQ (23) | 257.4 MH/s |
| 13100 | Kerberos TGS-REP (23) | 252.3 MH/s |
| 11300 | Bitcoin wallet.dat | 2348 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 132.2 kH/s |

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
nvmlDeviceGetFanSpeed(): Not Supported

CUDA API (CUDA 12.2)
====================
* Device #1: NVIDIA GeForce RTX 3050 Laptop GPU, 3822/3901 MB, 16MCU

OpenCL API (OpenCL 3.0 CUDA 12.2.149) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #2: NVIDIA GeForce RTX 3050 Laptop GPU, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 11450.6 MH/s (92.60ms) @ Accel:512 Loops:1024 Thr:128 Vec:8

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  3635.2 MH/s (72.81ms) @ Accel:32 Loops:1024 Thr:512 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  1552.0 MH/s (85.36ms) @ Accel:32 Loops:1024 Thr:256 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:   516.7 MH/s (63.99ms) @ Accel:4 Loops:1024 Thr:512 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   177.8 kH/s (89.19ms) @ Accel:8 Loops:1024 Thr:512 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 19822.7 MH/s (53.07ms) @ Accel:2048 Loops:1024 Thr:32 Vec:8

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........: 10749.0 MH/s (48.94ms) @ Accel:256 Loops:1024 Thr:128 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 11091.3 MH/s (95.47ms) @ Accel:128 Loops:1024 Thr:512 Vec:2

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:   793.4 MH/s (83.53ms) @ Accel:16 Loops:1024 Thr:256 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:   439.3 MH/s (75.36ms) @ Accel:8 Loops:1024 Thr:256 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:  4171.8 kH/s (49.78ms) @ Accel:32 Loops:1000 Thr:512 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    16933 H/s (77.28ms) @ Accel:4 Loops:32 Thr:24 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:    69548 H/s (92.30ms) @ Accel:256 Loops:512 Thr:256 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:   257.4 MH/s (64.31ms) @ Accel:256 Loops:128 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:   252.3 MH/s (65.60ms) @ Accel:256 Loops:128 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:    31523 H/s (87.80ms) @ Accel:32 Loops:512 Thr:256 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:    17443 H/s (70.51ms) @ Accel:2 Loops:1024 Thr:512 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:   213.7 kH/s (72.96ms) @ Accel:512 Loops:31 Thr:64 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:   163.5 kH/s (95.85ms) @ Accel:32 Loops:4096 Thr:128 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    20950 H/s (96.40ms) @ Accel:8 Loops:16384 Thr:256 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    19252 H/s (51.54ms) @ Accel:8 Loops:512 Thr:512 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:   132.2 kH/s (55.29ms) @ Accel:8 Loops:256 Thr:512 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    24620 H/s (54.46ms) @ Accel:4 Loops:1024 Thr:512 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  1064.7 kH/s (49.75ms) @ Accel:8 Loops:499 Thr:512 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:     2348 H/s (70.51ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1

Started: Sun Jan 11 14:12:13 2026
Stopped: Sun Jan 11 14:14:43 2026
```
