# AMD Radeon RX 5600 XT

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX 5600 XT
- **Версия hashcat / Version:** v6.2.6-851-g6716447df
- **Источник / Source:** [banderlog](https://hashcat.net/forum/thread-12245.html)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 20646.9 MH/s |
| 100 | SHA1 | 8176.3 MH/s |
| 1400 | SHA2-256 | 3469.0 MH/s |
| 1700 | SHA2-512 | 879.4 MH/s |
| 1000 | NTLM | 31602.0 MH/s |
| 3200 | bcrypt | 19154 H/s |
| 1800 | sha512crypt | 114.9 kH/s |
| 500 | md5crypt | 4671.5 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 412.9 kH/s |
| 7500 | Kerberos AS-REQ (23) | 356.8 MH/s |
| 13100 | Kerberos TGS-REP (23) | 167.8 MH/s |
| 11300 | Bitcoin wallet.dat | 4101 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 262.7 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6-851-g6716447df) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

HIP API (HIP 5.2.21153)
=======================
* Device #1: AMD Radeon RX 5600 XT, 6128/6128 MB, 18MCU

OpenCL API (OpenCL 2.1 AMD-APP (3452.0)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #2: AMD Radeon RX 5600 XT, skipped

Benchmark relevant options:
===========================
* --backend-devices=1
* --backend-devices-virtual=1
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 20646.9 MH/s (29.16ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  8176.3 MH/s (73.73ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  3469.0 MH/s (86.90ms) @ Accel:1024 Loops:512 Thr:32 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  879.4 MH/s (85.72ms) @ Accel:512 Loops:256 Thr:32 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:  412.9 kH/s (88.40ms) @ Accel:1024 Loops:256 Thr:32 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 31602.0 MH/s (18.16ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........: 17871.9 MH/s (33.65ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 21992.4 MH/s (27.36ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  1265.6 MH/s (59.55ms) @ Accel:512 Loops:256 Thr:32 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:  719.3 MH/s (52.36ms) @ Accel:64 Loops:1024 Thr:32 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:  4671.5 kH/s (60.68ms) @ Accel:1024 Loops:500 Thr:32 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    19154 H/s (57.47ms) @ Accel:16 Loops:8 Thr:16 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:  114.9 kH/s (56.62ms) @ Accel:512 Loops:256 Thr:256 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:  356.8 MH/s (52.81ms) @ Accel:128 Loops:256 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:  167.8 MH/s (55.77ms) @ Accel:32 Loops:512 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:    71053 H/s (88.34ms) @ Accel:1024 Loops:256 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:    31662 H/s (92.17ms) @ Accel:512 Loops:128 Thr:32 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:  394.6 kH/s (73.85ms) @ Accel:256 Loops:255 Thr:32 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:  423.3 kH/s (79.22ms) @ Accel:256 Loops:4096 Thr:32 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    47690 H/s (96.40ms) @ Accel:128 Loops:16384 Thr:32 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    43921 H/s (52.30ms) @ Accel:512 Loops:256 Thr:32 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:  262.7 kH/s (69.21ms) @ Accel:512 Loops:128 Thr:32 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    56028 H/s (54.76ms) @ Accel:512 Loops:256 Thr:32 Vec:1

-------------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 100099]
-------------------------------------------------------------------

Speed.#1.........:    14318 H/s (52.59ms) @ Accel:256 Loops:512 Thr:32 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:    4101 H/s (91.69ms) @ Accel:512 Loops:256 Thr:32 Vec:1

Started: Sat Nov 30 12:28:06 2024
Stopped: Sat Nov 30 12:34:17 2024
```
