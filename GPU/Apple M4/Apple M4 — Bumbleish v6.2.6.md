# Apple M4

- **Вендор / Vendor:** Apple
- **Видеокарта / GPU:** Apple M4 (Mac mini, 10 GPU-ядер)
- **Версия hashcat / Version:** v6.2.6
- **API:** Metal (Metal 367.6); OpenCL-устройство #2 в прогоне пропущено (skipped)
- **Источник / Source:** [Bumbleish, hashcat Forum](https://hashcat.net/forum/thread-12248.html)
- **Особенности прогона / Run options:** `--optimized-kernel-enable` (штатный `-b`)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 5582.5 MH/s |
| 100 | SHA1 | 2441.0 MH/s |
| 1400 | SHA2-256 | 889.7 MH/s |
| 1700 | SHA2-512 | 178.5 MH/s |
| 1000 | NTLM | 9849.3 MH/s |
| 3200 | bcrypt | 8680 H/s |
| 500 | md5crypt | 2544.2 kH/s |
| 1800 | sha512crypt | пропущен (Metal runtime issue) |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 122.4 kH/s |
| 7500 | Kerberos 5 AS-REQ | 69210.4 kH/s |
| 13100 | Kerberos 5 TGS-REP | 70110.0 kH/s |
| 11300 | Bitcoin/Litecoin wallet.dat | 867 H/s |
| 6211 | TrueCrypt RIPEMD160 + XTS 512 | 84342 H/s |

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
* Device #1: Apple M4, 5408/10922 MB, 10MCU

OpenCL API (OpenCL 1.2 (Nov  9 2024 22:11:50)) - Platform #1 [Apple]
====================================================================
* Device #2: Apple M4, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:  5582.5 MH/s (59.36ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  2441.0 MH/s (67.97ms) @ Accel:256 Loops:512 Thr:128 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  889.7 MH/s (93.53ms) @ Accel:1024 Loops:128 Thr:64 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  178.5 MH/s (58.00ms) @ Accel:64 Loops:256 Thr:64 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:  122.4 kH/s (83.07ms) @ Accel:1024 Loops:128 Thr:32 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:  9849.3 MH/s (67.39ms) @ Accel:2048 Loops:1024 Thr:32 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:  1303.5 GH/s (0.00ms) @ Accel:128 Loops:1024 Thr:128 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........:  6219.2 MH/s (53.22ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  415.8 MH/s (49.70ms) @ Accel:512 Loops:128 Thr:32 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:  109.6 MH/s (90.84ms) @ Accel:16 Loops:1024 Thr:64 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:  2544.2 kH/s (58.92ms) @ Accel:512 Loops:1000 Thr:32 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    8680 H/s (69.65ms) @ Accel:8 Loops:32 Thr:8 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

* Device #1: Skipping (hash-mode 1800)
            This is due to a known Metal runtime and/or device driver issue (not a hashcat issue)
            You can use --force to override, but do not report related errors.

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........: 69210.4 kH/s (75.00ms) @ Accel:64 Loops:256 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........: 70110.0 kH/s (74.02ms) @ Accel:64 Loops:256 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:    21448 H/s (80.95ms) @ Accel:256 Loops:128 Thr:128 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:    6313 H/s (63.88ms) @ Accel:256 Loops:32 Thr:64 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:    78435 H/s (60.74ms) @ Accel:128 Loops:63 Thr:64 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:  117.2 kH/s (85.65ms) @ Accel:64 Loops:4096 Thr:64 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    18991 H/s (66.92ms) @ Accel:32 Loops:16384 Thr:64 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    11123 H/s (57.01ms) @ Accel:256 Loops:64 Thr:128 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:    84342 H/s (59.93ms) @ Accel:256 Loops:64 Thr:64 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    17715 H/s (47.74ms) @ Accel:64 Loops:1024 Thr:32 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  681.0 kH/s (44.74ms) @ Accel:128 Loops:124 Thr:128 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:      867 H/s (59.90ms) @ Accel:256 Loops:64 Thr:64 Vec:1

```
