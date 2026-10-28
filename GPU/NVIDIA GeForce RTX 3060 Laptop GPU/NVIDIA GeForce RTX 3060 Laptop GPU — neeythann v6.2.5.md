# NVIDIA GeForce RTX 3060 Laptop GPU

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce RTX 3060 Laptop GPU
- **Версия hashcat / Version:** v6.2.5
- **Источник / Source:** [neeythann](https://gist.github.com/neeythann/542b28bbdf167fa76fa613698dfe4f86)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 25013.9 MH/s |
| 100 | SHA1 | 7905.2 MH/s |
| 1400 | SHA2-256 | 3394.6 MH/s |
| 1700 | SHA2-512 | 1183.6 MH/s |
| 1000 | NTLM | 47845.1 MH/s |
| 3200 | bcrypt | 35474 H/s |
| 1800 | sha512crypt | 179.4 kH/s |
| 500 | md5crypt | 10580.0 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 417.4 kH/s |
| 7500 | Kerberos AS-REQ (23) | 588.1 MH/s |
| 13100 | Kerberos TGS-REP (23) | 588.0 MH/s |
| 11300 | Bitcoin wallet.dat | 5512 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 316.5 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.5) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #1: WARNING! Kernel exec timeout is not disabled.
             This may cause "CL_OUT_OF_RESOURCES" or related errors.
             To disable the timeout, see: https://hashcat.net/q/timeoutpatch
nvmlDeviceGetFanSpeed(): Not Supported

CUDA API (CUDA 11.6)
====================
* Device #1: NVIDIA GeForce RTX 3060 Laptop GPU, 5157/6143 MB, 30MCU

OpenCL API (OpenCL 3.0 CUDA 11.6.99) - Platform #1 [NVIDIA Corporation]
=======================================================================
* Device #2: NVIDIA GeForce RTX 3060 Laptop GPU, skipped

OpenCL API (OpenCL 3.0 ) - Platform #2 [Intel(R) Corporation]
=============================================================
* Device #3: Intel(R) UHD Graphics, skipped

Benchmark relevant options:
===========================
* --backend-devices=1
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 25013.9 MH/s (79.63ms) @ Accel:2048 Loops:1024 Thr:32 Vec:8

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  7905.2 MH/s (63.16ms) @ Accel:32 Loops:1024 Thr:512 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  3394.6 MH/s (73.58ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  1183.6 MH/s (52.69ms) @ Accel:64 Loops:1024 Thr:32 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   417.4 kH/s (71.66ms) @ Accel:8 Loops:1024 Thr:512 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 47845.1 MH/s (41.34ms) @ Accel:256 Loops:1024 Thr:256 Vec:8

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........: 25135.4 MH/s (39.44ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 26244.9 MH/s (75.91ms) @ Accel:512 Loops:1024 Thr:128 Vec:2

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  1884.2 MH/s (66.29ms) @ Accel:32 Loops:512 Thr:256 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:  1029.2 MH/s (60.57ms) @ Accel:8 Loops:1024 Thr:256 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........: 10580.0 kH/s (79.40ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    35474 H/s (83.78ms) @ Accel:128 Loops:32 Thr:24 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:   179.4 kH/s (72.14ms) @ Accel:2048 Loops:256 Thr:128 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:   588.1 MH/s (53.00ms) @ Accel:256 Loops:128 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:   588.0 MH/s (53.01ms) @ Accel:256 Loops:128 Thr:32 Vec:1

---------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1) [Iterations: 23999]
---------------------------------------------------------------

Speed.#1.........:    72730 H/s (69.72ms) @ Accel:8 Loops:1024 Thr:512 Vec:1

---------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2) [Iterations: 12899]
---------------------------------------------------------------

Speed.#1.........:    42018 H/s (55.55ms) @ Accel:4 Loops:512 Thr:512 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:   516.2 kH/s (56.77ms) @ Accel:128 Loops:31 Thr:256 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:   420.3 kH/s (69.39ms) @ Accel:32 Loops:4096 Thr:128 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    54343 H/s (69.81ms) @ Accel:8 Loops:16384 Thr:256 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    45349 H/s (84.03ms) @ Accel:32 Loops:256 Thr:512 Vec:1

-----------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit) [Iterations: 1999]
-----------------------------------------------------------------------

Speed.#1.........:   316.5 kH/s (88.39ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    54739 H/s (93.01ms) @ Accel:16 Loops:1024 Thr:256 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  2697.1 kH/s (81.19ms) @ Accel:8 Loops:499 Thr:1024 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:     5512 H/s (60.35ms) @ Accel:4096 Loops:128 Thr:128 Vec:1
```
