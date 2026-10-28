# AMD Radeon RX 460

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX 460
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [linux](https://hashcat.net/forum/thread-13637.html)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 4200.5 MH/s |
| 100 | SHA1 | 1343.8 MH/s |
| 1400 | SHA2-256 | 573.0 MH/s |
| 1700 | SHA2-512 | 143.1 MH/s |
| 1000 | NTLM | 6640.0 MH/s |
| 3200 | bcrypt | 2696 H/s |
| 1800 | sha512crypt | 21933 H/s |
| 500 | md5crypt | 1508.5 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 67337 H/s |
| 7500 | Kerberos AS-REQ (23) | 31490.8 kH/s |
| 13100 | Kerberos TGS-REP (23) | 16203.7 kH/s |
| 11300 | Bitcoin wallet.dat | 722 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 47091 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

/sys/bus/pci/devices/0000:01:00.0/hwmon/hwmon1/pwm1: No such file or directory

OpenCL API (OpenCL 2.1 AMD-APP (3180.7)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #1: AMD Radeon (TM) RX 460 Graphics, 3968/4082 MB (3263 MB allocatable), 14MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:  4200.5 MH/s (54.68ms) @ Accel:512 Loops:512 Thr:64 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  1343.8 MH/s (86.13ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  573.0 MH/s (50.23ms) @ Accel:16 Loops:1024 Thr:128 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  143.1 MH/s (50.27ms) @ Accel:16 Loops:256 Thr:128 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:    67337 H/s (50.58ms) @ Accel:64 Loops:256 Thr:64 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:  6640.0 MH/s (69.38ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:  4024.6 MH/s (57.00ms) @ Accel:128 Loops:1024 Thr:128 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........:  3778.3 MH/s (60.94ms) @ Accel:128 Loops:1024 Thr:128 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  286.3 MH/s (50.10ms) @ Accel:4 Loops:1024 Thr:256 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:  155.9 MH/s (92.55ms) @ Accel:4 Loops:1024 Thr:256 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:  1508.5 kH/s (64.79ms) @ Accel:512 Loops:250 Thr:64 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    2696 H/s (55.31ms) @ Accel:2 Loops:32 Thr:8 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:    21933 H/s (73.08ms) @ Accel:512 Loops:128 Thr:128 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........: 31490.8 kH/s (57.41ms) @ Accel:32 Loops:128 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........: 16203.7 kH/s (55.91ms) @ Accel:4 Loops:512 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:    12119 H/s (49.45ms) @ Accel:64 Loops:128 Thr:128 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:    4037 H/s (66.29ms) @ Accel:4 Loops:512 Thr:128 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:    39983 H/s (46.35ms) @ Accel:4 Loops:511 Thr:128 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:    63369 H/s (107.30ms) @ Accel:8 Loops:4096 Thr:256 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    8655 H/s (101.54ms) @ Accel:16 Loops:16384 Thr:64 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    7249 H/s (58.52ms) @ Accel:8 Loops:1024 Thr:128 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:    47091 H/s (65.42ms) @ Accel:4 Loops:512 Thr:256 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    14653 H/s (79.77ms) @ Accel:16 Loops:1024 Thr:128 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  363.3 kH/s (39.27ms) @ Accel:64 Loops:249 Thr:64 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:      722 H/s (49.74ms) @ Accel:256 Loops:32 Thr:64 Vec:1

Started: Sun Jun 21 17:46:09 2026
Stopped: Sun Jun 21 17:50:53 2026
```
