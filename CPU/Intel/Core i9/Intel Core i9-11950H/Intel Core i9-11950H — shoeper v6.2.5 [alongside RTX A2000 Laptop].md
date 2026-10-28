# Intel Core i9-11950H

- **Вендор / Vendor:** Intel
- **Процессор / CPU:** 11th Gen Intel Core i9-11950H (8/16)
- **Версия hashcat / Version:** v6.2.5
- **Источник / Source:** [shoeper — gist](https://gist.github.com/shoeper/b896e6f851dc82ecebf4645cae8af581)
- **Примечание / Note:** смешанный полный прогон; Device #1 — NVIDIA RTX A2000 Laptop GPU, Device #2 (`Speed.#2`) — CPU через PoCL. Сырой вывод сохранён целиком.

## Ключевые результаты / Highlights (Speed.#2 = CPU)

| Mode | Алгоритм | Скорость CPU |
|-----:|----------|-------------:|
| 0 | MD5 | 1546.5 MH/s |
| 100 | SHA1 | 794.9 MH/s |
| 1400 | SHA2-256 | 350.3 MH/s |
| 1700 | SHA2-512 | 108.8 MH/s |
| 1000 | NTLM | 2631.8 MH/s |
| 3200 | bcrypt | 99 H/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 27234 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.5) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #1: WARNING! Kernel exec timeout is not disabled.
             This may cause "CL_OUT_OF_RESOURCES" or related errors.
             To disable the timeout, see: https://hashcat.net/q/timeoutpatch
nvmlDeviceGetFanSpeed(): Not Supported

CUDA API (CUDA 11.6)
====================
* Device #1: NVIDIA RTX A2000 Laptop GPU, 3312/3913 MB, 20MCU

OpenCL API (OpenCL 3.0 PoCL 3.0+debian  Linux, None+Asserts, RELOC, LLVM 13.0.1, SLEEF, DISTRO, POCL_DEBUG) - Platform #1 [The pocl project]
============================================================================================================================================
* Device #2: pthread-11th Gen Intel(R) Core(TM) i9-11950H @ 2.60GHz, 14852/29769 MB (4096 MB allocatable), 16MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:  2117.3 MH/s (156.01ms) @ Accel:64 Loops:512 Thr:512 Vec:1
Speed.#2.........:  1546.5 MH/s (10.40ms) @ Accel:1024 Loops:1024 Thr:1 Vec:16
Speed.#*.........:  3663.8 MH/s

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:   586.7 MH/s (70.78ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#2.........:   794.9 MH/s (20.08ms) @ Accel:1024 Loops:1024 Thr:1 Vec:16
Speed.#*.........:  1381.5 MH/s

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:   227.7 MH/s (90.85ms) @ Accel:16 Loops:128 Thr:512 Vec:1
Speed.#2.........:   350.3 MH/s (23.32ms) @ Accel:1024 Loops:512 Thr:1 Vec:16
Speed.#*.........:   578.0 MH/s

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........: 79298.0 kH/s (32.51ms) @ Accel:16 Loops:256 Thr:32 Vec:1
Speed.#2.........:   108.8 MH/s (76.72ms) @ Accel:1024 Loops:512 Thr:1 Vec:8
Speed.#*.........:   188.1 MH/s

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:    19015 H/s (31.44ms) @ Accel:8 Loops:256 Thr:64 Vec:1
Speed.#2.........:    27234 H/s (64.50ms) @ Accel:512 Loops:1024 Thr:1 Vec:16
Speed.#*.........:    46249 H/s

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:  2423.7 MH/s (68.04ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#2.........:  2631.8 MH/s (6.03ms) @ Accel:1024 Loops:1024 Thr:1 Vec:16
Speed.#*.........:  5055.4 MH/s

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:  1740.0 MH/s (95.08ms) @ Accel:256 Loops:1024 Thr:32 Vec:1
Speed.#2.........:   122.1 MH/s (67.10ms) @ Accel:512 Loops:1024 Thr:1 Vec:16
Speed.#*.........:  1862.1 MH/s

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........:  1469.6 MH/s (26.33ms) @ Accel:16 Loops:256 Thr:512 Vec:1
Speed.#2.........:  1793.6 MH/s (8.94ms) @ Accel:1024 Loops:1024 Thr:1 Vec:16
Speed.#*.........:  3263.2 MH/s

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:   121.3 MH/s (42.61ms) @ Accel:1 Loops:512 Thr:512 Vec:1
Speed.#2.........:   103.0 MH/s (40.28ms) @ Accel:256 Loops:1024 Thr:1 Vec:16
Speed.#*.........:   224.3 MH/s

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........: 50725.2 kH/s (101.74ms) @ Accel:8 Loops:1024 Thr:32 Vec:1
Speed.#2.........:  4768.8 kH/s (51.77ms) @ Accel:16 Loops:1024 Thr:1 Vec:16
Speed.#*.........: 55494.0 kH/s

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:   633.8 kH/s (45.31ms) @ Accel:2 Loops:1000 Thr:1024 Vec:1
Speed.#2.........:    67913 H/s (59.25ms) @ Accel:512 Loops:500 Thr:1 Vec:16
Speed.#*.........:   701.7 kH/s

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:     1664 H/s (63.23ms) @ Accel:72 Loops:2 Thr:24 Vec:1
Speed.#2.........:       99 H/s (3.27ms) @ Accel:16 Loops:32 Thr:1 Vec:1
Speed.#*.........:     1763 H/s

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:    11377 H/s (70.29ms) @ Accel:1024 Loops:128 Thr:32 Vec:1
Speed.#2.........:     3116 H/s (65.30ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8
Speed.#*.........:    14493 H/s

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........: 39307.1 kH/s (66.39ms) @ Accel:64 Loops:64 Thr:32 Vec:1
Speed.#2.........:  4843.7 kH/s (53.77ms) @ Accel:16 Loops:1024 Thr:1 Vec:16
Speed.#*.........: 44150.8 kH/s

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........: 32431.3 kH/s (80.53ms) @ Accel:8 Loops:512 Thr:32 Vec:1
Speed.#2.........:  4965.5 kH/s (52.46ms) @ Accel:16 Loops:1024 Thr:1 Vec:16
Speed.#*.........: 37396.8 kH/s

---------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1) [Iterations: 23999]
---------------------------------------------------------------

Speed.#1.........:     4716 H/s (91.68ms) @ Accel:16 Loops:128 Thr:256 Vec:1
Speed.#2.........:     5668 H/s (60.97ms) @ Accel:1024 Loops:512 Thr:1 Vec:16
Speed.#*.........:    10384 H/s

---------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2) [Iterations: 12899]
---------------------------------------------------------------

