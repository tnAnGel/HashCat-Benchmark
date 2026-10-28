# AMD Radeon RX 9070 XT

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX 9070 XT
- **Версия hashcat / Version:** v6.2.6-813-g686bc227c
- **Источник / Source:** [mi7chy](https://hashcat.net/forum/thread-12521.html)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 52565.5 MH/s |
| 100 | SHA1 | 21777.5 MH/s |
| 1400 | SHA2-256 | 9307.2 MH/s |
| 1700 | SHA2-512 | 2114.2 MH/s |
| 1000 | NTLM | 92429.4 MH/s |
| 3200 | bcrypt | 68810 H/s |
| 1800 | sha512crypt | 391.7 kH/s |
| 500 | md5crypt | 22144.5 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 1117.3 kH/s |
| 7500 | Kerberos AS-REQ (23) | 1224.2 MH/s |
| 13100 | Kerberos TGS-REP (23) | 1159.7 MH/s |
| 11300 | Bitcoin wallet.dat | 10556 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 727.7 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6-813-g686bc227c) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

Support for HIPRTC was dropped by AMD Adrenalin Edition 22.7.1 and later.
This is not a hashcat problem.

Please install the AMD HIP SDK

OpenCL API (OpenCL 2.1 AMD-APP (3640.0)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #1: AMD Radeon RX 9070 XT, 16192/16304 MB (13858 MB allocatable), 32MCU

Benchmark relevant options:
===========================
* --backend-devices-virtual=1
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 52565.5 MH/s (19.65ms) @ Accel:256 Loops:1024 Thr:128 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........: 21777.5 MH/s (48.49ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  9307.2 MH/s (56.88ms) @ Accel:64 Loops:1024 Thr:256 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  2114.2 MH/s (62.67ms) @ Accel:64 Loops:256 Thr:256 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:  1117.3 kH/s (57.48ms) @ Accel:64 Loops:512 Thr:256 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 92429.4 MH/s (10.83ms) @ Accel:256 Loops:1024 Thr:128 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........: 53134.6 MH/s (19.31ms) @ Accel:256 Loops:1024 Thr:128 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 59578.7 MH/s (17.21ms) @ Accel:256 Loops:1024 Thr:128 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  3911.3 MH/s (67.84ms) @ Accel:256 Loops:256 Thr:128 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:  1974.4 MH/s (67.01ms) @ Accel:16 Loops:1024 Thr:256 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........: 22144.5 kH/s (41.67ms) @ Accel:256 Loops:1000 Thr:128 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    68810 H/s (55.51ms) @ Accel:16 Loops:16 Thr:16 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:  391.7 kH/s (65.76ms) @ Accel:4096 Loops:512 Thr:64 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:  1224.2 MH/s (54.04ms) @ Accel:512 Loops:128 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:  1159.7 MH/s (57.10ms) @ Accel:512 Loops:128 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:  193.2 kH/s (55.75ms) @ Accel:32 Loops:1024 Thr:256 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:    81786 H/s (62.91ms) @ Accel:512 Loops:128 Thr:32 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:  1018.8 kH/s (59.25ms) @ Accel:256 Loops:63 Thr:128 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:  1164.2 kH/s (52.29ms) @ Accel:32 Loops:4096 Thr:256 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:  167.6 kH/s (96.68ms) @ Accel:32 Loops:16384 Thr:256 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:  113.8 kH/s (69.02ms) @ Accel:32 Loops:1024 Thr:256 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:  727.7 kH/s (86.84ms) @ Accel:32 Loops:512 Thr:256 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:  111.4 kH/s (48.41ms) @ Accel:512 Loops:128 Thr:64 Vec:1

-------------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 100099]
-------------------------------------------------------------------

Speed.#1.........:    37321 H/s (71.23ms) @ Accel:32 Loops:1024 Thr:256 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:    10556 H/s (62.76ms) @ Accel:128 Loops:128 Thr:256 Vec:1

Started: Thu Mar 06 14:55:44 2025
Stopped: Thu Mar 06 14:59:03 2025
```
