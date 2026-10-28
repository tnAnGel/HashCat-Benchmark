# AMD Radeon RX 6800 (OpenCL backend (HIP skipped) — device #2)

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX 6800
- **Конфигурация / Setup:** OpenCL backend (HIP skipped) — device #2
- **Версия hashcat / Version:** v6.2.6-846-g4d412c8e0
- **Источник / Source:** [epixoip](https://gist.github.com/epixoip/99085955a1145ff61ec83512a50421a7)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 42241.8 MH/s |
| 100 | SHA1 | 16414.5 MH/s |
| 1400 | SHA2-256 | 7015.9 MH/s |
| 1700 | SHA2-512 | 1638.0 MH/s |
| 1000 | NTLM | 75808.8 MH/s |
| 3200 | bcrypt | 42646 H/s |
| 1800 | sha512crypt | 292.6 kH/s |
| 500 | md5crypt | 11888.6 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 832.9 kH/s |
| 7500 | Kerberos AS-REQ (23) | 836.8 MH/s |
| 13100 | Kerberos TGS-REP (23) | 807.0 MH/s |
| 11300 | Bitcoin wallet.dat | 8179 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 535.1 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6-846-g4d412c8e0) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

hipMemGetInfo(): 1

HIP API (HIP 5.7.31921)
=======================
* Device #1: AMD Radeon RX 6800, skipped

OpenCL API (OpenCL 2.1 AMD-APP (3590.0)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #2: AMD Radeon RX 6800, 16256/16368 MB (13912 MB allocatable), 30MCU

Benchmark relevant options:
===========================
* --backend-devices-virtual=1
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#2.........: 42241.8 MH/s (23.28ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#2.........: 16414.5 MH/s (60.77ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#2.........:  7015.9 MH/s (71.11ms) @ Accel:64 Loops:1024 Thr:256 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#2.........:  1638.0 MH/s (76.20ms) @ Accel:32 Loops:512 Thr:256 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#2.........:   832.9 kH/s (72.22ms) @ Accel:64 Loops:512 Thr:256 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#2.........: 75808.8 MH/s (12.70ms) @ Accel:256 Loops:1024 Thr:128 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#2.........: 42900.4 MH/s (22.84ms) @ Accel:256 Loops:1024 Thr:128 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#2.........: 48369.9 MH/s (20.28ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#2.........:  2926.1 MH/s (85.36ms) @ Accel:64 Loops:512 Thr:256 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#2.........:  1607.1 MH/s (77.62ms) @ Accel:16 Loops:1024 Thr:256 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#2.........: 11888.6 kH/s (75.71ms) @ Accel:128 Loops:1000 Thr:256 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#2.........:    42646 H/s (86.13ms) @ Accel:32 Loops:8 Thr:16 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#2.........:   292.6 kH/s (88.57ms) @ Accel:2048 Loops:512 Thr:128 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#2.........:   836.8 MH/s (74.61ms) @ Accel:512 Loops:128 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#2.........:   807.0 MH/s (77.39ms) @ Accel:64 Loops:1024 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#2.........:   143.7 kH/s (72.07ms) @ Accel:64 Loops:512 Thr:256 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#2.........:    61672 H/s (78.45ms) @ Accel:128 Loops:128 Thr:128 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#2.........:   773.7 kH/s (73.40ms) @ Accel:128 Loops:63 Thr:256 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#2.........:   842.8 kH/s (67.10ms) @ Accel:32 Loops:4096 Thr:256 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#2.........:   122.1 kH/s (61.62ms) @ Accel:16 Loops:16384 Thr:256 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#2.........:    84181 H/s (90.55ms) @ Accel:64 Loops:512 Thr:256 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#2.........:   535.1 kH/s (55.87ms) @ Accel:128 Loops:128 Thr:128 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#2.........:    70559 H/s (69.44ms) @ Accel:512 Loops:128 Thr:64 Vec:1

-------------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 100099]
-------------------------------------------------------------------

Speed.#2.........:    28060 H/s (89.07ms) @ Accel:64 Loops:512 Thr:256 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#2.........:     8179 H/s (76.17ms) @ Accel:64 Loops:256 Thr:256 Vec:1

Started: Sat Dec  9 19:16:29 2023
Stopped: Sat Dec  9 19:23:20 2023
```
