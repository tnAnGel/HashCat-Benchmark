# NVIDIA GeForce RTX 3080 Laptop GPU

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce RTX 3080 Laptop GPU (RTX 3080 Mobile)
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [MaxiHP, hashcat Forum](https://hashcat.net/forum/thread-11085.html)
- **Примечание / Note:** многоустройственный прогон — Device #1 это RTX 3080 Laptop GPU, Device #2/#3 это встроенная AMD Radeon(TM) Graphics; ниже в таблице только строки `Speed.#1`. Вывод неполный: часть режимов (12500, 13400, 11300) упала с `hipMemAlloc(): 2` на AMD-устройстве.

## Ключевые результаты / Highlights (Speed.#1 = RTX 3080 Laptop GPU)

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 30312.4 MH/s |
| 100 | SHA1 | 9846.7 MH/s |
| 1400 | SHA2-256 | 4265.7 MH/s |
| 1700 | SHA2-512 | 1413.5 MH/s |
| 1000 | NTLM | 53455.9 MH/s |
| 3200 | bcrypt | 57605 H/s |
| 1800 | sha512crypt | 148.4 kH/s |
| 500 | md5crypt | 12051.6 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 477.6 kH/s |
| 7500 | Kerberos AS-REQ (23) | 673.3 MH/s |
| 13100 | Kerberos TGS-REP (23) | 708.5 MH/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 402.6 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode
Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.
* Device #1: WARNING! Kernel exec timeout is not disabled.
            This may cause "CL_OUT_OF_RESOURCES" or related errors.
            To disable the timeout, see: https://hashcat.net/q/timeoutpatch
* Device #4: WARNING! Kernel exec timeout is not disabled.
            This may cause "CL_OUT_OF_RESOURCES" or related errors.
            To disable the timeout, see: https://hashcat.net/q/timeoutpatch
ADL2_Overdrive_Caps(): -8
ADL2_Overdrive_Caps(): -8
ADL2_Overdrive_Caps(): -8
ADL2_Overdrive_Caps(): -8
nvmlDeviceGetFanSpeed(): Not Supported
ADL_Overdrive5_FanSpeed_Get(): -100
ADL_Overdrive5_Temperature_Get(): -100
ADL_Overdrive5_FanSpeed_Get(): -100
ADL_Overdrive5_Temperature_Get(): -100
CUDA API (CUDA 11.8)
====================
* Device #1: NVIDIA GeForce RTX 3080 Laptop GPU, 7119/8191 MB, 48MCU
HIP API (HIP 4.4)
=================
* Device #2: AMD Radeon(TM) Graphics, 6084/6216 MB, 8MCU
* Device #3: AMD Radeon(TM) Graphics, 6084/6216 MB, 8MCU
OpenCL API (OpenCL 3.0 CUDA 11.8.87) - Platform #1 [NVIDIA Corporation]
=======================================================================
* Device #4: NVIDIA GeForce RTX 3080 Laptop GPU, skipped
OpenCL API (OpenCL 2.1 AMD-APP (3380.6)) - Platform #2 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #5: AMD Radeon(TM) Graphics, skipped
* Device #6: AMD Radeon(TM) Graphics, skipped
Benchmark relevant options:
===========================
* --optimized-kernel-enable
-------------------
* Hash-Mode 0 (MD5)
-------------------
Speed.#1.........: 30312.4 MH/s (52.51ms) @ Accel:128 Loops:1024 Thr:256 Vec:8
Speed.#2.........:  1833.1 MH/s (28.36ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#3.........:  1805.7 MH/s (28.14ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#*.........: 33951.3 MH/s
----------------------
* Hash-Mode 100 (SHA1)
----------------------
Speed.#1.........:  9846.7 MH/s (81.14ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#2.........:  643.2 MH/s (47.22ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#3.........:  658.8 MH/s (47.36ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#*.........: 11148.7 MH/s
---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------
Speed.#1.........:  4265.7 MH/s (93.87ms) @ Accel:256 Loops:1024 Thr:32 Vec:1
Speed.#2.........:  278.3 MH/s (107.02ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#3.........:  270.2 MH/s (108.50ms) @ Accel:128 Loops:512 Thr:64 Vec:1
Speed.#*.........:  4814.2 MH/s
---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------
Speed.#1.........:  1413.5 MH/s (70.77ms) @ Accel:128 Loops:512 Thr:32 Vec:1
Speed.#2.........: 77488.2 kH/s (93.80ms) @ Accel:64 Loops:256 Thr:64 Vec:1
Speed.#3.........: 74943.3 kH/s (95.21ms) @ Accel:64 Loops:256 Thr:64 Vec:1
Speed.#*.........:  1565.9 MH/s
-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------
Speed.#1.........:  477.6 kH/s (49.69ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#2.........:    35454 H/s (55.07ms) @ Accel:64 Loops:256 Thr:64 Vec:1
Speed.#3.........:    35580 H/s (54.88ms) @ Accel:64 Loops:256 Thr:64 Vec:1
Speed.#*.........:  548.7 kH/s
-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------
Speed.#1.........: 53455.9 MH/s (29.48ms) @ Accel:1024 Loops:1024 Thr:32 Vec:8
Speed.#2.........:  3355.6 MH/s (72.38ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  3224.0 MH/s (75.32ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 60035.6 MH/s
---------------------
* Hash-Mode 3000 (LM)
---------------------
Speed.#1.........: 29804.5 MH/s (26.51ms) @ Accel:256 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  935.3 MH/s (65.34ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  935.3 MH/s (67.54ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 31675.1 MH/s
--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------
Speed.#1.........: 30577.4 MH/s (51.83ms) @ Accel:64 Loops:1024 Thr:512 Vec:2
Speed.#2.........:  992.5 MH/s (59.37ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#3.........:  977.8 MH/s (60.44ms) @ Accel:512 Loops:256 Thr:64 Vec:1
Speed.#*.........: 32547.7 MH/s
----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------
Speed.#1.........:  2172.3 MH/s (92.21ms) @ Accel:128 Loops:1024 Thr:32 Vec:1
Speed.#2.........:  147.7 MH/s (51.45ms) @ Accel:64 Loops:256 Thr:64 Vec:1
Speed.#3.........:  147.7 MH/s (51.02ms) @ Accel:64 Loops:256 Thr:64 Vec:1
Speed.#*.........:  2467.8 MH/s
--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------
Speed.#1.........:  1222.6 MH/s (81.82ms) @ Accel:64 Loops:1024 Thr:32 Vec:1
Speed.#2.........: 59933.5 kH/s (58.48ms) @ Accel:8 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 62004.9 kH/s (56.75ms) @ Accel:8 Loops:1024 Thr:64 Vec:1
Speed.#*.........:  1344.6 MH/s
------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------
Speed.#1.........: 12051.6 kH/s (54.24ms) @ Accel:32 Loops:1000 Thr:512 Vec:1
Speed.#2.........:  740.0 kH/s (65.70ms) @ Accel:256 Loops:500 Thr:64 Vec:1
Speed.#3.........:  740.2 kH/s (65.67ms) @ Accel:256 Loops:500 Thr:64 Vec:1
Speed.#*.........: 13531.8 kH/s
----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------
Speed.#1.........:    57605 H/s (77.00ms) @ Accel:4 Loops:32 Thr:24 Vec:1
Speed.#2.........:      736 H/s (70.40ms) @ Accel:2 Loops:16 Thr:16 Vec:1
Speed.#3.........:      736 H/s (70.37ms) @ Accel:2 Loops:16 Thr:16 Vec:1
Speed.#*.........:    59077 H/s
--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------
Speed.#1.........:  148.4 kH/s (86.14ms) @ Accel:2048 Loops:512 Thr:64 Vec:1
Speed.#2.........:    4979 H/s (66.72ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#3.........:    4986 H/s (66.63ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#*.........:  158.4 kH/s
--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------
Speed.#1.........:  673.3 MH/s (74.21ms) @ Accel:32 Loops:1024 Thr:32 Vec:1
Speed.#2.........: 18036.3 kH/s (51.90ms) @ Accel:16 Loops:128 Thr:64 Vec:1
Speed.#3.........: 17537.9 kH/s (54.16ms) @ Accel:16 Loops:128 Thr:64 Vec:1
Speed.#*.........:  708.8 MH/s
-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------
Speed.#1.........:  708.5 MH/s (70.44ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#2.........: 10991.2 kH/s (83.52ms) @ Accel:16 Loops:128 Thr:64 Vec:1
Speed.#3.........: 11121.7 kH/s (83.07ms) @ Accel:16 Loops:128 Thr:64 Vec:1
Speed.#*.........:  730.6 MH/s
---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------
Speed.#1.........:    92205 H/s (88.19ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#2.........:    5799 H/s (239.28ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#3.........:    5811 H/s (238.79ms) @ Accel:256 Loops:256 Thr:64 Vec:1
Speed.#*.........:  103.8 kH/s
---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------
Speed.#1.........:    52024 H/s (71.96ms) @ Accel:64 Loops:512 Thr:32 Vec:1
Speed.#2.........:    2877 H/s (167.92ms) @ Accel:96 Loops:128 Thr:64 Vec:1
Speed.#3.........:    2877 H/s (167.92ms) @ Accel:96 Loops:128 Thr:64 Vec:1
Speed.#*.........:    57778 H/s
------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------
Speed.#1.........:  634.1 kH/s (47.88ms) @ Accel:8 Loops:511 Thr:256 Vec:1
Speed.#2.........:    33354 H/s (36.11ms) @ Accel:8 Loops:511 Thr:64 Vec:1
Speed.#3.........:    33378 H/s (36.09ms) @ Accel:8 Loops:511 Thr:64 Vec:1
Speed.#*.........:  700.8 kH/s
---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------
Speed.#1.........:  503.0 kH/s (92.06ms) @ Accel:128 Loops:4096 Thr:32 Vec:1
Speed.#2.........:    42001 H/s (46.81ms) @ Accel:16 Loops:4096 Thr:64 Vec:1
Speed.#3.........:    42163 H/s (45.85ms) @ Accel:16 Loops:4096 Thr:64 Vec:1
Speed.#*.........:  587.1 kH/s
------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------
hipMemAlloc(): 2
--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------
Speed.#1.........:    55276 H/s (55.12ms) @ Accel:256 Loops:256 Thr:32 Vec:1
Speed.#2.........:    4695 H/s (53.94ms) @ Accel:64 Loops:256 Thr:64 Vec:1
Speed.#3.........:    4695 H/s (53.95ms) @ Accel:64 Loops:256 Thr:64 Vec:1
Speed.#*.........:    64665 H/s
--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------
Speed.#1.........:  402.6 kH/s (55.67ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#2.........:    26043 H/s (72.43ms) @ Accel:16 Loops:512 Thr:64 Vec:1
Speed.#3.........:    26192 H/s (67.77ms) @ Accel:16 Loops:512 Thr:64 Vec:1
Speed.#*.........:  454.9 kH/s
-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------
hipMemAlloc(): 2
----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------
Speed.#1.........:  3336.6 kH/s (50.18ms) @ Accel:32 Loops:499 Thr:128 Vec:1
Speed.#2.........:  270.2 kH/s (74.01ms) @ Accel:128 Loops:249 Thr:64 Vec:1
Speed.#3.........:  268.6 kH/s (75.11ms) @ Accel:128 Loops:249 Thr:64 Vec:1
Speed.#*.........:  3875.4 kH/s
--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------
hipMemAlloc(): 2
Started: Sat Oct 22 14:21:31 2022
Stopped: Sat Oct 22 14:30:52 2022
```
