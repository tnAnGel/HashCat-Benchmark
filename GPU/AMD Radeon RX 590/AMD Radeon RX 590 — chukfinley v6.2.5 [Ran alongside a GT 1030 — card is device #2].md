# AMD Radeon RX 590 (Ran alongside a GT 1030 — card is device #2)

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX 590
- **Конфигурация / Setup:** Ran alongside a GT 1030 — card is device #2
- **Версия hashcat / Version:** v6.2.5
- **Источник / Source:** [chukfinley](https://gist.github.com/chukfinley/175f08f1125bfd3fc83dfdda3361a739)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 14031.9 MH/s |
| 100 | SHA1 | 4507.7 MH/s |
| 1400 | SHA2-256 | 1923.1 MH/s |
| 1700 | SHA2-512 | 485.5 MH/s |
| 1000 | NTLM | 22570.7 MH/s |
| 3200 | bcrypt | 10636 H/s |
| 1800 | sha512crypt | 27890 H/s |
| 500 | md5crypt | 5269.2 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 236.4 kH/s |
| 7500 | Kerberos AS-REQ (23) | 213.6 MH/s |
| 13100 | Kerberos TGS-REP (23) | — |
| 11300 | Bitcoin wallet.dat | 2357 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 170.6 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.5) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

Successfully initialized NVIDIA CUDA library.

Failed to initialize NVIDIA RTC library.

* Device #1: CUDA SDK Toolkit not installed or incorrectly installed.
             CUDA SDK Toolkit required for proper device support and utilization.
             Falling back to OpenCL runtime.

* Device #1: WARNING! Kernel exec timeout is not disabled.
             This may cause "CL_OUT_OF_RESOURCES" or related errors.
             To disable the timeout, see: https://hashcat.net/q/timeoutpatch
OpenCL API (OpenCL 3.0 CUDA 12.0.133) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #1: NVIDIA GeForce GT 1030, 3584/4031 MB (1007 MB allocatable), 3MCU

OpenCL API (OpenCL 2.1 AMD-APP (3380.4)) - Platform #2 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #2: Radeon RX 590 Series, 8064/8192 MB (6745 MB allocatable), 36MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:  2871.4 MH/s (68.78ms) @ Accel:1024 Loops:512 Thr:128 Vec:8
Speed.#2.........: 14031.9 MH/s (85.36ms) @ Accel:128 Loops:1024 Thr:256 Vec:1
Speed.#*.........: 16903.3 MH/s

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  1055.1 MH/s (93.93ms) @ Accel:512 Loops:512 Thr:128 Vec:1
Speed.#2.........:  4507.7 MH/s (66.39ms) @ Accel:64 Loops:512 Thr:256 Vec:1
Speed.#*.........:  5562.8 MH/s

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:   370.5 MH/s (66.77ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#2.........:  1923.1 MH/s (78.09ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#*.........:  2293.6 MH/s

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:   110.8 MH/s (56.50ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#2.........:   485.5 MH/s (76.99ms) @ Accel:32 Loops:256 Thr:128 Vec:1
Speed.#*.........:   596.3 MH/s

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:    54607 H/s (52.28ms) @ Accel:64 Loops:256 Thr:256 Vec:1
Speed.#2.........:   236.4 kH/s (77.20ms) @ Accel:16 Loops:1024 Thr:128 Vec:1
Speed.#*.........:   291.0 kH/s

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:  5731.2 MH/s (69.08ms) @ Accel:512 Loops:1024 Thr:256 Vec:8
Speed.#2.........: 22570.7 MH/s (52.85ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 28302.0 MH/s

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:  3086.3 MH/s (64.31ms) @ Accel:512 Loops:1024 Thr:128 Vec:1
Speed.#2.........: 13827.0 MH/s (86.67ms) @ Accel:128 Loops:1024 Thr:256 Vec:1
Speed.#*.........: 16913.3 MH/s

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........:  2806.5 MH/s (70.25ms) @ Accel:1024 Loops:512 Thr:128 Vec:2
Speed.#2.........: 13320.9 MH/s (89.91ms) @ Accel:256 Loops:1024 Thr:128 Vec:1
Speed.#*.........: 16127.4 MH/s

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:   211.6 MH/s (58.65ms) @ Accel:32 Loops:512 Thr:256 Vec:1
Speed.#2.........:   955.8 MH/s (78.61ms) @ Accel:16 Loops:1024 Thr:128 Vec:1
Speed.#*.........:  1167.4 MH/s

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

* Device #2: Skipping (hash-mode 1500)
             This is due to a known CUDA/HIP/OpenCL runtime/driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
Speed.#1.........:   105.3 MH/s (58.84ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#*.........:   105.3 MH/s

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:  1083.6 kH/s (68.90ms) @ Accel:1024 Loops:250 Thr:128 Vec:1
Speed.#2.........:  5269.2 kH/s (48.45ms) @ Accel:256 Loops:250 Thr:128 Vec:1
Speed.#*.........:  6352.8 kH/s

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:     2368 H/s (72.70ms) @ Accel:32 Loops:16 Thr:11 Vec:1
Speed.#2.........:    10636 H/s (90.23ms) @ Accel:64 Loops:32 Thr:16 Vec:1
Speed.#*.........:    13004 H/s

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:     9689 H/s (79.39ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#2.........:    27890 H/s (57.61ms) @ Accel:512 Loops:128 Thr:128 Vec:1
Speed.#*.........:    37579 H/s

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........: 40143.8 kH/s (78.10ms) @ Accel:64 Loops:512 Thr:32 Vec:1
Speed.#2.........:   213.6 MH/s (87.88ms) @ Accel:64 Loops:128 Thr:64 Vec:1
Speed.#*.........:   253.8 MH/s

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

* Device #2: Skipping (hash-mode 13100)
             This is due to a known CUDA/HIP/OpenCL runtime/driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
Speed.#1.........: 38468.0 kH/s (40.64ms) @ Accel:64 Loops:256 Thr:32 Vec:1
Speed.#*.........: 38468.0 kH/s

---------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1) [Iterations: 23999]
---------------------------------------------------------------

* Device #2: Skipping (hash-mode 15300)
             This is due to a known CUDA/HIP/OpenCL runtime/driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
Speed.#1.........:     8931 H/s (57.56ms) @ Accel:64 Loops:256 Thr:256 Vec:1
Speed.#*.........:     8931 H/s

---------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2) [Iterations: 12899]
---------------------------------------------------------------

Speed.#1.........:     4655 H/s (50.51ms) @ Accel:8 Loops:512 Thr:256 Vec:1
Speed.#2.........:    12382 H/s (57.86ms) @ Accel:16 Loops:64 Thr:256 Vec:1
Speed.#*.........:    17037 H/s

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:    22582 H/s (58.03ms) @ Accel:4 Loops:1023 Thr:256 Vec:1
Speed.#2.........:   147.6 kH/s (57.47ms) @ Accel:32 Loops:63 Thr:128 Vec:1
Speed.#*.........:   170.1 kH/s

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:    20780 H/s (54.27ms) @ Accel:64 Loops:4096 Thr:32 Vec:1
Speed.#2.........:   239.6 kH/s (71.34ms) @ Accel:8 Loops:4096 Thr:256 Vec:1
Speed.#*.........:   260.4 kH/s

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:     2581 H/s (69.83ms) @ Accel:32 Loops:16384 Thr:32 Vec:1
Speed.#2.........:    31156 H/s (73.18ms) @ Accel:4 Loops:16384 Thr:256 Vec:1
Speed.#*.........:    33737 H/s

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:     4670 H/s (80.13ms) @ Accel:32 Loops:512 Thr:256 Vec:1
Speed.#2.........:    24162 H/s (94.39ms) @ Accel:64 Loops:128 Thr:256 Vec:1
Speed.#*.........:    28832 H/s

-----------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit) [Iterations: 1999]
-----------------------------------------------------------------------

Speed.#1.........:    25438 H/s (76.13ms) @ Accel:64 Loops:1024 Thr:32 Vec:1
Speed.#2.........:   170.6 kH/s (50.55ms) @ Accel:64 Loops:128 Thr:64 Vec:1
Speed.#*.........:   196.0 kH/s

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:     4614 H/s (53.61ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#2.........:    50574 H/s (60.24ms) @ Accel:32 Loops:256 Thr:256 Vec:1
Speed.#*.........:    55187 H/s

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:   191.5 kH/s (70.08ms) @ Accel:32 Loops:499 Thr:256 Vec:1
Speed.#2.........:  1525.1 kH/s (81.21ms) @ Accel:128 Loops:62 Thr:256 Vec:1
Speed.#*.........:  1716.6 kH/s

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:      599 H/s (69.38ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#2.........:     2357 H/s (70.36ms) @ Accel:1024 Loops:128 Thr:256 Vec:1
Speed.#*.........:     2956 H/s

Started: Fri Feb 17 22:43:40 2023
Stopped: Fri Feb 17 22:52:06 2023
```
