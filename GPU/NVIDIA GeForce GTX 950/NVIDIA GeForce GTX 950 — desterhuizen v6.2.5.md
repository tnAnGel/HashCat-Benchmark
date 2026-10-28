# NVIDIA GeForce GTX 950

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce GTX 950
- **Версия hashcat / Version:** v6.2.5
- **Источник / Source:** [desterhuizen](https://gist.github.com/desterhuizen/010addc5b07e394f49e7b960796e51e1)
- **Примечание / Note:** Прогон многокарточный (`hashcat -b -O`): Device #1 — RTX 4060, **Device #2 — GTX 950**. Ниже в таблице приведены строки `Speed.#2` (GTX 950). Полный вывод сохранён как есть.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 5835.1 MH/s |
| 100 | SHA1 | 1990.9 MH/s |
| 1400 | SHA2-256 | 712.1 MH/s |
| 1700 | SHA2-512 | 241.2 MH/s |
| 1000 | NTLM | 10156.3 MH/s |
| 3200 | bcrypt | 4396 H/s |
| 1800 | sha512crypt | 34616 H/s |
| 500 | md5crypt | 2179.3 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 101.5 kH/s |
| 7500 | Kerberos AS-REQ (23) | 87566.6 kH/s |
| 13100 | Kerberos TGS-REP (23) | 87144.7 kH/s |
| 11300 | Bitcoin wallet.dat | 1096 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 64468 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat -b -O
hashcat (v6.2.5) starting in benchmark mode
CUDA API (CUDA 12.6)
====================
* Device #1: NVIDIA GeForce RTX 4060, 7706/7835 MB, 24MCU
* Device #2: NVIDIA GeForce GTX 950, 1950/1989 MB, 6MCU

OpenCL API (OpenCL 3.0 CUDA 12.6.65) - Platform #1 [NVIDIA Corporation]
=======================================================================
* Device #3: NVIDIA GeForce RTX 4060, skipped
* Device #4: NVIDIA GeForce GTX 950, skipped

OpenCL API (OpenCL 3.0 PoCL 5.0+debian  Linux, None+Asserts, RELOC, SPIR, LLVM 16.0.6, SLEEF, DISTRO, POCL_DEBUG) - Platform #2 [The pocl project]
==================================================================================================================================================
* Device #5: cpu-skylake-avx512-AMD Ryzen 9 7950X 16-Core Processor, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 29646.4 MH/s (53.74ms) @ Accel:128 Loops:1024 Thr:512 Vec:1
Speed.#2.........:  5835.1 MH/s (68.33ms) @ Accel:128 Loops:1024 Thr:512 Vec:8
Speed.#*.........: 35481.5 MH/s

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  9480.7 MH/s (84.29ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#2.........:  1990.9 MH/s (50.12ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#*.........: 11471.6 MH/s

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  4108.8 MH/s (48.49ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#2.........:   712.1 MH/s (70.13ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#*.........:  4820.9 MH/s

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  1396.4 MH/s (71.50ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#2.........:   241.2 MH/s (51.74ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#*.........:  1637.6 MH/s

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   487.9 kH/s (49.69ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#2.........:   101.5 kH/s (58.02ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#*.........:   589.5 kH/s

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 50289.9 MH/s (63.31ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1
Speed.#2.........: 10156.3 MH/s (78.40ms) @ Accel:256 Loops:1024 Thr:512 Vec:8
Speed.#*.........: 60446.3 MH/s

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........: 28711.0 MH/s (27.54ms) @ Accel:128 Loops:1024 Thr:256 Vec:1
Speed.#2.........:  5409.0 MH/s (73.73ms) @ Accel:2048 Loops:1024 Thr:32 Vec:1
Speed.#*.........: 34120.0 MH/s

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 30544.4 MH/s (52.04ms) @ Accel:256 Loops:512 Thr:512 Vec:1
Speed.#2.........:  5399.2 MH/s (73.86ms) @ Accel:64 Loops:1024 Thr:1024 Vec:2
Speed.#*.........: 35943.6 MH/s

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  2197.7 MH/s (90.97ms) @ Accel:16 Loops:1024 Thr:512 Vec:1
Speed.#2.........:   423.2 MH/s (58.99ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1
Speed.#*.........:  2620.9 MH/s

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:  1167.7 MH/s (85.54ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#2.........:   213.5 MH/s (58.46ms) @ Accel:64 Loops:1024 Thr:32 Vec:1
Speed.#*.........:  1381.3 MH/s

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........: 12378.5 kH/s (56.28ms) @ Accel:64 Loops:1000 Thr:512 Vec:1
Speed.#2.........:  2179.3 kH/s (78.39ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1
Speed.#*.........: 14557.8 kH/s

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    40503 H/s (73.00ms) @ Accel:128 Loops:32 Thr:24 Vec:1
Speed.#2.........:     4396 H/s (84.40ms) @ Accel:32 Loops:32 Thr:12 Vec:1
Speed.#*.........:    44899 H/s

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:   217.9 kH/s (58.55ms) @ Accel:256 Loops:1024 Thr:256 Vec:1
Speed.#2.........:    34616 H/s (46.26ms) @ Accel:512 Loops:512 Thr:32 Vec:1
Speed.#*.........:   252.5 kH/s

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:   668.4 MH/s (74.87ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.#2.........: 87566.6 kH/s (71.44ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#*.........:   756.0 MH/s

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:   667.0 MH/s (75.01ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.#2.........: 87144.7 kH/s (71.79ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#*.........:   754.1 MH/s

---------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1) [Iterations: 23999]
---------------------------------------------------------------

Speed.#1.........:    83216 H/s (48.76ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#2.........:    17654 H/s (57.23ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#*.........:   100.9 kH/s

---------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2) [Iterations: 12899]
---------------------------------------------------------------

Speed.#1.........:    47204 H/s (78.61ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#2.........:     8770 H/s (53.45ms) @ Accel:4 Loops:512 Thr:512 Vec:1
Speed.#*.........:    55974 H/s

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:   588.0 kH/s (76.96ms) @ Accel:128 Loops:63 Thr:256 Vec:1
Speed.#2.........:   107.2 kH/s (54.68ms) @ Accel:64 Loops:31 Thr:512 Vec:1
Speed.#*.........:   695.2 kH/s

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:   524.0 kH/s (89.80ms) @ Accel:32 Loops:4096 Thr:256 Vec:1
Speed.#2.........:    83731 H/s (71.86ms) @ Accel:32 Loops:4096 Thr:128 Vec:1
Speed.#*.........:   607.8 kH/s

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    72136 H/s (83.87ms) @ Accel:16 Loops:16384 Thr:256 Vec:1
Speed.#2.........:    13610 H/s (55.92ms) @ Accel:4 Loops:16384 Thr:512 Vec:1
Speed.#*.........:    85745 H/s

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    51683 H/s (57.27ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#2.........:     8967 H/s (82.47ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1
Speed.#*.........:    60650 H/s

-----------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit) [Iterations: 1999]
-----------------------------------------------------------------------

Speed.#1.........:   373.1 kH/s (60.83ms) @ Accel:4 Loops:512 Thr:1024 Vec:1
Speed.#2.........:    64468 H/s (87.47ms) @ Accel:4 Loops:512 Thr:1024 Vec:1
Speed.#*.........:   437.6 kH/s

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    60697 H/s (66.84ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#2.........:     7995 H/s (63.71ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#*.........:    68691 H/s

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  3236.8 kH/s (57.33ms) @ Accel:16 Loops:499 Thr:512 Vec:1
Speed.#2.........:   519.8 kH/s (82.82ms) @ Accel:8 Loops:499 Thr:1024 Vec:1
Speed.#*.........:  3756.6 kH/s

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:     6162 H/s (54.01ms) @ Accel:256 Loops:1024 Thr:256 Vec:1
Speed.#2.........:     1096 H/s (75.71ms) @ Accel:256 Loops:64 Thr:1024 Vec:1
Speed.#*.........:     7257 H/s

Started: Sun Jul  6 08:57:05 2025
Stopped: Sun Jul  6 08:59:46 2025```
