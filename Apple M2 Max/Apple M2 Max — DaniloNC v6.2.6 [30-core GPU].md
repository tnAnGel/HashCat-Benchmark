# Apple M2 Max (30-core GPU)

- **Вендор / Vendor:** Apple
- **Видеокарта / GPU:** Apple M2 Max
- **Конфигурация / Setup:** 30-core GPU
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [DaniloNC](https://gist.github.com/DaniloNC/015fbb2cd74adbe39b566c7e6251ffc6)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 12936.1 MH/s |
| 100 | SHA1 | 5496.9 MH/s |
| 1400 | SHA2-256 | 1988.7 MH/s |
| 1700 | SHA2-512 | 405.5 MH/s |
| 1000 | NTLM | 22391.7 MH/s |
| 3200 | bcrypt | 8219 H/s |
| 1800 | sha512crypt | — |
| 500 | md5crypt | 4989.3 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 246.1 kH/s |
| 7500 | Kerberos AS-REQ (23) | 113.6 MH/s |
| 13100 | Kerberos TGS-REP (23) | 165.4 MH/s |
| 11300 | Bitcoin wallet.dat | 1889 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 141.5 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #2: Apple's OpenCL drivers (GPU) are known to be unreliable.
             You have been warned.

METAL API (Metal 367.6)
=======================
* Device #1: Apple M2 Max, 10880/21845 MB, 30MCU

OpenCL API (OpenCL 1.2 (Dec 13 2024 23:09:21)) - Platform #1 [Apple]
====================================================================
* Device #2: Apple M2 Max, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 12936.1 MH/s (76.95ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  5496.9 MH/s (90.81ms) @ Accel:512 Loops:1024 Thr:32 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  1988.7 MH/s (62.53ms) @ Accel:256 Loops:256 Thr:64 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:   405.5 MH/s (76.76ms) @ Accel:256 Loops:64 Thr:64 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   246.1 kH/s (61.66ms) @ Accel:512 Loops:128 Thr:32 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 22391.7 MH/s (89.16ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:  1690.7 MH/s (71.45ms) @ Accel:128 Loops:1024 Thr:32 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 14219.2 MH/s (70.05ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:   953.7 MH/s (65.25ms) @ Accel:256 Loops:128 Thr:64 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........: 31753.6 kH/s (121.16ms) @ Accel:4 Loops:1024 Thr:32 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:  4989.3 kH/s (87.68ms) @ Accel:256 Loops:1000 Thr:64 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:     8219 H/s (56.65ms) @ Accel:16 Loops:4 Thr:8 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

* Device #1: Skipping (hash-mode 1800)
             This is due to a known Metal runtime and/or device driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:   113.6 MH/s (137.65ms) @ Accel:16 Loops:1024 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:   165.4 MH/s (46.82ms) @ Accel:8 Loops:1024 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:    43379 H/s (59.96ms) @ Accel:512 Loops:128 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:     7385 H/s (79.42ms) @ Accel:16 Loops:512 Thr:32 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:   128.7 kH/s (57.16ms) @ Accel:64 Loops:31 Thr:128 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:   241.7 kH/s (60.61ms) @ Accel:64 Loops:4096 Thr:32 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    29504 H/s (64.46ms) @ Accel:32 Loops:16384 Thr:32 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    24488 H/s (77.83ms) @ Accel:512 Loops:128 Thr:32 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:   141.5 kH/s (50.98ms) @ Accel:8 Loops:1024 Thr:64 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    71559 H/s (71.14ms) @ Accel:256 Loops:256 Thr:64 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  1505.0 kH/s (60.96ms) @ Accel:512 Loops:124 Thr:32 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:     1889 H/s (82.60ms) @ Accel:256 Loops:64 Thr:64 Vec:1

Started: Wed Mar 19 14:52:58 2025
```
