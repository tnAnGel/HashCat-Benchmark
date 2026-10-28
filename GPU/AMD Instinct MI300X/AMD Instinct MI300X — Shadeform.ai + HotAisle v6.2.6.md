# AMD Instinct MI300X

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Instinct MI300X
- **Версия hashcat / Version:** v6.2.6-854-g3033ed126
- **Источник / Source:** [публичный сырой вывод](https://gitlab.com/-/snippets/4805487)
- **Параметры / Options:** `-b` (исходные параметры — см. лог)
- **Примечание / Note:** одна MI300X, HIP 6.2.41134 и OpenCL AMD-APP 3625.0. Опубликован частичный сырой стандартный benchmark; исходный --benchmark-all падал на PKZIP, поэтому PKZIP и возможные последующие режимы отсутствуют. Сборка hashcat сторонняя, не официальный релиз.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость |
|-----:|----------|---------:|
| 0 | MD5 | 163.7 GH/s |
| 100 | SHA1 | 60868.2 MH/s |
| 1400 | SHA2-256 | 25242.9 MH/s |
| 1700 | SHA2-512 | 8588.7 MH/s |
| 1000 | NTLM | 272.3 GH/s |
| 22000 | WPA2-PMKID+EAPOL | 3019.9 kH/s |
| 3200 | bcrypt | 131.3 kH/s |

## Полный доступный сырой вывод / Raw output

```text
# Thanks to Shadeform.ai and HotAisle.xyz
# Ubuntu 22.04 + ROCm 6.2.4

##############################
#          HASHCAT           #
##############################
# hashcat from https://github.com/mostwanted002/hashcat.git, branch: hip_rtc_windows_env_implementation
# Tried with -b --benchmark_all, had a GPU memory access violation on PKZIP. 
# Following is the output of `hashcat -b`

hashcat (v6.2.6-854-g3033ed126) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

The device #2 specifically listed was skipped because it is an alias of device #1

HIP API (HIP 6.2.41134)
=======================
* Device #1: AMD Instinct MI300X, 196086/196592 MB, 304MCU

OpenCL API (OpenCL 2.1 AMD-APP (3625.0)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #2: AMD Instinct MI300X, skipped

Benchmark relevant options:
===========================
* --backend-devices-virtual=1
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:   163.7 GH/s (30.88ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........: 60868.2 MH/s (83.50ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........: 25242.9 MH/s (50.23ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  8588.7 MH/s (73.95ms) @ Accel:32 Loops:1024 Thr:64 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:  3019.9 kH/s (51.36ms) @ Accel:128 Loops:256 Thr:64 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:   272.3 GH/s (18.43ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:   154.3 GH/s (32.57ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........:   167.8 GH/s (30.10ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........: 12223.4 MH/s (51.87ms) @ Accel:128 Loops:256 Thr:64 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:  5776.9 MH/s (54.73ms) @ Accel:16 Loops:1024 Thr:64 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........: 58444.2 kH/s (82.14ms) @ Accel:256 Loops:1000 Thr:64 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:   131.3 kH/s (62.40ms) @ Accel:2 Loops:32 Thr:16 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:   943.5 kH/s (13.74ms) @ Accel:2048 Loops:256 Thr:128 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:  2660.4 MH/s (59.64ms) @ Accel:128 Loops:64 Thr:64 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:  2573.8 MH/s (61.66ms) @ Accel:128 Loops:64 Thr:64 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:   543.2 kH/s (97.71ms) @ Accel:128 Loops:512 Thr:64 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:   332.1 kH/s (73.39ms) @ Accel:64 Loops:256 Thr:64 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:  3919.6 kH/s (69.95ms) @ Accel:128 Loops:127 Thr:64 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:  3070.9 kH/s (96.58ms) @ Accel:64 Loops:4096 Thr:64 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:   343.2 kH/s (83.03ms) @ Accel:32 Loops:16384 Thr:64 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:   320.2 kH/s (59.76ms) @ Accel:64 Loops:512 Thr:64 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:  2130.7 kH/s (72.40ms) @ Accel:128 Loops:128 Thr:64 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:   558.7 kH/s (92.77ms) @ Accel:256 Loops:256 Thr:64 Vec:1

-------------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 100099]
-------------------------------------------------------------------

Speed.#1.........:   105.0 kH/s (60.61ms) @ Accel:64 Loops:512 Thr:64 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:    40528 H/s (78.40ms) @ Accel:64 Loops:512 Thr:64 Vec:1

Started: Wed Feb 12 04:55:43 2025
Stopped: Wed Feb 12 04:58:14 2025
```

