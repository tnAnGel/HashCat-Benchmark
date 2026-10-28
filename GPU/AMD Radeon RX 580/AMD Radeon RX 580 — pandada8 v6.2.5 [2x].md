# AMD Radeon RX 580 (2x)

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon RX 580
- **Конфигурация / Setup:** 2x
- **Версия hashcat / Version:** v6.2.5
- **Источник / Source:** [pandada8](https://gist.github.com/pandada8/6608b3c9969bc85c0e1f2953f9853725)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 11066.1 MH/s |
| 100 | SHA1 | 3633.2 MH/s |
| 1400 | SHA2-256 | 1460.2 MH/s |
| 1700 | SHA2-512 | 304.6 MH/s |
| 1000 | NTLM | 18396.6 MH/s |
| 3200 | bcrypt | 8963 H/s |
| 1800 | sha512crypt | 45592 H/s |
| 500 | md5crypt | 672.2 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 118.6 kH/s |
| 7500 | Kerberos AS-REQ (23) | 84230.1 kH/s |
| 13100 | Kerberos TGS-REP (23) | 0 H/s |
| 11300 | Bitcoin wallet.dat | 1882 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 73538 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.5) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

hipDeviceGetAttribute(): 1

hipDeviceGetAttribute(): 1

HIP API (HIP 4.4)
=================
* Device #1: Radeon RX 580 Series, skipped
* Device #2: Radeon RX 580 Series, skipped

OpenCL API (OpenCL 2.1 AMD-APP (3354.13)) - Platform #1 [Advanced Micro Devices, Inc.]
======================================================================================
* Device #3: Radeon RX 580 Series, 8064/8192 MB (6745 MB allocatable), 36MCU
* Device #4: Radeon RX 580 Series, 8064/8192 MB (6745 MB allocatable), 36MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#3.........:  5947.1 MH/s (42.21ms) @ Accel:256 Loops:256 Thr:128 Vec:1
Speed.#4.........:  5119.0 MH/s (45.75ms) @ Accel:256 Loops:256 Thr:128 Vec:1
Speed.#*.........: 11066.1 MH/s

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#3.........:  2088.8 MH/s (61.82ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#4.........:  1544.3 MH/s (87.98ms) @ Accel:512 Loops:128 Thr:64 Vec:1
Speed.#*.........:  3633.2 MH/s

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#3.........:   843.3 MH/s (79.58ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#4.........:   616.9 MH/s (109.86ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  1460.2 MH/s

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#3.........:   153.5 MH/s (56.41ms) @ Accel:8 Loops:512 Thr:64 Vec:1
Speed.#4.........:   151.1 MH/s (58.59ms) @ Accel:8 Loops:512 Thr:64 Vec:1
Speed.#*.........:   304.6 MH/s

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#3.........:    65018 H/s (73.17ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#4.........:    53550 H/s (87.52ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   118.6 kH/s

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#3.........:  9703.7 MH/s (20.63ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#4.........:  8692.9 MH/s (21.15ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#*.........: 18396.6 MH/s

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#3.........:  5583.3 MH/s (38.67ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#4.........:  4236.3 MH/s (52.55ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#*.........:  9819.6 MH/s

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#3.........:  5480.7 MH/s (27.37ms) @ Accel:256 Loops:128 Thr:128 Vec:1
Speed.#4.........:  4917.8 MH/s (27.23ms) @ Accel:256 Loops:128 Thr:128 Vec:1
Speed.#*.........: 10398.6 MH/s

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#3.........:   437.4 MH/s (37.97ms) @ Accel:16 Loops:512 Thr:64 Vec:1
Speed.#4.........:   308.3 MH/s (53.27ms) @ Accel:16 Loops:512 Thr:64 Vec:1
Speed.#*.........:   745.8 MH/s

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

* Device #3: Skipping (hash-mode 1500)
             This is due to a known CUDA/HIP/OpenCL runtime/driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #4: Skipping (hash-mode 1500)
             This is due to a known CUDA/HIP/OpenCL runtime/driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
