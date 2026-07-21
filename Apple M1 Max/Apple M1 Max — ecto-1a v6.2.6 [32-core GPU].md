# Apple M1 Max (32-core GPU)

- **Вендор / Vendor:** Apple
- **Видеокарта / GPU:** Apple M1 Max
- **Конфигурация / Setup:** 32-core GPU
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [ecto-1a](https://ecto-1a.github.io/hashcatmac/)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 13215.7 MH/s |
| 100 | SHA1 | 5405.3 MH/s |
| 1400 | SHA2-256 | 1954.6 MH/s |
| 1700 | SHA2-512 | 395.7 MH/s |
| 1000 | NTLM | 21123.8 MH/s |
| 3200 | bcrypt | 9342 H/s |
| 1800 | sha512crypt | — |
| 500 | md5crypt | 5298.5 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 247.8 kH/s |
| 7500 | Kerberos AS-REQ (23) | 180.1 MH/s |
| 13100 | Kerberos TGS-REP (23) | 180.8 MH/s |
| 11300 | Bitcoin wallet.dat | 1789 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 168.6 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #2: Apple's OpenCL drivers (GPU) are known to be unreliable.
             You have been warned.

METAL API (Metal 343.14)
========================
* Device #1: Apple M1 Max, 10880/21845 MB, 32MCU

OpenCL API (OpenCL 1.2 (Feb 10 2024 00:43:19)) - Platform #1 [Apple]
====================================================================
* Device #2: Apple M1 Max, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 13215.7 MH/s (80.36ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  5405.3 MH/s (48.80ms) @ Accel:256 Loops:1024 Thr:32 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  1954.6 MH/s (67.67ms) @ Accel:512 Loops:256 Thr:32 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:   395.7 MH/s (83.93ms) @ Accel:256 Loops:64 Thr:64 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   247.8 kH/s (65.57ms) @ Accel:512 Loops:128 Thr:32 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 21123.8 MH/s (49.95ms) @ Accel:2048 Loops:512 Thr:32 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:   668.6 MH/s (52.74ms) @ Accel:16 Loops:1024 Thr:128 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 13590.9 MH/s (78.14ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:   915.6 MH/s (72.43ms) @ Accel:64 Loops:256 Thr:128 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........: 18597.5 kH/s (183.61ms) @ Accel:4 Loops:1024 Thr:32 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:  5298.5 kH/s (94.24ms) @ Accel:512 Loops:500 Thr:64 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:     9342 H/s (51.95ms) @ Accel:2 Loops:32 Thr:8 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

* Device #1: Skipping (hash-mode 1800)
             This is due to a known Metal runtime and/or device driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:   180.1 MH/s (92.27ms) @ Accel:256 Loops:64 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:   180.8 MH/s (91.95ms) @ Accel:256 Loops:64 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:    43357 H/s (64.01ms) @ Accel:512 Loops:128 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:     6748 H/s (47.74ms) @ Accel:128 Loops:16 Thr:64 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:    89131 H/s (88.48ms) @ Accel:128 Loops:31 Thr:64 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:   251.7 kH/s (62.38ms) @ Accel:32 Loops:4096 Thr:64 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    32033 H/s (63.45ms) @ Accel:8 Loops:16384 Thr:128 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    24212 H/s (84.02ms) @ Accel:512 Loops:128 Thr:32 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:   168.6 kH/s (47.83ms) @ Accel:64 Loops:128 Thr:64 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    73676 H/s (73.66ms) @ Accel:128 Loops:512 Thr:64 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  1532.7 kH/s (65.67ms) @ Accel:256 Loops:124 Thr:64 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:     1789 H/s (92.88ms) @ Accel:1024 Loops:32 Thr:32 Vec:1

Started: Wed Jun 25 18:22:25 2025
Stopped: Wed Jun 25 18:28:53 2025
```
