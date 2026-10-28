# NVIDIA H200

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA H200
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [lepomiz](https://gist.github.com/lepomiz/e2dbb9359a71e2064eddedd0b5724b14)
- **Примечание / Note:** прогон на одиночной H200 (CUDA 12.4, драйвер 550.127.05). Для режима 1000 (NTLM) автор дополнительно прогнал вариант с backend vec 8 — в выводе две строки Speed.#1; в таблице ниже указан результат с настройками по умолчанию. Вывод сокращён автором: отсутствуют строки Started/Stopped.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 120.3 GH/s |
| 100 | SHA1 | 43268.8 MH/s |
| 1400 | SHA2-256 | 16406.0 MH/s |
| 1700 | SHA2-512 | 5423.5 MH/s |
| 1000 | NTLM | 203.5 GH/s |
| 3200 | bcrypt | 352.2 kH/s |
| 1800 | sha512crypt | 869.7 kH/s |
| 500 | md5crypt | 60000.4 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 2186.5 kH/s |
| 7500 | Kerberos AS-REQ (23) | 4379.7 MH/s |
| 13100 | Kerberos TGS-REP (23) | 3754.7 MH/s |
| 11300 | Bitcoin wallet.dat | 24826 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 1475.7 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

nvmlDeviceGetFanSpeed(): Not Supported

CUDA API (CUDA 12.4)
====================
* Device #1: NVIDIA H200, 142546/143071 MB, 132MCU

OpenCL API (OpenCL 3.0 CUDA 12.4.131) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #2: NVIDIA H200, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:   120.3 GH/s (36.68ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........: 43268.8 MH/s (51.06ms) @ Accel:32 Loops:1024 Thr:512 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........: 16406.0 MH/s (67.31ms) @ Accel:64 Loops:256 Thr:512 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  5423.5 MH/s (50.91ms) @ Accel:32 Loops:128 Thr:512 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:  2186.5 kH/s (61.40ms) @ Accel:8 Loops:1024 Thr:512 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:   203.5 GH/s (21.59ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#1.........:   225.1 GH/s (9.72ms) @ Accel:256 Loops:1024 Thr:64 Vec:8

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:   112.2 GH/s (9.76ms) @ Accel:256 Loops:1024 Thr:32 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........:   123.7 GH/s (35.64ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  9622.6 MH/s (57.44ms) @ Accel:16 Loops:1024 Thr:256 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:  4541.2 MH/s (60.84ms) @ Accel:16 Loops:1024 Thr:128 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........: 60000.4 kH/s (64.89ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:   352.2 kH/s (76.49ms) @ Accel:4 Loops:32 Thr:56 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:   869.7 kH/s (59.72ms) @ Accel:256 Loops:1024 Thr:1024 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:  4379.7 MH/s (63.08ms) @ Accel:512 Loops:128 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:  3754.7 MH/s (73.60ms) @ Accel:512 Loops:128 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:   372.1 kH/s (60.38ms) @ Accel:8 Loops:1024 Thr:512 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:   182.5 kH/s (58.66ms) @ Accel:16 Loops:128 Thr:512 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:  2300.8 kH/s (54.85ms) @ Accel:64 Loops:63 Thr:256 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:  2053.4 kH/s (62.92ms) @ Accel:64 Loops:4096 Thr:64 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:   316.6 kH/s (53.21ms) @ Accel:8 Loops:16384 Thr:256 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:   201.1 kH/s (83.82ms) @ Accel:32 Loops:512 Thr:256 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:  1475.7 kH/s (81.22ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:   240.3 kH/s (93.62ms) @ Accel:8 Loops:1024 Thr:512 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........: 12791.3 kH/s (54.28ms) @ Accel:64 Loops:249 Thr:256 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:    24826 H/s (55.57ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1
```
