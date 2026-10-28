# NVIDIA Jetson AGX Orin (Orin)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA Jetson AGX Orin (Orin)
- **Версия hashcat / Version:** v6.2.5-676-g2e5cc361d
- **Источник / Source:** [Shatatel — gist](https://gist.github.com/Shatatel/227b6a1ae4f430909f18866b97c40d46)

> Встраиваемый модуль, hashcat видит устройство как `Orin` (30535 MB, 16MCU). В gist перед этим прогоном есть прерванный (^C) запуск v6.2.5 — здесь приведён полный прогон.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 9079.2 MH/s |
| 100 | SHA1 | 2989.4 MH/s |
| 1400 | SHA2-256 | 1284.6 MH/s |
| 1700 | SHA2-512 | 434.1 MH/s |
| 1000 | NTLM | 15267.2 MH/s |
| 3200 | bcrypt | 16186 H/s |
| 1800 | sha512crypt | 71581 H/s |
| 500 | md5crypt | 3571.2 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 142.7 kH/s |
| 7500 | Kerberos AS-REQ (23) | 269.5 MH/s |
| 13100 | Kerberos TGS-REP (23) | 263.3 MH/s |
| 11300 | Bitcoin wallet.dat | 1988 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 100.8 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
orin@ubuntu:~/Downloads/hashcat/hashcat-master/hashcat$ ./hashcat -b
hashcat (v6.2.5-676-g2e5cc361d) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

clGetPlatformIDs(): CL_PLATFORM_NOT_FOUND_KHR

CUDA API (CUDA 11.4)
====================
* Device #1: Orin, 24367/30535 MB, 16MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:  9079.2 MH/s (57.98ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  2989.4 MH/s (88.70ms) @ Accel:64 Loops:1024 Thr:256 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  1284.6 MH/s (51.23ms) @ Accel:8 Loops:1024 Thr:512 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:   434.1 MH/s (76.29ms) @ Accel:4 Loops:1024 Thr:512 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   142.7 kH/s (53.32ms) @ Accel:4 Loops:1024 Thr:512 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 15267.2 MH/s (34.07ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:  8988.0 MH/s (58.53ms) @ Accel:256 Loops:1024 Thr:128 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........:  9123.8 MH/s (28.11ms) @ Accel:512 Loops:64 Thr:512 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:   673.3 MH/s (48.78ms) @ Accel:64 Loops:512 Thr:64 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:   363.2 MH/s (45.15ms) @ Accel:32 Loops:1024 Thr:32 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:  3571.2 kH/s (58.65ms) @ Accel:32 Loops:1000 Thr:512 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    16186 H/s (59.09ms) @ Accel:2 Loops:32 Thr:40 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:    71581 H/s (89.74ms) @ Accel:1024 Loops:128 Thr:256 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:   269.5 MH/s (61.43ms) @ Accel:256 Loops:128 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:   263.3 MH/s (78.69ms) @ Accel:640 Loops:64 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:    25347 H/s (52.45ms) @ Accel:4 Loops:1024 Thr:512 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:    14008 H/s (21.92ms) @ Accel:32 Loops:256 Thr:32 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:   183.1 kH/s (84.81ms) @ Accel:128 Loops:31 Thr:256 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:   152.0 kH/s (48.53ms) @ Accel:64 Loops:4096 Thr:32 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    22017 H/s (91.04ms) @ Accel:8 Loops:16384 Thr:256 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    15996 H/s (30.59ms) @ Accel:8 Loops:512 Thr:256 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:   100.8 kH/s (16.43ms) @ Accel:64 Loops:128 Thr:32 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    18861 H/s (71.40ms) @ Accel:16 Loops:256 Thr:512 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:   377.1 kH/s (23.45ms) @ Accel:8 Loops:124 Thr:512 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:     1988 H/s (83.25ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1

Started: Sun Aug 28 15:18:15 2022
Stopped: Sun Aug 28 15:26:40 2022
```
