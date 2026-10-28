# AMD Radeon RX 7900 XT

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX 7900 XT
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [gartnera](https://gist.github.com/gartnera/4b9dca45cb6be647dbb12e25c2b645db)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 61748.3 MH/s |
| 100 | SHA1 | 24809.5 MH/s |
| 1400 | SHA2-256 | 10583.4 MH/s |
| 1700 | SHA2-512 | 2081.4 MH/s |
| 1000 | NTLM | 97751.9 MH/s |
| 3200 | bcrypt | 83426 H/s |
| 1800 | sha512crypt | 327.1 kH/s |
| 500 | md5crypt | 22083.9 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 1242.2 kH/s |
| 7500 | Kerberos AS-REQ (23) | 1387.7 MH/s |
| 13100 | Kerberos TGS-REP (23) | 856.3 MH/s |
| 11300 | Bitcoin wallet.dat | 9613 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 792.3 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

HIP API (HIP 5.4.22802)
=======================
* Device #1: Radeon RX 7900 XT, 20464/20464 MB, 42MCU
* Device #2: , skipped

OpenCL API (OpenCL 2.1 AMD-APP (3513.0)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #3: Radeon RX 7900 XT, skipped
* Device #4: , skipped

Benchmark relevant options:
===========================
* --backend-devices=1
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 61748.3 MH/s (22.69ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........: 24809.5 MH/s (56.55ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........: 10583.4 MH/s (66.47ms) @ Accel:512 Loops:1024 Thr:32 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  2081.4 MH/s (84.41ms) @ Accel:256 Loops:512 Thr:32 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:  1242.2 kH/s (68.91ms) @ Accel:1024 Loops:256 Thr:32 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 97751.9 MH/s (14.26ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........: 62701.4 MH/s (22.37ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 63791.0 MH/s (21.98ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  4243.8 MH/s (82.89ms) @ Accel:1024 Loops:256 Thr:32 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:  2248.8 MH/s (77.85ms) @ Accel:128 Loops:1024 Thr:32 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........: 22083.9 kH/s (58.82ms) @ Accel:1024 Loops:1000 Thr:32 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    83426 H/s (62.07ms) @ Accel:32 Loops:8 Thr:16 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:   327.1 kH/s (79.12ms) @ Accel:8192 Loops:512 Thr:32 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:  1387.7 MH/s (63.25ms) @ Accel:512 Loops:128 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:   856.3 MH/s (51.18ms) @ Accel:256 Loops:128 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:   216.4 kH/s (67.70ms) @ Accel:1024 Loops:256 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:    74127 H/s (91.74ms) @ Accel:512 Loops:128 Thr:32 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:   945.9 kH/s (72.22ms) @ Accel:256 Loops:255 Thr:32 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:  1198.7 kH/s (66.14ms) @ Accel:256 Loops:4096 Thr:32 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:   173.6 kH/s (61.78ms) @ Accel:128 Loops:16384 Thr:32 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:   138.0 kH/s (77.65ms) @ Accel:1024 Loops:256 Thr:32 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:   792.3 kH/s (53.17ms) @ Accel:64 Loops:1024 Thr:32 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:   209.2 kH/s (68.38ms) @ Accel:1024 Loops:256 Thr:32 Vec:1

-------------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 100099]
-------------------------------------------------------------------

Speed.#1.........:    44953 H/s (78.20ms) @ Accel:512 Loops:512 Thr:32 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:     9613 H/s (91.27ms) @ Accel:512 Loops:256 Thr:32 Vec:1

Started: Thu Dec 15 12:16:44 2022
Stopped: Thu Dec 15 12:19:37 2022
```