Speed.#*.........:        0 H/s

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#3.........:   347.0 kH/s (60.06ms) @ Accel:64 Loops:1000 Thr:128 Vec:1
Speed.#4.........:   325.2 kH/s (56.16ms) @ Accel:64 Loops:1000 Thr:128 Vec:1
Speed.#*.........:   672.2 kH/s

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#3.........:     4483 H/s (55.00ms) @ Accel:32 Loops:32 Thr:8 Vec:1
Speed.#4.........:     4480 H/s (55.21ms) @ Accel:32 Loops:32 Thr:8 Vec:1
Speed.#*.........:     8963 H/s

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#3.........:    22795 H/s (70.36ms) @ Accel:128 Loops:256 Thr:256 Vec:1
Speed.#4.........:    22797 H/s (69.97ms) @ Accel:128 Loops:256 Thr:256 Vec:1
Speed.#*.........:    45592 H/s

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#3.........: 43232.0 kH/s (107.50ms) @ Accel:16 Loops:256 Thr:32 Vec:1
Speed.#4.........: 40998.0 kH/s (110.60ms) @ Accel:16 Loops:256 Thr:32 Vec:1
Speed.#*.........: 84230.1 kH/s

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

* Device #3: Skipping (hash-mode 13100)
             This is due to a known CUDA/HIP/OpenCL runtime/driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #4: Skipping (hash-mode 13100)
             This is due to a known CUDA/HIP/OpenCL runtime/driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
Speed.#*.........:        0 H/s

---------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1) [Iterations: 23999]
---------------------------------------------------------------

* Device #3: Skipping (hash-mode 15300)
             This is due to a known CUDA/HIP/OpenCL runtime/driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
* Device #4: Skipping (hash-mode 15300)
             This is due to a known CUDA/HIP/OpenCL runtime/driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.
Speed.#*.........:        0 H/s

---------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2) [Iterations: 12899]
---------------------------------------------------------------

Speed.#3.........:     4176 H/s (38.76ms) @ Accel:128 Loops:4 Thr:128 Vec:1
Speed.#4.........:     4176 H/s (38.66ms) @ Accel:128 Loops:4 Thr:128 Vec:1
Speed.#*.........:     8352 H/s

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#3.........:    54583 H/s (60.71ms) @ Accel:32 Loops:63 Thr:64 Vec:1
Speed.#4.........:    56501 H/s (70.28ms) @ Accel:32 Loops:63 Thr:64 Vec:1
Speed.#*.........:   111.1 kH/s

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#3.........:    30078 H/s (81.71ms) @ Accel:16 Loops:4096 Thr:64 Vec:1
Speed.#4.........:    29868 H/s (88.46ms) @ Accel:16 Loops:4096 Thr:64 Vec:1
Speed.#*.........:    59946 H/s

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#3.........:     1496 H/s (347.89ms) @ Accel:4 Loops:16384 Thr:64 Vec:1
Speed.#4.........:     1224 H/s (312.67ms) @ Accel:4 Loops:16384 Thr:64 Vec:1
Speed.#*.........:     2720 H/s

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#3.........:     7826 H/s (56.44ms) @ Accel:8 Loops:1024 Thr:64 Vec:1
Speed.#4.........:     7829 H/s (56.11ms) @ Accel:8 Loops:1024 Thr:64 Vec:1
Speed.#*.........:    15655 H/s

-----------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit) [Iterations: 1999]
-----------------------------------------------------------------------

Speed.#3.........:    36763 H/s (26.59ms) @ Accel:32 Loops:16 Thr:128 Vec:1
Speed.#4.........:    36775 H/s (25.98ms) @ Accel:32 Loops:16 Thr:128 Vec:1
Speed.#*.........:    73538 H/s

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#3.........:    19059 H/s (65.37ms) @ Accel:32 Loops:512 Thr:64 Vec:1
Speed.#4.........:    14918 H/s (83.80ms) @ Accel:32 Loops:512 Thr:64 Vec:1
Speed.#*.........:    33977 H/s

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#3.........:    69877 H/s (31.29ms) @ Accel:32 Loops:249 Thr:64 Vec:1
Speed.#4.........:    69824 H/s (25.93ms) @ Accel:32 Loops:249 Thr:64 Vec:1
Speed.#*.........:   139.7 kH/s

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#3.........:      952 H/s (86.41ms) @ Accel:2048 Loops:128 Thr:64 Vec:1
Speed.#4.........:      931 H/s (88.75ms) @ Accel:2048 Loops:128 Thr:64 Vec:1
Speed.#*.........:     1882 H/s

Started: Mon Feb 14 13:10:39 2022
Stopped: Mon Feb 14 13:17:43 2022
```
