# AMD Radeon RX 6800M

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX 6800M (Dell G15 Advantage Edition; Device #1 — встроенная APU Radeon Graphics, Device #2 — сама RX 6800M)
- **Версия hashcat / Version:** не указана в источнике / not stated in source
- **Источник / Source:** [hashcat forum — thread 10470, chaos.exe, 2021-11-21](https://hashcat.net/forum/thread-10470.html)

> Примечание: цифры в таблице ниже — для **Device #2 (RX 6800M)**. В полном выводе также присутствует Device #1 (встроенная AMD Radeon Graphics APU) и суммарная строка `Speed.#*`.

## Ключевые результаты / Highlights (Device #2 — RX 6800M)

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 31663.8 MH/s |
| 100 | SHA1 | 12376.2 MH/s |
| 1400 | SHA2-256 | 5226.0 MH/s |
| 1700 | SHA2-512 | 1399.7 MH/s |
| 1000 | NTLM | 50889.7 MH/s |
| 3200 | bcrypt | 28478 H/s |
| 1800 | sha512crypt | 189.3 kH/s |
| 500 | md5crypt | 12555.7 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 616.9 kH/s |
| 7500 | Kerberos AS-REQ (23) | 579.9 MH/s |
| 13100 | Kerberos TGS-REP (23) | 521.1 MH/s |
| 11300 | Bitcoin wallet.dat | 6453 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 395.2 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
OpenCL API (OpenCL 2.1 AMD-APP (3276.6)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #1: AMD Radeon(TM) Graphics, 3072/6235 MB (2432 MB allocatable), 8MCU
* Device #2: AMD Radeon RX 6800M, 12160/12272 MB (10431 MB allocatable), 20MCU
Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:  4767.8 MH/s (55.15ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 31663.8 MH/s (41.60ms) @ Accel:256 Loops:1024 Thr:256 Vec:1
Speed.#*.........: 36431.6 MH/s

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  1837.6 MH/s (71.62ms) @ Accel:256 Loops:512 Thr:128 Vec:1
Speed.#2.........: 12376.2 MH/s (53.32ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 14213.9 MH/s

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  723.3 MH/s (91.22ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  5226.0 MH/s (63.42ms) @ Accel:256 Loops:512 Thr:128 Vec:1
Speed.#*.........:  5949.3 MH/s

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  168.1 MH/s (49.13ms) @ Accel:16 Loops:512 Thr:128 Vec:1
Speed.#2.........:  1399.7 MH/s (59.23ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#*.........:  1567.8 MH/s

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:    89031 H/s (90.12ms) @ Accel:256 Loops:128 Thr:128 Vec:1
Speed.#2.........:  616.9 kH/s (65.67ms) @ Accel:128 Loops:256 Thr:256 Vec:1
Speed.#*.........:  706.0 kH/s

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:  7959.4 MH/s (65.88ms) @ Accel:512 Loops:512 Thr:256 Vec:1
Speed.#2.........: 50889.7 MH/s (25.71ms) @ Accel:512 Loops:1024 Thr:128 Vec:1
Speed.#*.........: 58849.2 MH/s

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:  4436.7 MH/s (59.10ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 30734.3 MH/s (42.72ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 35171.0 MH/s

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........:  4849.4 MH/s (54.13ms) @ Accel:256 Loops:1024 Thr:128 Vec:1
Speed.#2.........: 33712.6 MH/s (39.10ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 38562.0 MH/s

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  349.0 MH/s (95.32ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#2.........:  2079.0 MH/s (79.93ms) @ Accel:128 Loops:256 Thr:256 Vec:1
Speed.#*.........:  2427.9 MH/s

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

* Device #1: Skipping (hash-mode 1500)
            This is due to a known CUDA/HIP/OpenCL runtime/driver issue (not a hashcat issue)
            You can use --force to override, but do not report related errors.
Speed.#2.........:  1118.1 MH/s (73.74ms) @ Accel:32 Loops:1024 Thr:128 Vec:1
Speed.#*.........:  1118.1 MH/s

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:  1844.2 kH/s (62.80ms) @ Accel:512 Loops:500 Thr:64 Vec:1
Speed.#2.........: 12555.7 kH/s (93.98ms) @ Accel:256 Loops:1000 Thr:256 Vec:1
Speed.#*.........: 14399.9 kH/s

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    2587 H/s (94.79ms) @ Accel:32 Loops:32 Thr:8 Vec:1
Speed.#2.........:    28478 H/s (68.27ms) @ Accel:128 Loops:32 Thr:16 Vec:1
Speed.#*.........:    31064 H/s

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:    26253 H/s (58.75ms) @ Accel:128 Loops:512 Thr:128 Vec:1
Speed.#2.........:  189.3 kH/s (67.40ms) @ Accel:512 Loops:1024 Thr:128 Vec:1
Speed.#*.........:  215.6 kH/s

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........: 30794.1 kH/s (67.15ms) @ Accel:8 Loops:1024 Thr:32 Vec:1
Speed.#2.........:  579.9 MH/s (71.37ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.#*.........:  610.7 MH/s

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

* Device #1: Skipping (hash-mode 13100)
            This is due to a known CUDA/HIP/OpenCL runtime/driver issue (not a hashcat issue)
            You can use --force to override, but do not report related errors.
Speed.#2.........:  521.1 MH/s (79.46ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.#*.........:  521.1 MH/s

---------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1) [Iterations: 23999]
---------------------------------------------------------------

* Device #1: Skipping (hash-mode 15300)
            This is due to a known CUDA/HIP/OpenCL runtime/driver issue (not a hashcat issue)
            You can use --force to override, but do not report related errors.
Speed.#2.........:  105.8 kH/s (63.57ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#*.........:  105.8 kH/s

---------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2) [Iterations: 12899]
---------------------------------------------------------------

Speed.#1.........:    3831 H/s (79.85ms) @ Accel:8 Loops:512 Thr:128 Vec:1
Speed.#2.........:    47921 H/s (67.07ms) @ Accel:64 Loops:128 Thr:256 Vec:1
Speed.#*.........:    51751 H/s

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:    46557 H/s (72.93ms) @ Accel:64 Loops:127 Thr:64 Vec:1
Speed.#2.........:  597.7 kH/s (63.12ms) @ Accel:128 Loops:63 Thr:256 Vec:1
Speed.#*.........:  644.2 kH/s

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:    89297 H/s (83.62ms) @ Accel:32 Loops:4096 Thr:128 Vec:1
Speed.#2.........:  536.6 kH/s (69.06ms) @ Accel:32 Loops:4096 Thr:256 Vec:1
Speed.#*.........:  625.9 kH/s

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    8256 H/s (61.25ms) @ Accel:8 Loops:16384 Thr:128 Vec:1
Speed.#2.........:    83837 H/s (59.77ms) @ Accel:16 Loops:16384 Thr:256 Vec:1
Speed.#*.........:    92092 H/s

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    9859 H/s (49.58ms) @ Accel:16 Loops:1024 Thr:128 Vec:1
Speed.#2.........:    66345 H/s (76.20ms) @ Accel:256 Loops:256 Thr:128 Vec:1
Speed.#*.........:    76204 H/s

-----------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit) [Iterations: 1999]
-----------------------------------------------------------------------

Speed.#1.........:    63065 H/s (61.13ms) @ Accel:128 Loops:128 Thr:64 Vec:1
Speed.#2.........:  395.2 kH/s (50.80ms) @ Accel:256 Loops:64 Thr:128 Vec:1
Speed.#*.........:  458.2 kH/s

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    8263 H/s (81.73ms) @ Accel:32 Loops:512 Thr:128 Vec:1
Speed.#2.........:    51325 H/s (65.74ms) @ Accel:1024 Loops:64 Thr:64 Vec:1
Speed.#*.........:    59588 H/s

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  565.7 kH/s (50.90ms) @ Accel:32 Loops:499 Thr:128 Vec:1
Speed.#2.........:  4135.7 kH/s (59.23ms) @ Accel:512 Loops:124 Thr:128 Vec:1
Speed.#*.........:  4701.4 kH/s

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:      859 H/s (48.12ms) @ Accel:512 Loops:128 Thr:128 Vec:1
Speed.#2.........:    6453 H/s (51.46ms) @ Accel:8192 Loops:256 Thr:32 Vec:1
Speed.#*.........:    7312 H/s
```
