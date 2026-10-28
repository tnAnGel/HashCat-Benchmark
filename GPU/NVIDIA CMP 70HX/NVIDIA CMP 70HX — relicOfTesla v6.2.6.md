# NVIDIA CMP 70HX

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA CMP 70HX
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [relicOfTesla](https://hashcat.net/forum/thread-13435.html)
- **Особенности прогона / Run options:** прогон на одной карте из многокарточной системы, выбрана через `--backend-devices=4` (OpenCL-бэкенд); все результаты — `Speed.#4`

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 20799.1 MH/s |
| 100 | SHA1 | 6728.3 MH/s |
| 1400 | SHA2-256 | 2901.4 MH/s |
| 1700 | SHA2-512 | 851.6 MH/s |
| 1000 | NTLM | 35063.1 MH/s |
| 3200 | bcrypt | 29536 H/s |
| 1800 | sha512crypt | 162.5 kH/s |
| 500 | md5crypt | 9029.3 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 340.5 kH/s |
| 7500 | Kerberos AS-REQ (23) | 440.8 MH/s |
| 13100 | Kerberos TGS-REP (23) | 434.1 MH/s |
| 11300 | Bitcoin wallet.dat | 4443 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 252.9 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode
Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.
CUDA API (CUDA 12.4)
====================
* Device #1: NVIDIA CMP 70HX, skipped
* Device #2: NVIDIA CMP 50HX, skipped
* Device #3: NVIDIA CMP 50HX, skipped
OpenCL API (OpenCL 3.0 CUDA 12.4.89) - Platform #1 [NVIDIA Corporation]
=======================================================================
* Device #4: NVIDIA CMP 70HX, 7872/8048 MB (2012 MB allocatable), 30MCU
* Device #5: NVIDIA CMP 50HX, skipped
* Device #6: NVIDIA CMP 50HX, skipped
OpenCL API (OpenCL 2.1 ) - Platform #2 [Intel(R) Corporation]
=============================================================
* Device #7: Intel(R) UHD Graphics 630, skipped
* Device #8: Intel(R) Core(TM) i5-8600 CPU @ 3.10GHz, skipped
Benchmark relevant options:
===========================
* --backend-devices=4
* --optimized-kernel-enable
-------------------
* Hash-Mode 0 (MD5)
-------------------
Speed.#4.........: 20799.1 MH/s (48.16ms) @ Accel:128 Loops:1024 Thr:256 Vec:1
----------------------
* Hash-Mode 100 (SHA1)
----------------------
Speed.#4.........:  6728.3 MH/s (74.51ms) @ Accel:128 Loops:512 Thr:256 Vec:1
---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------
Speed.#4.........:  2901.4 MH/s (86.41ms) @ Accel:128 Loops:256 Thr:256 Vec:1
---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------
Speed.#4.........:  851.6 MH/s (73.58ms) @ Accel:128 Loops:64 Thr:256 Vec:1
-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------
Speed.#4.........:  340.5 kH/s (89.29ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------
Speed.#4.........: 35063.1 MH/s (28.45ms) @ Accel:128 Loops:1024 Thr:256 Vec:1
---------------------
* Hash-Mode 3000 (LM)
---------------------
Speed.#4.........: 20304.4 MH/s (49.29ms) @ Accel:128 Loops:1024 Thr:256 Vec:1
--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------
Speed.#4.........: 21039.2 MH/s (47.60ms) @ Accel:256 Loops:1024 Thr:128 Vec:1
----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------
Speed.#4.........:  1541.8 MH/s (81.31ms) @ Accel:128 Loops:128 Thr:256 Vec:1
--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------
Speed.#4.........:  828.7 MH/s (75.69ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------
Speed.#4.........:  9029.3 kH/s (49.32ms) @ Accel:128 Loops:500 Thr:256 Vec:1
----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------
Speed.#4.........:    29536 H/s (86.04ms) @ Accel:8 Loops:32 Thr:11 Vec:1
--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------
Speed.#4.........:  162.5 kH/s (80.03ms) @ Accel:4096 Loops:256 Thr:64 Vec:1
--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------
Speed.#4.........:  440.8 MH/s (71.18ms) @ Accel:256 Loops:128 Thr:32 Vec:1
-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------
Speed.#4.........:  434.1 MH/s (72.28ms) @ Accel:256 Loops:128 Thr:32 Vec:1
---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------
Speed.#4.........:    58271 H/s (87.55ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------
Speed.#4.........:    33256 H/s (70.61ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------
Speed.#4.........:  415.5 kH/s (68.78ms) @ Accel:512 Loops:63 Thr:32 Vec:1
---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------
Speed.#4.........:  334.4 kH/s (78.24ms) @ Accel:128 Loops:4096 Thr:32 Vec:1
------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------
Speed.#4.........:    51679 H/s (73.85ms) @ Accel:8 Loops:16384 Thr:256 Vec:1
--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------
Speed.#4.........:    36347 H/s (52.61ms) @ Accel:32 Loops:256 Thr:256 Vec:1
--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------
Speed.#4.........:  252.9 kH/s (55.02ms) @ Accel:8 Loops:512 Thr:256 Vec:1
-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------
Speed.#4.........:    42600 H/s (59.95ms) @ Accel:16 Loops:512 Thr:256 Vec:1
----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------
Speed.#4.........:  2281.0 kH/s (41.04ms) @ Accel:64 Loops:124 Thr:256 Vec:1
--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------
Speed.#4.........:    4443 H/s (70.50ms) @ Accel:16 Loops:512 Thr:256 Vec:1
Started: Mon Dec 01 11:36:18 2025
Stopped: Mon Dec 01 11:41:44 2025
```