Speed.#1.........:     2413 H/s (83.50ms) @ Accel:2 Loops:128 Thr:512 Vec:1
Speed.#2.........:     3868 H/s (80.78ms) @ Accel:256 Loops:1024 Thr:1 Vec:8
Speed.#*.........:     6281 H/s

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:    21139 H/s (54.89ms) @ Accel:4 Loops:63 Thr:256 Vec:1
Speed.#2.........:    42182 H/s (93.01ms) @ Accel:256 Loops:1023 Thr:1 Vec:8
Speed.#*.........:    63321 H/s

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:    23212 H/s (102.83ms) @ Accel:2 Loops:4096 Thr:256 Vec:1
Speed.#2.........:     3730 H/s (67.94ms) @ Accel:64 Loops:4096 Thr:1 Vec:16
Speed.#*.........:    26942 H/s

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:     3757 H/s (168.21ms) @ Accel:1 Loops:16384 Thr:512 Vec:1
Speed.#2.........:      461 H/s (69.28ms) @ Accel:32 Loops:16384 Thr:1 Vec:16
Speed.#*.........:     4218 H/s

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:     3247 H/s (48.78ms) @ Accel:4 Loops:128 Thr:512 Vec:1
Speed.#2.........:     3816 H/s (64.84ms) @ Accel:512 Loops:1024 Thr:1 Vec:16
Speed.#*.........:     7063 H/s

-----------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit) [Iterations: 1999]
-----------------------------------------------------------------------

Speed.#1.........:    21740 H/s (54.85ms) @ Accel:8 Loops:32 Thr:512 Vec:1
Speed.#2.........:    23794 H/s (83.73ms) @ Accel:256 Loops:1024 Thr:1 Vec:16
Speed.#*.........:    45534 H/s

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:     3753 H/s (56.46ms) @ Accel:4 Loops:128 Thr:512 Vec:1
Speed.#2.........:     1397 H/s (60.90ms) @ Accel:128 Loops:1024 Thr:1 Vec:16
Speed.#*.........:     5150 H/s

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:   186.4 kH/s (80.17ms) @ Accel:8 Loops:124 Thr:512 Vec:1
Speed.#2.........:   250.4 kH/s (59.26ms) @ Accel:1024 Loops:499 Thr:1 Vec:16
Speed.#*.........:   436.8 kH/s

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:      307 H/s (67.60ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#2.........:      477 H/s (10.68ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8
Speed.#*.........:      784 H/s

Started: Thu Jul 14 12:40:22 2022
Stopped: Thu Jul 14 12:54:36 2022
```
