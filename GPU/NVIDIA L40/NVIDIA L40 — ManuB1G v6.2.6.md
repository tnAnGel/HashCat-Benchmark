# NVIDIA L40

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA L40
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [ManuB1G](https://hashcat.net/forum/thread-11732.html)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 121.3 GH/s |
| 100 | SHA1 | 44103.0 MH/s |
| 1400 | SHA2-256 | 18695.2 MH/s |
| 1700 | SHA2-512 | 6212.1 MH/s |
| 1000 | NTLM | 206.3 GH/s |
| 3200 | bcrypt | 176.7 kH/s |
| 1800 | sha512crypt | 879.2 kH/s |
| 500 | md5crypt | 54471.2 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 2241.6 kH/s |
| 7500 | Kerberos AS-REQ (23) | 3366.9 MH/s |
| 13100 | Kerberos TGS-REP (23) | 3333.5 MH/s |
| 11300 | Bitcoin wallet.dat | 28061 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 1629.2 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

CUDA API (CUDA 12.3)
====================
* Device #1: NVIDIA L40, 44945/45382 MB, 142MCU
* Device #2: NVIDIA L40, 44945/45382 MB, 142MCU
* Device #3: NVIDIA L40, 44945/45382 MB, 142MCU
* Device #4: NVIDIA L40, 44945/45382 MB, 142MCU
* Device #5: NVIDIA L40, 44945/45382 MB, 142MCU
* Device #6: NVIDIA L40, 44945/45382 MB, 142MCU
* Device #7: NVIDIA L40, 44945/45382 MB, 142MCU
* Device #8: NVIDIA L40, 44945/45382 MB, 142MCU

OpenCL API (OpenCL 3.0 PoCL 3.1+debian  Linux, None+Asserts, RELOC, SPIR, LLVM 15.0.6, SLEEF, DISTRO, POCL_DEBUG) - Platform #1 [The pocl project]
==================================================================================================================================================
* Device #9: pthread-skylake-avx512-AMD EPYC 9754 128-Core Processor, skipped

OpenCL API (OpenCL 3.0 CUDA 12.3.68) - Platform #2 [NVIDIA Corporation]
=======================================================================
* Device #10: NVIDIA L40, skipped
* Device #11: NVIDIA L40, skipped
* Device #12: NVIDIA L40, skipped
* Device #13: NVIDIA L40, skipped
* Device #14: NVIDIA L40, skipped
* Device #15: NVIDIA L40, skipped
* Device #16: NVIDIA L40, skipped
* Device #17: NVIDIA L40, skipped

OpenCL API (OpenCL 2.1 LINUX) - Platform #3 [Intel(R) Corporation]
==================================================================
* Device #18: AMD EPYC 9754 128-Core Processor, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:  121.3 GH/s (38.81ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#2.........:  126.4 GH/s (37.22ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#3.........:  121.8 GH/s (38.65ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#4.........:  124.6 GH/s (37.83ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#5.........:  122.7 GH/s (38.35ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#6.........:  123.1 GH/s (38.23ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#7.........:  124.7 GH/s (37.75ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#8.........:  121.3 GH/s (38.78ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#*.........:  985.9 GH/s

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........: 44103.0 MH/s (53.58ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#2.........: 44645.6 MH/s (52.90ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#3.........: 43572.3 MH/s (54.21ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#4.........: 44121.2 MH/s (53.55ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#5.........: 43396.9 MH/s (54.47ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#6.........: 44544.8 MH/s (53.03ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#7.........: 44594.9 MH/s (52.97ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#8.........: 43443.2 MH/s (54.38ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#*.........:  352.4 GH/s

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........: 18695.2 MH/s (63.27ms) @ Accel:16 Loops:1024 Thr:512 Vec:1
Speed.#2.........: 18954.7 MH/s (62.41ms) @ Accel:16 Loops:1024 Thr:512 Vec:1
Speed.#3.........: 18341.1 MH/s (64.50ms) @ Accel:16 Loops:1024 Thr:512 Vec:1
Speed.#4.........: 18872.2 MH/s (62.69ms) @ Accel:16 Loops:1024 Thr:512 Vec:1
Speed.#5.........: 18400.7 MH/s (64.28ms) @ Accel:16 Loops:1024 Thr:512 Vec:1
Speed.#6.........: 18769.2 MH/s (63.05ms) @ Accel:16 Loops:1024 Thr:512 Vec:1
Speed.#7.........: 18820.3 MH/s (62.88ms) @ Accel:16 Loops:1024 Thr:512 Vec:1
Speed.#8.........: 18520.2 MH/s (63.88ms) @ Accel:16 Loops:1024 Thr:512 Vec:1
Speed.#*.........:  149.4 GH/s

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  6212.1 MH/s (95.48ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  6221.5 MH/s (95.32ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  6084.4 MH/s (97.50ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  6181.3 MH/s (95.90ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#5.........:  6060.2 MH/s (97.81ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#6.........:  6168.4 MH/s (96.08ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#7.........:  6155.0 MH/s (96.33ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#8.........:  6078.4 MH/s (97.57ms) @ Accel:64 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 49161.3 MH/s

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:  2241.6 kH/s (63.99ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#2.........:  2225.1 kH/s (64.42ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#3.........:  2207.6 kH/s (64.96ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#4.........:  2255.4 kH/s (63.55ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#5.........:  2209.2 kH/s (64.85ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#6.........:  2236.2 kH/s (64.07ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#7.........:  2262.0 kH/s (63.37ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#8.........:  2105.0 kH/s (67.68ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#*.........: 17742.0 kH/s

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:  206.3 GH/s (22.58ms) @ Accel:256 Loops:1024 Thr:128 Vec:1
Speed.#2.........:  210.8 GH/s (22.07ms) @ Accel:256 Loops:1024 Thr:128 Vec:1
Speed.#3.........:  202.9 GH/s (22.98ms) @ Accel:256 Loops:1024 Thr:128 Vec:1
Speed.#4.........:  206.6 GH/s (22.59ms) @ Accel:256 Loops:1024 Thr:128 Vec:1
Speed.#5.........:  204.3 GH/s (22.77ms) @ Accel:256 Loops:1024 Thr:128 Vec:1
Speed.#6.........:  205.2 GH/s (22.69ms) @ Accel:256 Loops:1024 Thr:128 Vec:1
Speed.#7.........:  209.5 GH/s (22.21ms) @ Accel:256 Loops:1024 Thr:128 Vec:1
Speed.#8.........:  205.0 GH/s (22.73ms) @ Accel:256 Loops:1024 Thr:128 Vec:1
Speed.#*.........:  1650.7 GH/s

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:  130.0 GH/s (8.95ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#2.........:  131.7 GH/s (8.87ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#3.........:  128.3 GH/s (9.08ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#4.........:  131.3 GH/s (8.85ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#5.........:  127.9 GH/s (9.08ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#6.........:  129.4 GH/s (9.02ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#7.........:  129.6 GH/s (8.99ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#8.........:  128.3 GH/s (9.08ms) @ Accel:32 Loops:1024 Thr:256 Vec:1
Speed.#*.........:  1036.4 GH/s

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........:  129.3 GH/s (36.30ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#2.........:  133.0 GH/s (35.26ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#3.........:  127.9 GH/s (36.69ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#4.........:  129.7 GH/s (36.24ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#5.........:  128.6 GH/s (36.45ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#6.........:  130.0 GH/s (36.08ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#7.........:  130.5 GH/s (35.93ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#8.........:  128.7 GH/s (36.49ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#*.........:  1037.8 GH/s

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  9048.9 MH/s (65.32ms) @ Accel:512 Loops:256 Thr:32 Vec:1
Speed.#2.........:  9312.1 MH/s (63.45ms) @ Accel:512 Loops:256 Thr:32 Vec:1
Speed.#3.........:  8981.4 MH/s (65.82ms) @ Accel:512 Loops:256 Thr:32 Vec:1
Speed.#4.........:  9117.9 MH/s (64.82ms) @ Accel:512 Loops:256 Thr:32 Vec:1
Speed.#5.........:  9040.9 MH/s (65.35ms) @ Accel:512 Loops:256 Thr:32 Vec:1
Speed.#6.........:  9098.4 MH/s (64.97ms) @ Accel:512 Loops:256 Thr:32 Vec:1
Speed.#7.........:  9270.8 MH/s (63.80ms) @ Accel:512 Loops:256 Thr:32 Vec:1
Speed.#8.........:  8986.3 MH/s (65.78ms) @ Accel:512 Loops:256 Thr:32 Vec:1
Speed.#*.........: 72856.7 MH/s

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:  5339.3 MH/s (55.38ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  5423.8 MH/s (54.48ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  5214.8 MH/s (56.67ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  5364.2 MH/s (55.15ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#5.........:  5311.3 MH/s (55.70ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#6.........:  5373.6 MH/s (55.03ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#7.........:  5393.6 MH/s (54.89ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#8.........:  5281.3 MH/s (55.98ms) @ Accel:32 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 42701.8 MH/s

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........: 54471.2 kH/s (67.42ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1
Speed.#2.........: 54793.0 kH/s (66.85ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1
Speed.#3.........: 50721.9 kH/s (72.09ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1
Speed.#4.........: 53799.5 kH/s (68.26ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1
Speed.#5.........: 51983.4 kH/s (71.45ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1
Speed.#6.........: 53013.3 kH/s (69.70ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1
Speed.#7.........: 53485.6 kH/s (68.76ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1
Speed.#8.........: 53358.9 kH/s (69.19ms) @ Accel:32 Loops:1000 Thr:1024 Vec:1
Speed.#*.........:  425.6 MH/s

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:  176.7 kH/s (54.67ms) @ Accel:4 Loops:32 Thr:24 Vec:1
Speed.#2.........:  175.8 kH/s (54.68ms) @ Accel:4 Loops:32 Thr:24 Vec:1
Speed.#3.........:  176.8 kH/s (54.67ms) @ Accel:4 Loops:32 Thr:24 Vec:1
Speed.#4.........:  177.8 kH/s (54.67ms) @ Accel:4 Loops:32 Thr:24 Vec:1
Speed.#5.........:  176.9 kH/s (54.66ms) @ Accel:4 Loops:32 Thr:24 Vec:1
Speed.#6.........:  177.8 kH/s (54.67ms) @ Accel:4 Loops:32 Thr:24 Vec:1
Speed.#7.........:  176.5 kH/s (54.67ms) @ Accel:4 Loops:32 Thr:24 Vec:1
Speed.#8.........:  176.7 kH/s (54.67ms) @ Accel:4 Loops:32 Thr:24 Vec:1
Speed.#*.........:  1415.1 kH/s

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:  879.2 kH/s (58.89ms) @ Accel:2048 Loops:1024 Thr:128 Vec:1
Speed.#2.........:  895.1 kH/s (57.82ms) @ Accel:2048 Loops:1024 Thr:128 Vec:1
Speed.#3.........:  804.3 kH/s (64.25ms) @ Accel:2048 Loops:1024 Thr:128 Vec:1
Speed.#4.........:  905.1 kH/s (57.13ms) @ Accel:2048 Loops:1024 Thr:128 Vec:1
Speed.#5.........:  827.2 kH/s (62.55ms) @ Accel:2048 Loops:1024 Thr:128 Vec:1
Speed.#6.........:  882.0 kH/s (58.60ms) @ Accel:2048 Loops:1024 Thr:128 Vec:1
Speed.#7.........:  879.5 kH/s (58.82ms) @ Accel:2048 Loops:1024 Thr:128 Vec:1
Speed.#8.........:  837.9 kH/s (61.78ms) @ Accel:2048 Loops:1024 Thr:128 Vec:1
Speed.#*.........:  6910.3 kH/s

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:  3366.9 MH/s (87.92ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.#2.........:  3348.0 MH/s (88.41ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.#3.........:  3330.0 MH/s (88.93ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.#4.........:  3366.0 MH/s (87.96ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.#5.........:  3281.1 MH/s (90.10ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.#6.........:  3378.2 MH/s (87.57ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.#7.........:  3374.6 MH/s (87.65ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.#8.........:  3366.6 MH/s (87.99ms) @ Accel:512 Loops:128 Thr:32 Vec:1
Speed.#*.........: 26811.4 MH/s

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:  3333.5 MH/s (88.88ms) @ Accel:256 Loops:256 Thr:32 Vec:1
Speed.#2.........:  3313.4 MH/s (89.40ms) @ Accel:256 Loops:256 Thr:32 Vec:1
Speed.#3.........:  3299.2 MH/s (89.81ms) @ Accel:256 Loops:256 Thr:32 Vec:1
Speed.#4.........:  3332.7 MH/s (88.88ms) @ Accel:256 Loops:256 Thr:32 Vec:1
Speed.#5.........:  3251.9 MH/s (91.04ms) @ Accel:256 Loops:256 Thr:32 Vec:1
Speed.#6.........:  3346.5 MH/s (88.53ms) @ Accel:256 Loops:256 Thr:32 Vec:1
Speed.#7.........:  3339.1 MH/s (88.67ms) @ Accel:256 Loops:256 Thr:32 Vec:1
Speed.#8.........:  3331.0 MH/s (88.92ms) @ Accel:256 Loops:256 Thr:32 Vec:1
Speed.#*.........: 26547.3 MH/s

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:  397.4 kH/s (60.57ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#2.........:  398.2 kH/s (60.46ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#3.........:  388.6 kH/s (61.85ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#4.........:  397.8 kH/s (60.56ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#5.........:  386.3 kH/s (62.29ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#6.........:  393.6 kH/s (61.15ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#7.........:  400.2 kH/s (60.13ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#8.........:  396.5 kH/s (60.72ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#*.........:  3158.7 kH/s

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:  222.3 kH/s (49.93ms) @ Accel:8 Loops:512 Thr:256 Vec:1
Speed.#2.........:  225.5 kH/s (49.23ms) @ Accel:8 Loops:512 Thr:256 Vec:1
Speed.#3.........:  221.3 kH/s (50.21ms) @ Accel:8 Loops:512 Thr:256 Vec:1
Speed.#4.........:  223.9 kH/s (49.59ms) @ Accel:8 Loops:512 Thr:256 Vec:1
Speed.#5.........:  220.3 kH/s (50.45ms) @ Accel:8 Loops:512 Thr:256 Vec:1
Speed.#6.........:  224.6 kH/s (49.46ms) @ Accel:8 Loops:512 Thr:256 Vec:1
Speed.#7.........:  225.4 kH/s (49.31ms) @ Accel:8 Loops:512 Thr:256 Vec:1
Speed.#8.........:  221.6 kH/s (49.98ms) @ Accel:8 Loops:512 Thr:256 Vec:1
Speed.#*.........:  1784.9 kH/s

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:  3012.6 kH/s (47.21ms) @ Accel:4 Loops:1023 Thr:256 Vec:1
Speed.#2.........:  3024.9 kH/s (46.94ms) @ Accel:4 Loops:1023 Thr:256 Vec:1
Speed.#3.........:  2489.5 kH/s (53.27ms) @ Accel:4 Loops:1023 Thr:256 Vec:1
Speed.#4.........:  3031.8 kH/s (46.92ms) @ Accel:4 Loops:1023 Thr:256 Vec:1
Speed.#5.........:  3049.6 kH/s (46.61ms) @ Accel:4 Loops:1023 Thr:256 Vec:1
Speed.#6.........:  2576.0 kH/s (52.18ms) @ Accel:4 Loops:1023 Thr:256 Vec:1
Speed.#7.........:  2987.3 kH/s (47.59ms) @ Accel:4 Loops:1023 Thr:256 Vec:1
Speed.#8.........:  3016.3 kH/s (47.15ms) @ Accel:4 Loops:1023 Thr:256 Vec:1
Speed.#*.........: 23188.0 kH/s

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:  2075.8 kH/s (62.20ms) @ Accel:16 Loops:4096 Thr:256 Vec:1
Speed.#2.........:  2203.6 kH/s (61.33ms) @ Accel:16 Loops:4096 Thr:256 Vec:1
Speed.#3.........:  2007.7 kH/s (66.11ms) @ Accel:16 Loops:4096 Thr:256 Vec:1
Speed.#4.........:  2076.0 kH/s (62.56ms) @ Accel:16 Loops:4096 Thr:256 Vec:1
Speed.#5.........:  1993.2 kH/s (67.35ms) @ Accel:16 Loops:4096 Thr:256 Vec:1
Speed.#6.........:  2054.9 kH/s (64.62ms) @ Accel:16 Loops:4096 Thr:256 Vec:1
Speed.#7.........:  2083.3 kH/s (62.07ms) @ Accel:16 Loops:4096 Thr:256 Vec:1
Speed.#8.........:  2066.0 kH/s (65.64ms) @ Accel:16 Loops:4096 Thr:256 Vec:1
Speed.#*.........: 16560.3 kH/s

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    56345 H/s (4.86ms) @ Accel:64 Loops:16384 Thr:32 Vec:1
Speed.#2.........:    57036 H/s (4.80ms) @ Accel:64 Loops:16384 Thr:32 Vec:1
Speed.#3.........:    52286 H/s (5.27ms) @ Accel:64 Loops:16384 Thr:32 Vec:1
Speed.#4.........:    56372 H/s (4.85ms) @ Accel:64 Loops:16384 Thr:32 Vec:1
Speed.#5.........:    48026 H/s (5.51ms) @ Accel:64 Loops:16384 Thr:32 Vec:1
Speed.#6.........:    55779 H/s (4.92ms) @ Accel:64 Loops:16384 Thr:32 Vec:1
Speed.#7.........:    55683 H/s (4.92ms) @ Accel:64 Loops:16384 Thr:32 Vec:1
Speed.#8.........:    55350 H/s (4.98ms) @ Accel:64 Loops:16384 Thr:32 Vec:1
Speed.#*.........:  436.9 kH/s

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:  227.7 kH/s (79.39ms) @ Accel:8 Loops:512 Thr:1024 Vec:1
Speed.#2.........:  230.2 kH/s (78.56ms) @ Accel:8 Loops:512 Thr:1024 Vec:1
Speed.#3.........:  222.8 kH/s (81.06ms) @ Accel:8 Loops:512 Thr:1024 Vec:1
Speed.#4.........:  229.6 kH/s (78.73ms) @ Accel:8 Loops:512 Thr:1024 Vec:1
Speed.#5.........:  224.4 kH/s (80.54ms) @ Accel:8 Loops:512 Thr:1024 Vec:1
Speed.#6.........:  224.0 kH/s (80.63ms) @ Accel:8 Loops:512 Thr:1024 Vec:1
Speed.#7.........:  228.5 kH/s (79.09ms) @ Accel:8 Loops:512 Thr:1024 Vec:1
Speed.#8.........:  225.1 kH/s (80.31ms) @ Accel:8 Loops:512 Thr:1024 Vec:1
Speed.#*.........:  1812.2 kH/s

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:  1629.2 kH/s (80.83ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#2.........:  1662.8 kH/s (79.18ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#3.........:  1544.3 kH/s (84.36ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#4.........:  1648.4 kH/s (80.02ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#5.........:  1580.4 kH/s (83.61ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#6.........:  1622.8 kH/s (81.37ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#7.........:  1627.7 kH/s (81.03ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#8.........:  1546.7 kH/s (85.31ms) @ Accel:64 Loops:512 Thr:64 Vec:1
Speed.#*.........: 12862.4 kH/s

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:  324.1 kH/s (74.42ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#2.........:  324.0 kH/s (74.38ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#3.........:  324.1 kH/s (74.41ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#4.........:  324.2 kH/s (74.38ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#5.........:  321.3 kH/s (74.99ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#6.........:  324.1 kH/s (74.38ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#7.........:  324.3 kH/s (74.37ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#8.........:  324.3 kH/s (74.37ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#*.........:  2590.3 kH/s

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........: 16322.9 kH/s (65.21ms) @ Accel:8 Loops:499 Thr:1024 Vec:1
Speed.#2.........: 15706.6 kH/s (67.97ms) @ Accel:8 Loops:499 Thr:1024 Vec:1
Speed.#3.........: 15608.7 kH/s (68.51ms) @ Accel:8 Loops:499 Thr:1024 Vec:1
Speed.#4.........: 16075.4 kH/s (66.35ms) @ Accel:8 Loops:499 Thr:1024 Vec:1
Speed.#5.........: 15642.4 kH/s (68.27ms) @ Accel:8 Loops:499 Thr:1024 Vec:1
Speed.#6.........: 16330.0 kH/s (65.04ms) @ Accel:8 Loops:499 Thr:1024 Vec:1
Speed.#7.........: 16007.1 kH/s (66.53ms) @ Accel:8 Loops:499 Thr:1024 Vec:1
Speed.#8.........: 13253.9 kH/s (79.54ms) @ Accel:8 Loops:499 Thr:1024 Vec:1
Speed.#*.........:  124.9 MH/s

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:    28061 H/s (52.71ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#2.........:    28418 H/s (52.00ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#3.........:    27122 H/s (54.58ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#4.........:    28072 H/s (52.67ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#5.........:    27103 H/s (54.51ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#6.........:    27721 H/s (53.30ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#7.........:    27959 H/s (52.88ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#8.........:    27571 H/s (53.64ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#*.........:  222.0 kH/s

Started: Fri Dec 15 23:10:36 2023
Stopped: Fri Dec 15 23:15:10 2023
```
