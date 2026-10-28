# NVIDIA Quadro P4000

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA Quadro P4000
- **Версия hashcat / Version:** v6.2.5
- **Источник / Source:** [Gyfer](https://hashcat.net/forum/thread-11482.html)
- **Особенности прогона / Run options:** многокарточный прогон (GTX 1660 SUPER + Quadro P4000 + GT 730 + CPU) без ограничения устройств; Quadro P4000 — это `Device #2`, все её результаты в строках `Speed.#2`

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 13818.9 MH/s |
| 100 | SHA1 | 5469.6 MH/s |
| 1400 | SHA2-256 | 2041.4 MH/s |
| 1700 | SHA2-512 | 658.0 MH/s |
| 1000 | NTLM | 23516.7 MH/s |
| 3200 | bcrypt | 10446 H/s |
| 1800 | sha512crypt | 85689 H/s |
| 500 | md5crypt | 5405.2 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 285.1 kH/s |
| 7500 | Kerberos AS-REQ (23) | 226.5 MH/s |
| 13100 | Kerberos TGS-REP (23) | 226.6 MH/s |
| 11300 | Bitcoin wallet.dat | 3016 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 180.5 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.5) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

Unsupported AMD HIP runtime version '4.2' detected! Falling back to OpenCL...

* Device #3: This hardware has outdated CUDA compute capability (3.5).
            For modern OpenCL performance, upgrade to hardware that supports
            CUDA compute capability version 5.0 (Maxwell) or higher.
CUDA API (CUDA 11.4)
====================
* Device #1: NVIDIA GeForce GTX 1660 SUPER, 5877/5944 MB, 22MCU
* Device #2: Quadro P4000, 8038/8119 MB, 14MCU
* Device #3: NVIDIA GeForce GT 730, 1982/2002 MB, 2MCU

OpenCL API (OpenCL 3.0 PoCL 3.0-rc2  Linux, RelWithDebInfo, RELOC, SPIR, LLVM 10.0.0, SLEEF, POCL_DEBUG) - Platform #1 [The pocl project]
=========================================================================================================================================
* Device #4: pthread-Intel(R) Core(TM) i3-4130 CPU @ 3.40GHz, 2847/5758 MB (1024 MB allocatable), 4MCU

