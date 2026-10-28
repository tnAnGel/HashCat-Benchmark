# NVIDIA GeForce GT 720

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce GT 720
- **Версия hashcat / Version:** v6.2.5
- **Источник / Source:** [Gyfer](https://hashcat.net/forum/thread-11467.html)
- **Особенности прогона / Run options:** прогон одной карты из системы с тремя GPU, выбрана через `--backend-devices=3` (CUDA); все результаты — `Speed.#3`

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 401.2 MH/s |
| 100 | SHA1 | 113.3 MH/s |
| 1400 | SHA2-256 | 51236.6 kH/s |
| 1700 | SHA2-512 | 13975.3 kH/s |
| 1000 | NTLM | 644.6 MH/s |
| 3200 | bcrypt | 69 H/s |
| 1800 | sha512crypt | 2483 H/s |
| 500 | md5crypt | 145.5 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 5994 H/s |
| 7500 | Kerberos AS-REQ (23) | 2156.9 kH/s |
| 13100 | Kerberos TGS-REP (23) | 1957.3 kH/s |
| 11300 | Bitcoin wallet.dat | 77 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 3793 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.5) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #3: This hardware has outdated CUDA compute capability (3.5).
            For modern OpenCL performance, upgrade to hardware that supports
            CUDA compute capability version 5.0 (Maxwell) or higher.

CUUDA API (CUDA 11.4)
====================
* Device #1: Quadro P4000, skipped
* Device #2: NVIDIA GeForce GT 730, skipped
* Device #3: NVIDIA GeForce GT 720, 1982/2002 MB, 1MCU

OpenCL API (OpenCL 3.0 CUDA 11.4.364) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #4: Quadro P4000, skipped
* Device #5: NVIDIA GeForce GT 730, skipped
* Device #6: NVIDIA GeForce GT 720, skipped

Benchmark relevant options:
===========================
* --backend-devices=3
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#3.........:  401.2 MH/s (82.63ms) @ Accel:256 Loops:512 Thr:256 Vec:2

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#3.........:  113.3 MH/s (73.29ms) @ Accel:256 Loops:1024 Thr:32 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#3.........: 51236.6 kH/s (80.97ms) @ Accel:64 Loops:128 Thr:512 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#3.........: 13975.3 kH/s (74.23ms) @ Accel:64 Loops:64 Thr:256 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#3.........:    5994 H/s (83.04ms) @ Accel:32 Loops:256 Thr:256 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#3.........:  644.6 MH/s (51.19ms) @ Accel:256 Loops:1024 Thr:128 Vec:4

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#3.........:  221.4 MH/s (74.84ms) @ Accel:128 Loops:1024 Thr:128 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#3.........:  413.3 MH/s (80.25ms) @ Accel:256 Loops:1024 Thr:128 Vec:4

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#3.........: 20288.5 kH/s (50.93ms) @ Accel:2 Loops:1024 Thr:512 Vec:2

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#3.........:  9503.0 kH/s (54.36ms) @ Accel:8 Loops:1024 Thr:64 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#3.........:  145.5 kH/s (87.47ms) @ Accel:128 Loops:1000 Thr:128 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#3.........:      69 H/s (82.33ms) @ Accel:1 Loops:16 Thr:12 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#3.........:    2483 H/s (80.07ms) @ Accel:128 Loops:128 Thr:64 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#3.........:  2156.9 kH/s (60.38ms) @ Accel:128 Loops:32 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#3.........:  1957.3 kH/s (66.56ms) @ Accel:16 Loops:256 Thr:32 Vec:1

---------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1) [Iterations: 23999]
---------------------------------------------------------------

Speed.#3.........:    1012 H/s (82.31ms) @ Accel:8 Loops:1024 Thr:256 Vec:1

---------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2) [Iterations: 12899]
---------------------------------------------------------------

Speed.#3.........:      475 H/s (80.54ms) @ Accel:2 Loops:512 Thr:512 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#3.........:    5875 H/s (82.30ms) @ Accel:32 Loops:31 Thr:512 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#3.........:    6256 H/s (73.90ms) @ Accel:2 Loops:4096 Thr:1024 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#3.........:      703 H/s (87.92ms) @ Accel:32 Loops:16384 Thr:32 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#3.........:      649 H/s (47.61ms) @ Accel:2 Loops:512 Thr:1024 Vec:1

-----------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit) [Iterations: 1999]
-----------------------------------------------------------------------

Speed.#3.........:    3793 H/s (56.48ms) @ Accel:2 Loops:256 Thr:1024 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#3.........:      696 H/s (60.60ms) @ Accel:64 Loops:128 Thr:128 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#3.........:    32046 H/s (94.18ms) @ Accel:4 Loops:499 Thr:1024 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#3.........:      77 H/s (66.90ms) @ Accel:2 Loops:512 Thr:1024 Vec:1

Started: Thu Jun 15 17:22:25 2023
Stopped: Thu Jun 15 17:27:43 2023
```
