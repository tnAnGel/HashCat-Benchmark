# NVIDIA Quadro T2000

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA Quadro T2000
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [9pii9 — gist](https://gist.github.com/9pii9/ac6992e34af6b42638d5b05e182f1984)

> Мобильная (ноутбучная) Quadro на Turing. В исходном gist первый запуск был прерван (^C) — здесь приведён полный второй прогон.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 12766.3 MH/s |
| 100 | SHA1 | 4251.9 MH/s |
| 1400 | SHA2-256 | 1829.9 MH/s |
| 1700 | SHA2-512 | 613.3 MH/s |
| 1000 | NTLM | 21280.4 MH/s |
| 3200 | bcrypt | 12830 H/s |
| 1800 | sha512crypt | 68185 H/s |
| 500 | md5crypt | 4345.3 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 209.4 kH/s |
| 7500 | Kerberos AS-REQ (23) | 238.3 MH/s |
| 13100 | Kerberos TGS-REP (23) | 231.0 MH/s |
| 11300 | Bitcoin wallet.dat | 2775 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 157.7 kH/s |

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

CUDA API (CUDA 12.1)
====================
* Device #1: Quadro T2000, 3705/3768 MB, 16MCU

OpenCL API (OpenCL 3.0 CUDA 12.1.98) - Platform #1 [NVIDIA Corporation]
=======================================================================
* Device #2: Quadro T2000, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 12766.3 MH/s (82.30ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  4251.9 MH/s (62.10ms) @ Accel:64 Loops:1024 Thr:256 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  1829.9 MH/s (72.08ms) @ Accel:64 Loops:256 Thr:512 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:   613.3 MH/s (54.23ms) @ Accel:8 Loops:1024 Thr:256 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   209.4 kH/s (75.38ms) @ Accel:16 Loops:512 Thr:512 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 21280.4 MH/s (49.07ms) @ Accel:128 Loops:1024 Thr:512 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........: 12375.5 MH/s (85.07ms) @ Accel:512 Loops:1024 Thr:128 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 13147.0 MH/s (79.96ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:   954.1 MH/s (69.71ms) @ Accel:16 Loops:1024 Thr:256 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:   509.0 MH/s (65.34ms) @ Accel:16 Loops:1024 Thr:128 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:  4345.3 kH/s (87.49ms) @ Accel:128 Loops:500 Thr:512 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    12830 H/s (67.62ms) @ Accel:4 Loops:32 Thr:16 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:    68185 H/s (45.74ms) @ Accel:512 Loops:1024 Thr:32 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:   238.3 MH/s (70.01ms) @ Accel:32 Loops:1024 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:   231.0 MH/s (72.16ms) @ Accel:256 Loops:128 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:    36648 H/s (73.42ms) @ Accel:16 Loops:1024 Thr:256 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:    20423 H/s (60.60ms) @ Accel:8 Loops:512 Thr:256 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:   239.2 kH/s (50.10ms) @ Accel:64 Loops:255 Thr:64 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:   205.0 kH/s (74.10ms) @ Accel:128 Loops:4096 Thr:32 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    20695 H/s (97.17ms) @ Accel:64 Loops:16384 Thr:32 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    22767 H/s (44.32ms) @ Accel:32 Loops:256 Thr:256 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:   157.7 kH/s (46.77ms) @ Accel:32 Loops:64 Thr:512 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    13785 H/s (49.00ms) @ Accel:8 Loops:512 Thr:256 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  1076.8 kH/s (42.67ms) @ Accel:16 Loops:499 Thr:256 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:     2775 H/s (59.84ms) @ Accel:16 Loops:512 Thr:256 Vec:1

Started: Sun Apr 30 14:17:58 2023
Stopped: Sun Apr 30 14:23:25 2023
```
