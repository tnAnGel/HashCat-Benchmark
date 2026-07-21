# AMD Radeon RX 6400

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX 6400
- **Версия hashcat / Version:** v6.2.5-491-g407875fe4
- **Источник / Source:** [TheAlgorythm](https://gist.github.com/TheAlgorythm/0af4fb3b351b5e3199f250c6e2cae57d)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 8847.1 MH/s |
| 100 | SHA1 | 3342.0 MH/s |
| 1400 | SHA2-256 | 1421.4 MH/s |
| 1700 | SHA2-512 | 334.7 MH/s |
| 1000 | NTLM | 14413.5 MH/s |
| 3200 | bcrypt | 9012 H/s |
| 1800 | sha512crypt | 62752 H/s |
| 500 | md5crypt | 3009.5 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 173.7 kH/s |
| 7500 | Kerberos AS-REQ (23) | 162.0 MH/s |
| 13100 | Kerberos TGS-REP (23) | — |
| 11300 | Bitcoin wallet.dat | 1680 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 111.2 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.5-491-g407875fe4) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

OpenCL API (OpenCL 2.1 AMD-APP (3423.0)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #1: , 3968/4080 MB (3468 MB allocatable), 6MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:  8847.1 MH/s (89.47ms) @ Accel:1024 Loops:1024 Thr:128 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  3342.0 MH/s (58.66ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  1421.4 MH/s (69.36ms) @ Accel:128 Loops:1024 Thr:128 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:   334.7 MH/s (73.76ms) @ Accel:64 Loops:512 Thr:128 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   173.7 kH/s (69.08ms) @ Accel:512 Loops:128 Thr:128 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 14413.5 MH/s (54.46ms) @ Accel:1024 Loops:1024 Thr:128 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:  7976.9 MH/s (99.09ms) @ Accel:2048 Loops:1024 Thr:64 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........:  9219.2 MH/s (85.63ms) @ Accel:4096 Loops:1024 Thr:32 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:   599.1 MH/s (82.44ms) @ Accel:512 Loops:512 Thr:32 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

* Device #1: Skipping (hash-mode 1500)
             This is due to a known OpenCL runtime and/or device driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:  3009.5 kH/s (56.02ms) @ Accel:512 Loops:500 Thr:128 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:     9012 H/s (73.72ms) @ Accel:8 Loops:32 Thr:16 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:    62752 H/s (50.78ms) @ Accel:1024 Loops:128 Thr:128 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:   162.0 MH/s (76.39ms) @ Accel:512 Loops:128 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

* Device #1: Skipping (hash-mode 13100)
             This is due to a known OpenCL runtime and/or device driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

* Device #1: Skipping (hash-mode 15300)
             This is due to a known OpenCL runtime and/or device driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:    12916 H/s (73.15ms) @ Accel:64 Loops:256 Thr:128 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:   161.1 kH/s (69.35ms) @ Accel:512 Loops:63 Thr:64 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:   184.3 kH/s (60.81ms) @ Accel:256 Loops:4096 Thr:32 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    27388 H/s (110.05ms) @ Accel:32 Loops:16384 Thr:256 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    17411 H/s (86.72ms) @ Accel:512 Loops:256 Thr:64 Vec:1

-----------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit) [Iterations: 1999]
-----------------------------------------------------------------------

Speed.#1.........:   111.2 kH/s (52.37ms) @ Accel:512 Loops:128 Thr:32 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    14567 H/s (69.06ms) @ Accel:1024 Loops:64 Thr:64 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  1062.0 kH/s (67.81ms) @ Accel:256 Loops:124 Thr:256 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:     1680 H/s (73.43ms) @ Accel:2048 Loops:64 Thr:32 Vec:1

Started: Thu Jun  9 15:47:26 2022
Stopped: Thu Jun  9 15:50:41 2022
```