OpenCL API (OpenCL 2.0 AMD-APP (3314.0)) - Platform #2 [Advanced Micro Devices, Inc.]
=====================================================================================

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 17269.3 MH/s (83.39ms) @ Accel:256 Loops:512 Thr:512 Vec:1
Speed.#2.........: 13818.9 MH/s (66.92ms) @ Accel:256 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  895.2 MH/s (73.53ms) @ Accel:256 Loops:1024 Thr:128 Vec:2
Speed.#4.........:  276.1 MH/s (7.45ms) @ Accel:512 Loops:1024 Thr:1 Vec:8
Speed.#*.........: 32259.6 MH/s

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  5928.4 MH/s (61.41ms) @ Accel:256 Loops:256 Thr:256 Vec:1
Speed.#2.........:  5469.6 MH/s (84.95ms) @ Accel:256 Loops:256 Thr:512 Vec:1
Speed.#3.........:  253.2 MH/s (65.19ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  119.0 MH/s (16.71ms) @ Accel:512 Loops:1024 Thr:1 Vec:8
Speed.#*.........: 11770.3 MH/s

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  2588.3 MH/s (70.98ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........:  2041.4 MH/s (57.31ms) @ Accel:32 Loops:256 Thr:1024 Vec:1
Speed.#3.........:  111.8 MH/s (73.91ms) @ Accel:8 Loops:512 Thr:1024 Vec:1
Speed.#4.........: 53338.8 kH/s (39.19ms) @ Accel:512 Loops:1024 Thr:1 Vec:8
Speed.#*.........:  4794.8 MH/s

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  862.3 MH/s (53.37ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#2.........:  658.0 MH/s (44.54ms) @ Accel:16 Loops:512 Thr:256 Vec:1
Speed.#3.........: 26638.0 kH/s (77.74ms) @ Accel:32 Loops:1024 Thr:32 Vec:1
Speed.#4.........: 15595.7 kH/s (67.14ms) @ Accel:256 Loops:1024 Thr:1 Vec:4
Speed.#*.........:  1562.6 MH/s

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:  292.3 kH/s (74.24ms) @ Accel:16 Loops:512 Thr:512 Vec:1
Speed.#2.........:  285.1 kH/s (49.73ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#3.........:    12276 H/s (77.54ms) @ Accel:16 Loops:512 Thr:256 Vec:1
Speed.#4.........:    6038 H/s (83.33ms) @ Accel:512 Loops:1024 Thr:1 Vec:8
Speed.#*.........:  595.8 kH/s

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 31637.2 MH/s (90.61ms) @ Accel:128 Loops:1024 Thr:1024 Vec:1
Speed.#2.........: 23516.7 MH/s (78.22ms) @ Accel:256 Loops:512 Thr:1024 Vec:1
Speed.#3.........:  1413.4 MH/s (89.57ms) @ Accel:4096 Loops:256 Thr:64 Vec:4
Speed.#4.........:  402.1 MH/s (5.11ms) @ Accel:512 Loops:1024 Thr:1 Vec:8
Speed.#*.........: 56969.4 MH/s

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........: 17398.3 MH/s (41.93ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1
Speed.#2.........: 14020.7 MH/s (66.65ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  489.6 MH/s (67.32ms) @ Accel:128 Loops:1024 Thr:128 Vec:1
Speed.#4.........: 52062.7 kH/s (39.17ms) @ Accel:512 Loops:1024 Thr:1 Vec:8
Speed.#*.........: 31960.7 MH/s

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 18163.7 MH/s (78.98ms) @ Accel:512 Loops:512 Thr:256 Vec:1
Speed.#2.........: 14033.8 MH/s (66.18ms) @ Accel:128 Loops:512 Thr:1024 Vec:1
Speed.#3.........:  916.7 MH/s (71.30ms) @ Accel:512 Loops:512 Thr:128 Vec:4
Speed.#4.........:  291.4 MH/s (7.09ms) @ Accel:512 Loops:1024 Thr:1 Vec:8
Speed.#*.........: 33405.7 MH/s

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  1336.4 MH/s (67.89ms) @ Accel:256 Loops:64 Thr:256 Vec:1
Speed.#2.........:  1054.6 MH/s (55.39ms) @ Accel:128 Loops:64 Thr:512 Vec:1
Speed.#3.........: 44933.0 kH/s (92.15ms) @ Accel:4 Loops:1024 Thr:512 Vec:2
Speed.#4.........: 21484.4 kH/s (48.70ms) @ Accel:512 Loops:512 Thr:1 Vec:8
Speed.#*.........:  2457.4 MH/s

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:  715.5 MH/s (64.24ms) @ Accel:16 Loops:1024 Thr:128 Vec:1
Speed.#2.........:  552.2 MH/s (52.97ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#3.........: 21461.6 kH/s (48.56ms) @ Accel:2 Loops:1024 Thr:256 Vec:1
Speed.#4.........:  2076.0 kH/s (59.07ms) @ Accel:32 Loops:1024 Thr:1 Vec:8
Speed.#*.........:  1291.2 MH/s

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:  6771.1 kH/s (82.58ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1
Speed.#2.........:  5405.2 kH/s (66.97ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1
Speed.#3.........:  309.1 kH/s (77.27ms) @ Accel:128 Loops:500 Thr:256 Vec:1
Speed.#4.........:    22753 H/s (86.97ms) @ Accel:512 Loops:1000 Thr:1 Vec:8
Speed.#*.........: 12508.1 kH/s

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    17638 H/s (55.92ms) @ Accel:64 Loops:32 Thr:16 Vec:1
Speed.#2.........:    10446 H/s (71.32ms) @ Accel:64 Loops:32 Thr:12 Vec:1
Speed.#3.........:      156 H/s (72.79ms) @ Accel:2 Loops:16 Thr:12 Vec:1
Speed.#4.........:      18 H/s (2.06ms) @ Accel:4 Loops:32 Thr:1 Vec:1
Speed.#*.........:    28258 H/s

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:  136.6 kH/s (47.12ms) @ Accel:512 Loops:512 Thr:128 Vec:1
Speed.#2.........:    85689 H/s (74.90ms) @ Accel:64 Loops:512 Thr:1024 Vec:1
Speed.#3.........:    5492 H/s (72.03ms) @ Accel:256 Loops:128 Thr:64 Vec:1
Speed.#4.........:    1004 H/s (50.19ms) @ Accel:512 Loops:512 Thr:1 Vec:4
Speed.#*.........:  228.8 kH/s

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:  318.5 MH/s (72.17ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#2.........:  226.5 MH/s (64.69ms) @ Accel:128 Loops:256 Thr:32 Vec:1
Speed.#3.........:  4880.8 kH/s (53.46ms) @ Accel:128 Loops:32 Thr:32 Vec:1
Speed.#4.........:  2020.7 kH/s (64.79ms) @ Accel:128 Loops:256 Thr:1 Vec:8
Speed.#*.........:  551.9 MH/s

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:  315.9 MH/s (72.75ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#2.........:  226.6 MH/s (64.66ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#3.........:  4771.9 kH/s (54.60ms) @ Accel:64 Loops:64 Thr:32 Vec:1
Speed.#4.........:  1999.4 kH/s (65.46ms) @ Accel:32 Loops:1024 Thr:1 Vec:8
Speed.#*.........:  549.3 MH/s

---------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1) [Iterations: 23999]
---------------------------------------------------------------

Speed.#1.........:    51916 H/s (73.42ms) @ Accel:16 Loops:512 Thr:512 Vec:1
Speed.#2.........:    49991 H/s (47.25ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#3.........:    2125 H/s (78.15ms) @ Accel:16 Loops:1024 Thr:128 Vec:1
Speed.#4.........:    1063 H/s (79.73ms) @ Accel:512 Loops:1024 Thr:1 Vec:8
Speed.#*.........:  105.1 kH/s

---------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2) [Iterations: 12899]
---------------------------------------------------------------

Speed.#1.........:    28521 H/s (60.14ms) @ Accel:8 Loops:512 Thr:256 Vec:1
Speed.#2.........:    23251 H/s (47.20ms) @ Accel:2 Loops:1024 Thr:512 Vec:1
Speed.#3.........:    1100 H/s (71.15ms) @ Accel:2 Loops:512 Thr:512 Vec:1
Speed.#4.........:      576 H/s (68.21ms) @ Accel:256 Loops:512 Thr:1 Vec:4
Speed.#*.........:    53449 H/s

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:  357.0 kH/s (59.54ms) @ Accel:128 Loops:31 Thr:256 Vec:1
Speed.#2.........:  273.8 kH/s (49.41ms) @ Accel:64 Loops:31 Thr:512 Vec:1
Speed.#3.........:    13673 H/s (48.94ms) @ Accel:2 Loops:511 Thr:512 Vec:1
Speed.#4.........:    7111 H/s (57.06ms) @ Accel:512 Loops:255 Thr:1 Vec:4
Speed.#*.........:  651.6 kH/s

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:  285.3 kH/s (65.22ms) @ Accel:16 Loops:4096 Thr:256 Vec:1
Speed.#2.........:  218.8 kH/s (58.57ms) @ Accel:4 Loops:4096 Thr:1024 Vec:1
Speed.#3.........:    13271 H/s (66.38ms) @ Accel:2 Loops:4096 Thr:1024 Vec:1
Speed.#4.........:    1140 H/s (55.77ms) @ Accel:64 Loops:4096 Thr:1 Vec:8
Speed.#*.........:  518.4 kH/s

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    44107 H/s (62.76ms) @ Accel:8 Loops:16384 Thr:256 Vec:1
Speed.#2.........:    31671 H/s (55.19ms) @ Accel:4 Loops:16384 Thr:512 Vec:1
Speed.#3.........:    1518 H/s (80.38ms) @ Accel:32 Loops:16384 Thr:32 Vec:1
Speed.#4.........:      177 H/s (90.14ms) @ Accel:64 Loops:16384 Thr:1 Vec:8
Speed.#*.........:    77474 H/s

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    31599 H/s (43.84ms) @ Accel:128 Loops:64 Thr:256 Vec:1
Speed.#2.........:    24943 H/s (68.99ms) @ Accel:4 Loops:1024 Thr:1024 Vec:1
Speed.#3.........:    1422 H/s (87.96ms) @ Accel:16 Loops:128 Thr:1024 Vec:1
Speed.#4.........:      621 H/s (49.82ms) @ Accel:256 Loops:1024 Thr:1 Vec:8
Speed.#*.........:    58586 H/s

-----------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit) [Iterations: 1999]
-----------------------------------------------------------------------

Speed.#1.........:  225.9 kH/s (90.44ms) @ Accel:32 Loops:128 Thr:512 Vec:1
Speed.#2.........:  180.5 kH/s (73.76ms) @ Accel:8 Loops:256 Thr:1024 Vec:1
Speed.#3.........:    9277 H/s (50.38ms) @ Accel:4 Loops:128 Thr:1024 Vec:1
Speed.#4.........:    4176 H/s (59.29ms) @ Accel:128 Loops:1024 Thr:1 Vec:8
Speed.#*.........:  419.9 kH/s

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    19087 H/s (48.98ms) @ Accel:32 Loops:128 Thr:256 Vec:1
Speed.#2.........:    21715 H/s (54.93ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#3.........:    1536 H/s (55.27ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#4.........:      476 H/s (89.52ms) @ Accel:512 Loops:512 Thr:1 Vec:8
Speed.#*.........:    42815 H/s

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  1906.7 kH/s (37.83ms) @ Accel:128 Loops:62 Thr:256 Vec:1
Speed.#2.........:  1508.3 kH/s (55.60ms) @ Accel:32 Loops:124 Thr:1024 Vec:1
Speed.#3.........:    73897 H/s (56.35ms) @ Accel:8 Loops:249 Thr:1024 Vec:1
Speed.#4.........:    35818 H/s (51.20ms) @ Accel:512 Loops:499 Thr:1 Vec:8
Speed.#*.........:  3524.7 kH/s

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:    3893 H/s (85.43ms) @ Accel:2048 Loops:128 Thr:256 Vec:1
Speed.#2.........:    3016 H/s (55.20ms) @ Accel:256 Loops:128 Thr:1024 Vec:1
Speed.#3.........:      175 H/s (59.58ms) @ Accel:2 Loops:1024 Thr:1024 Vec:1
Speed.#4.........:      71 H/s (36.78ms) @ Accel:512 Loops:1024 Thr:1 Vec:4
Speed.#*.........:    7155 H/s

Started: Wed Jun 28 13:44:45 2023

Stopped: Wed Jun 28 14:04:53 2023
```
