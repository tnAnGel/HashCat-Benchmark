# NVIDIA GeForce RTX 4050 Laptop GPU

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce RTX 4050 Laptop GPU (Device #1 — 4050 Laptop, Device #3 — встроенная Intel UHD Graphics)
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [hashcat forum — thread 13412, agrodude, 2025-10-21](https://hashcat.net/forum/thread-13412.html)

> Важно: прогон выполнен с `--workload-profile=1` (низкий профиль нагрузки), поэтому скорости заметно ниже, чем на дефолтном профиле. Цифры в таблице — для **Device #1 (RTX 4050 Laptop GPU)**.

## Ключевые результаты / Highlights (Device #1 — RTX 4050 Laptop GPU, `-w 1`)

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 8278.2 MH/s |
| 100 | SHA1 | 4219.1 MH/s |
| 1400 | SHA2-256 | 1457.1 MH/s |
| 1700 | SHA2-512 | 806.6 MH/s |
| 1000 | NTLM | 7275.7 MH/s |
| 3200 | bcrypt | 18379 H/s |
| 1800 | sha512crypt | 61720 H/s |
| 500 | md5crypt | 885.3 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 340.7 kH/s |
| 7500 | Kerberos AS-REQ (23) | 381.5 MH/s |
| 13100 | Kerberos TGS-REP (23) | 205.1 MH/s |
| 11300 | Bitcoin wallet.dat | 4347 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 228.7 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode
nvmlDeviceGetFanSpeed(): Not Supported
CUDA API (CUDA 12.9)
====================
* Device #1: NVIDIA GeForce RTX 4050 Laptop GPU, 5075/6140 MB, 20MCU
OpenCL API (OpenCL 3.0 CUDA 12.9.76) - Platform #1 [NVIDIA Corporation]
=======================================================================
* Device #2: NVIDIA GeForce RTX 4050 Laptop GPU, skipped
OpenCL API (OpenCL 3.0 ) - Platform #2 [Intel(R) Corporation]
=============================================================
* Device #3: Intel(R) UHD Graphics, 15040/30176 MB (2047 MB allocatable), 64MCU
Benchmark relevant options:
===========================
* --workload-profile=1

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:  8278.2 MH/s (1.09ms) @ Accel:256 Loops:16 Thr:128 Vec:1
Speed.#3.........:  948.7 MH/s (1.93ms) @ Accel:16 Loops:16 Thr:128 Vec:1
Speed.#*.........:  9226.8 MH/s

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  4219.1 MH/s (1.07ms) @ Accel:32 Loops:32 Thr:256 Vec:1
Speed.#3.........:  488.4 MH/s (1.88ms) @ Accel:128 Loops:8 Thr:16 Vec:1
Speed.#*.........:  4707.5 MH/s

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  1457.1 MH/s (0.29ms) @ Accel:64 Loops:16 Thr:32 Vec:1
Speed.#3.........:  253.4 MH/s (1.83ms) @ Accel:32 Loops:4 Thr:64 Vec:1
Speed.#*.........:  1710.5 MH/s

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  806.6 MH/s (1.46ms) @ Accel:16 Loops:16 Thr:256 Vec:1
Speed.#3.........: 24124.5 kH/s (1.10ms) @ Accel:32 Loops:1 Thr:16 Vec:1
Speed.#*.........:  830.8 MH/s

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:  340.7 kH/s (1.74ms) @ Accel:16 Loops:32 Thr:256 Vec:1
Speed.#3.........:    25985 H/s (2.12ms) @ Accel:4 Loops:4 Thr:256 Vec:1
Speed.#*.........:  366.7 kH/s

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:  7275.7 MH/s (0.24ms) @ Accel:256 Loops:16 Thr:32 Vec:1
Speed.#3.........:  1138.7 MH/s (1.53ms) @ Accel:32 Loops:16 Thr:64 Vec:1
Speed.#*.........:  8414.4 MH/s

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........: 17719.9 MH/s (0.95ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#3.........:  409.8 MH/s (81.03ms) @ Accel:1 Loops:1024 Thr:512 Vec:1
Speed.#*.........: 18129.8 MH/s

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........:  9897.4 MH/s (0.89ms) @ Accel:256 Loops:16 Thr:128 Vec:1
Speed.#3.........:  914.8 MH/s (0.92ms) @ Accel:32 Loops:16 Thr:32 Vec:1
Speed.#*.........: 10812.1 MH/s

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  1095.8 MH/s (0.99ms) @ Accel:16 Loops:16 Thr:256 Vec:1
Speed.#3.........:  9134.5 kH/s (3.27ms) @ Accel:8 Loops:1 Thr:64 Vec:1
Speed.#*.........:  1104.9 MH/s

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Kernel minimum runtime larger than default TDR
* Device #3: skipped, due to kernel autotune failure (-4).
Speed.#1.........:  795.3 MH/s (5.85ms) @ Accel:1 Loops:1024 Thr:256 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:  885.3 kH/s (1.13ms) @ Accel:64 Loops:15 Thr:64 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    18379 H/s (1.72ms) @ Accel:1 Loops:4 Thr:24 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:    61720 H/s (1.47ms) @ Accel:256 Loops:64 Thr:32 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:  381.5 MH/s (1.45ms) @ Accel:64 Loops:16 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:  205.1 MH/s (0.26ms) @ Accel:16 Loops:8 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:    57739 H/s (1.73ms) @ Accel:16 Loops:32 Thr:256 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:    31646 H/s (1.44ms) @ Accel:4 Loops:32 Thr:256 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:  373.0 kH/s (1.26ms) @ Accel:16 Loops:7 Thr:256 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:    99375 H/s (1.44ms) @ Accel:16 Loops:32 Thr:256 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    36447 H/s (16.37ms) @ Accel:1 Loops:16384 Thr:512 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    34751 H/s (1.02ms) @ Accel:4 Loops:32 Thr:512 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:  228.7 kH/s (1.10ms) @ Accel:4 Loops:16 Thr:512 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    40704 H/s (1.15ms) @ Accel:8 Loops:64 Thr:128 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  1413.5 kH/s (0.94ms) @ Accel:4 Loops:31 Thr:512 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:    4347 H/s (1.36ms) @ Accel:4 Loops:32 Thr:512 Vec:1

Started: Tue Oct 21 17:25:33 2025
Stopped: Tue Oct 21 17:31:35 2025
```
