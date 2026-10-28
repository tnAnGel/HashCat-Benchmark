# AMD Radeon RX 6650 XT

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX 6650 XT
- **Версия hashcat / Version:** v6.2.5
- **Источник / Source:** [Pepino](https://hashcat.net/forum/thread-10919.html)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 27980.6 MH/s |
| 100 | SHA1 | 11040.3 MH/s |
| 1400 | SHA2-256 | 4658.4 MH/s |
| 1700 | SHA2-512 | 1254.0 MH/s |
| 1000 | NTLM | 45114.5 MH/s |
| 3200 | bcrypt | 31678 H/s |
| 1800 | sha512crypt | 202.0 kH/s |
| 500 | md5crypt | 5559.7 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 547.6 kH/s |
| 7500 | Kerberos AS-REQ (23) | 514.8 MH/s |
| 13100 | Kerberos TGS-REP (23) | 465.1 MH/s |
| 11300 | Bitcoin wallet.dat | 5713 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 241.1 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.5) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

hiprtcAddNameExpression is missing from HIPRTC shared library.

OpenCL API (OpenCL 2.1 AMD-APP (3444.0)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #1: AMD Radeon RX 6650 XT, 8064/8176 MB (6732 MB allocatable), 16MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 27980.6 MH/s (38.12ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........: 11040.3 MH/s (96.86ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  4658.4 MH/s (57.34ms) @ Accel:64 Loops:1024 Thr:256 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  1254.0 MH/s (53.16ms) @ Accel:16 Loops:1024 Thr:256 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:  547.6 kH/s (58.43ms) @ Accel:64 Loops:512 Thr:256 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 45114.5 MH/s (23.51ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........: 27474.5 MH/s (38.78ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 30336.2 MH/s (35.09ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  1847.4 MH/s (72.29ms) @ Accel:1024 Loops:256 Thr:32 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:  995.5 MH/s (67.05ms) @ Accel:16 Loops:1024 Thr:256 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:  5559.7 kH/s (85.41ms) @ Accel:128 Loops:1000 Thr:256 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    31678 H/s (62.17ms) @ Accel:128 Loops:32 Thr:16 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:  202.0 kH/s (64.16ms) @ Accel:2048 Loops:256 Thr:128 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:  514.8 MH/s (64.86ms) @ Accel:512 Loops:128 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:  465.1 MH/s (71.90ms) @ Accel:64 Loops:1024 Thr:32 Vec:1

---------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1) [Iterations: 23999]
---------------------------------------------------------------

Speed.#1.........:    94411 H/s (58.92ms) @ Accel:256 Loops:256 Thr:128 Vec:1

---------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2) [Iterations: 12899]
---------------------------------------------------------------

Speed.#1.........:    41279 H/s (60.25ms) @ Accel:16 Loops:512 Thr:256 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:  500.8 kH/s (48.87ms) @ Accel:32 Loops:255 Thr:256 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:  562.3 kH/s (53.84ms) @ Accel:32 Loops:4096 Thr:256 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    82733 H/s (97.96ms) @ Accel:64 Loops:16384 Thr:128 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    57176 H/s (71.14ms) @ Accel:128 Loops:256 Thr:256 Vec:1

-----------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit) [Iterations: 1999]
-----------------------------------------------------------------------

Speed.#1.........:  241.1 kH/s (92.86ms) @ Accel:128 Loops:128 Thr:256 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    46307 H/s (58.68ms) @ Accel:1024 Loops:64 Thr:64 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  3437.3 kH/s (45.89ms) @ Accel:128 Loops:249 Thr:256 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:    5713 H/s (58.42ms) @ Accel:512 Loops:512 Thr:256 Vec:1

Started: Mon Aug 01 11:01:34 2022
Stopped: Mon Aug 01 11:06:19 2022
```
