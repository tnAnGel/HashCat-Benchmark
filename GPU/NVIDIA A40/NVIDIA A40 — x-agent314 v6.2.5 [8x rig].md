# NVIDIA A40

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA A40
- **Версия hashcat / Version:** v6.2.5
- **Источник / Source:** [публичный сырой вывод](https://github.com/x-agent314/gpu_cloud_benchmarks/blob/main/hashcat_benchmark_8xA40.txt)
- **Параметры / Options:** `-b` (исходные параметры — см. лог)
- **Примечание / Note:** полный сырой benchmark восьми A40. В таблице приведены значения Device #1; в логе также есть суммарные Speed.#*. CUDA RTC отсутствует, поэтому hashcat переключился на OpenCL CUDA 12.0.151.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость |
|-----:|----------|---------:|
| 0 | MD5 | 65339.2 MH/s |
| 100 | SHA1 | 21190.4 MH/s |
| 1400 | SHA2-256 | 9143.5 MH/s |
| 1700 | SHA2-512 | 2692.0 MH/s |
| 1000 | NTLM | 110.7 GH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 1081.3 kH/s |
| 3200 | bcrypt | 71689 H/s |

## Полный доступный сырой вывод / Raw output

```text
hashcat (v6.2.5) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

Successfully initialized NVIDIA CUDA library.

Failed to initialize NVIDIA RTC library.

* Device #1: CUDA SDK Toolkit not installed or incorrectly installed.
             CUDA SDK Toolkit required for proper device support and utilization.
             Falling back to OpenCL runtime.

Successfully initialized NVIDIA CUDA library.

Failed to initialize NVIDIA RTC library.

* Device #2: CUDA SDK Toolkit not installed or incorrectly installed.
             CUDA SDK Toolkit required for proper device support and utilization.
             Falling back to OpenCL runtime.

Successfully initialized NVIDIA CUDA library.

Failed to initialize NVIDIA RTC library.

* Device #3: CUDA SDK Toolkit not installed or incorrectly installed.
             CUDA SDK Toolkit required for proper device support and utilization.
             Falling back to OpenCL runtime.

Successfully initialized NVIDIA CUDA library.

Failed to initialize NVIDIA RTC library.

* Device #4: CUDA SDK Toolkit not installed or incorrectly installed.
             CUDA SDK Toolkit required for proper device support and utilization.
             Falling back to OpenCL runtime.

Successfully initialized NVIDIA CUDA library.

Failed to initialize NVIDIA RTC library.

* Device #5: CUDA SDK Toolkit not installed or incorrectly installed.
             CUDA SDK Toolkit required for proper device support and utilization.
             Falling back to OpenCL runtime.

Successfully initialized NVIDIA CUDA library.

Failed to initialize NVIDIA RTC library.

* Device #6: CUDA SDK Toolkit not installed or incorrectly installed.
             CUDA SDK Toolkit required for proper device support and utilization.
             Falling back to OpenCL runtime.

Successfully initialized NVIDIA CUDA library.

Failed to initialize NVIDIA RTC library.

* Device #7: CUDA SDK Toolkit not installed or incorrectly installed.
             CUDA SDK Toolkit required for proper device support and utilization.
             Falling back to OpenCL runtime.

Successfully initialized NVIDIA CUDA library.

Failed to initialize NVIDIA RTC library.

* Device #8: CUDA SDK Toolkit not installed or incorrectly installed.
             CUDA SDK Toolkit required for proper device support and utilization.
             Falling back to OpenCL runtime.

OpenCL API (OpenCL 3.0 CUDA 12.0.151) - Platform #1 NVIDIA Corporation]
========================================================================
* Device #1: NVIDIA A40, 45184/45449 MB (11362 MB allocatable), 84MCU
* Device #2: NVIDIA A40, 45184/45449 MB (11362 MB allocatable), 84MCU
* Device #3: NVIDIA A40, 45184/45449 MB (11362 MB allocatable), 84MCU
* Device #4: NVIDIA A40, 45184/45449 MB (11362 MB allocatable), 84MCU
* Device #5: NVIDIA A40, 45184/45449 MB (11362 MB allocatable), 84MCU
* Device #6: NVIDIA A40, 45184/45449 MB (11362 MB allocatable), 84MCU
* Device #7: NVIDIA A40, 45184/45449 MB (11362 MB allocatable), 84MCU
* Device #8: NVIDIA A40, 45184/45449 MB (11362 MB allocatable), 84MCU

OpenCL API (OpenCL 2.0 pocl 1.8  Linux, None+Asserts, RELOC, LLVM 11.1.0, SLEEF, DISTRO, POCL_DEBUG) - Platform #2 The pocl project]
=====================================================================================================================================
* Device #9: pthread-Intel(R) Xeon(R) CPU E5-2630 v2 @ 2.60GHz, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 65339.2 MH/s (21.47ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#2.........: 65347.4 MH/s (21.47ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#3.........: 65359.1 MH/s (21.47ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#4.........: 65358.2 MH/s (21.47ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#5.........: 65346.4 MH/s (21.47ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#6.........: 65349.5 MH/s (21.47ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#7.........: 65331.0 MH/s (21.47ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#8.........: 65355.6 MH/s (21.47ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   522.8 GH/s

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........: 21190.4 MH/s (66.36ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#2.........: 21192.0 MH/s (66.36ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#3.........: 21188.5 MH/s (66.36ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#4.........: 21189.6 MH/s (66.36ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#5.........: 21189.3 MH/s (66.36ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#6.........: 21190.5 MH/s (66.36ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#7.........: 21187.5 MH/s (66.37ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#8.........: 21176.1 MH/s (66.37ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   169.5 GH/s

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  9143.5 MH/s (76.9s) @ Accel:64 Loops:512 Thr:256 Vec:1
Speed.#2.........:  9144.7 MH/s (76.9s) @ Accel:64 Loops:512 Thr:256 Vec:1
Speed.#3.........:  9143.4 MH/s (76.91ms) @ Accel:64 Loops:512 Thr:256 Vec:1
Speed.#4.........:  9143.4 MH/s (76.91ms) @ Accel:64 Loops:512 Thr:256 Vec:1
Speed.#5.........:  9143.6 MH/s (76.9s) @ Accel:64 Loops:512 Thr:256 Vec:1
Speed.#6.........:  9144.0 MH/s (76.9s) @ Accel:64 Loops:512 Thr:256 Vec:1
Speed.#7.........:  9143.8 MH/s (76.9s) @ Accel:64 Loops:512 Thr:256 Vec:1
Speed.#8.........:  9138.6 MH/s (76.92ms) @ Accel:64 Loops:512 Thr:256 Vec:1
Speed.#*.........: 73144.9 MH/s

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  2692.0 MH/s (65.3s) @ Accel:64 Loops:128 Thr:256 Vec:1
Speed.#2.........:  2692.0 MH/s (65.29ms) @ Accel:64 Loops:128 Thr:256 Vec:1
Speed.#3.........:  2692.1 MH/s (65.3s) @ Accel:64 Loops:128 Thr:256 Vec:1
Speed.#4.........:  2691.6 MH/s (65.3s) @ Accel:64 Loops:128 Thr:256 Vec:1
Speed.#5.........:  2691.7 MH/s (65.3s) @ Accel:64 Loops:128 Thr:256 Vec:1
Speed.#6.........:  2691.8 MH/s (65.3s) @ Accel:64 Loops:128 Thr:256 Vec:1
Speed.#7.........:  2691.9 MH/s (65.3s) @ Accel:64 Loops:128 Thr:256 Vec:1
Speed.#8.........:  2690.7 MH/s (65.3s) @ Accel:64 Loops:128 Thr:256 Vec:1
Speed.#*.........: 21533.7 MH/s

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:  1081.3 kH/s (79.02ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#2.........:  1082.6 kH/s (78.93ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#3.........:  1081.9 kH/s (78.99ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#4.........:  1082.6 kH/s (78.93ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#5.........:  1080.7 kH/s (79.06ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#6.........:  1081.4 kH/s (79.01ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#7.........:  1072.4 kH/s (78.95ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#8.........:  1082.2 kH/s (78.94ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#*.........:  8645.2 kH/s

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:   110.7 GH/s (12.58ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#2.........:   110.8 GH/s (12.58ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#3.........:   110.7 GH/s (12.58ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#4.........:   110.8 GH/s (12.58ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#5.........:   110.7 GH/s (12.58ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#6.........:   110.7 GH/s (12.59ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#7.........:   110.7 GH/s (12.59ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#8.........:   110.5 GH/s (12.59ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   885.7 GH/s

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........: 63790.6 MH/s (21.96ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#2.........: 63805.9 MH/s (21.96ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#3.........: 63791.6 MH/s (21.96ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#4.........: 63807.6 MH/s (21.96ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#5.........: 63788.2 MH/s (21.96ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#6.........: 63786.4 MH/s (21.96ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#7.........: 63806.0 MH/s (21.96ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#8.........: 63769.2 MH/s (21.96ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   510.3 GH/s

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 67077.6 MH/s (20.87ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#2.........: 67085.3 MH/s (20.87ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#3.........: 67075.5 MH/s (20.87ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#4.........: 67094.4 MH/s (20.87ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#5.........: 67037.7 MH/s (20.87ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#6.........: 67040.3 MH/s (20.87ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#7.........: 67051.9 MH/s (20.87ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#8.........: 66968.7 MH/s (20.88ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   536.4 GH/s

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  4865.3 MH/s (72.26ms) @ Accel:64 Loops:256 Thr:256 Vec:1
Speed.#2.........:  4871.6 MH/s (72.17ms) @ Accel:64 Loops:256 Thr:256 Vec:1
Speed.#3.........:  4871.8 MH/s (72.17ms) @ Accel:64 Loops:256 Thr:256 Vec:1
Speed.#4.........:  4871.1 MH/s (72.17ms) @ Accel:64 Loops:256 Thr:256 Vec:1
Speed.#5.........:  4871.3 MH/s (72.17ms) @ Accel:64 Loops:256 Thr:256 Vec:1
Speed.#6.........:  4861.7 MH/s (72.31ms) @ Accel:64 Loops:256 Thr:256 Vec:1
Speed.#7.........:  4868.6 MH/s (72.21ms) @ Accel:64 Loops:256 Thr:256 Vec:1
Speed.#8.........:  4869.5 MH/s (72.17ms) @ Accel:64 Loops:256 Thr:256 Vec:1
Speed.#*.........: 38951.0 MH/s

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:  2611.1 MH/s (67.35ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#2.........:  2611.1 MH/s (67.35ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#3.........:  2610.4 MH/s (67.37ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#4.........:  2611.6 MH/s (67.35ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#5.........:  2611.0 MH/s (67.35ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#6.........:  2611.3 MH/s (67.35ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#7.........:  2611.0 MH/s (67.35ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#8.........:  2609.8 MH/s (67.36ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#*.........: 20887.4 MH/s

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........: 27584.9 kH/s (43.66ms) @ Accel:64 Loops:1000 Thr:256 Vec:1
Speed.#2.........: 27594.8 kH/s (43.66ms) @ Accel:64 Loops:1000 Thr:256 Vec:1
Speed.#3.........: 27538.1 kH/s (43.69ms) @ Accel:64 Loops:1000 Thr:256 Vec:1
Speed.#4.........: 27571.0 kH/s (43.65ms) @ Accel:64 Loops:1000 Thr:256 Vec:1
Speed.#5.........: 27547.4 kH/s (43.67ms) @ Accel:64 Loops:1000 Thr:256 Vec:1
Speed.#6.........: 27557.7 kH/s (43.66ms) @ Accel:64 Loops:1000 Thr:256 Vec:1
Speed.#7.........: 27530.0 kH/s (43.68ms) @ Accel:64 Loops:1000 Thr:256 Vec:1
Speed.#8.........: 26547.3 kH/s (43.71ms) @ Accel:64 Loops:1000 Thr:256 Vec:1
Speed.#*.........:   219.5 MH/s

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    71689 H/s (76.37ms) @ Accel:512 Loops:32 Thr:11 Vec:1
Speed.#2.........:    71687 H/s (76.37ms) @ Accel:512 Loops:32 Thr:11 Vec:1
Speed.#3.........:    71720 H/s (76.37ms) @ Accel:512 Loops:32 Thr:11 Vec:1
Speed.#4.........:    71722 H/s (76.37ms) @ Accel:512 Loops:32 Thr:11 Vec:1
Speed.#5.........:    71707 H/s (76.38ms) @ Accel:512 Loops:32 Thr:11 Vec:1
Speed.#6.........:    71734 H/s (76.38ms) @ Accel:512 Loops:32 Thr:11 Vec:1
Speed.#7.........:    71640 H/s (76.38ms) @ Accel:512 Loops:32 Thr:11 Vec:1
Speed.#8.........:    71648 H/s (76.38ms) @ Accel:512 Loops:32 Thr:11 Vec:1
Speed.#*.........:   573.5 kH/s

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:   385.5 kH/s (67.45ms) @ Accel:4096 Loops:1024 Thr:32 Vec:1
Speed.#2.........:   383.3 kH/s (67.84ms) @ Accel:4096 Loops:1024 Thr:32 Vec:1
Speed.#3.........:   383.4 kH/s (67.81ms) @ Accel:4096 Loops:1024 Thr:32 Vec:1
Speed.#4.........:   382.0 kH/s (68.07ms) @ Accel:4096 Loops:1024 Thr:32 Vec:1
Speed.#5.........:   379.3 kH/s (68.57ms) @ Accel:4096 Loops:1024 Thr:32 Vec:1
Speed.#6.........:   385.8 kH/s (67.39ms) @ Accel:4096 Loops:1024 Thr:32 Vec:1
Speed.#7.........:   382.6 kH/s (67.96ms) @ Accel:4096 Loops:1024 Thr:32 Vec:1
Speed.#8.........:   381.2 kH/s (68.03ms) @ Accel:4096 Loops:1024 Thr:32 Vec:1
Speed.#*.........:  3063.2 kH/s

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:  1390.0 MH/s (63.25ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#2.........:  1390.0 MH/s (63.26ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#3.........:  1389.8 MH/s (63.27ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#4.........:  1390.1 MH/s (63.25ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#5.........:  1390.1 MH/s (63.25ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#6.........:  1389.9 MH/s (63.26ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#7.........:  1389.6 MH/s (63.28ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#8.........:  1389.5 MH/s (63.28ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#*.........: 11119.1 MH/s

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:  1360.9 MH/s (64.61ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#2.........:  1360.9 MH/s (64.61ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#3.........:  1360.9 MH/s (64.62ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#4.........:  1361.1 MH/s (64.61ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#5.........:  1361.0 MH/s (64.61ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#6.........:  1360.9 MH/s (64.61ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#7.........:  1360.2 MH/s (64.64ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#8.........:  1360.2 MH/s (64.65ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#*.........: 10886.2 MH/s

---------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1) Iterations: 23999]
---------------------------------------------------------------

Speed.#1.........:   183.4 kH/s (77.93ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#2.........:   183.4 kH/s (77.94ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#3.........:   183.4 kH/s (77.95ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#4.........:   183.4 kH/s (77.93ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#5.........:   183.4 kH/s (77.93ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#6.........:   183.1 kH/s (77.93ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#7.........:   183.4 kH/s (77.93ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#8.........:   183.4 kH/s (77.94ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#*.........:  1467.1 kH/s

---------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2) Iterations: 12899]
---------------------------------------------------------------

Speed.#1.........:   105.3 kH/s (62.64ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#2.........:   105.3 kH/s (62.64ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#3.........:   105.3 kH/s (62.65ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#4.........:   105.3 kH/s (62.65ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#5.........:   104.6 kH/s (62.63ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#6.........:   105.3 kH/s (62.65ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#7.........:   105.3 kH/s (62.63ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#8.........:   105.3 kH/s (62.64ms) @ Accel:4 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   841.7 kH/s

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:  1314.9 kH/s (60.88ms) @ Accel:256 Loops:63 Thr:64 Vec:1
Speed.#2.........:  1314.6 kH/s (60.9s) @ Accel:256 Loops:63 Thr:64 Vec:1
Speed.#3.........:  1314.9 kH/s (60.89ms) @ Accel:256 Loops:63 Thr:64 Vec:1
Speed.#4.........:  1314.9 kH/s (60.88ms) @ Accel:256 Loops:63 Thr:64 Vec:1
Speed.#5.........:  1315.0 kH/s (60.88ms) @ Accel:256 Loops:63 Thr:64 Vec:1
Speed.#6.........:  1311.9 kH/s (60.88ms) @ Accel:256 Loops:63 Thr:64 Vec:1
Speed.#7.........:  1308.2 kH/s (60.87ms) @ Accel:256 Loops:63 Thr:64 Vec:1
Speed.#8.........:  1314.8 kH/s (60.88ms) @ Accel:256 Loops:63 Thr:64 Vec:1
Speed.#*.........: 10509.2 kH/s

---------------------------------------------
* Hash-Mode 11600 (7-Zip) Iterations: 16384]
---------------------------------------------

Speed.#1.........:   827.1 kH/s (77.09ms) @ Accel:32 Loops:4096 Thr:128 Vec:1
Speed.#2.........:   825.5 kH/s (76.63ms) @ Accel:32 Loops:4096 Thr:128 Vec:1
Speed.#3.........:   826.9 kH/s (76.75ms) @ Accel:32 Loops:4096 Thr:128 Vec:1
Speed.#4.........:   835.2 kH/s (76.18ms) @ Accel:32 Loops:4096 Thr:128 Vec:1
Speed.#5.........:   835.7 kH/s (76.23ms) @ Accel:32 Loops:4096 Thr:128 Vec:1
Speed.#6.........:   825.9 kH/s (77.27ms) @ Accel:32 Loops:4096 Thr:128 Vec:1
Speed.#7.........:   827.1 kH/s (76.97ms) @ Accel:32 Loops:4096 Thr:128 Vec:1
Speed.#8.........:   821.6 kH/s (77.24ms) @ Accel:32 Loops:4096 Thr:128 Vec:1
Speed.#*.........:  6625.1 kH/s

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) Iterations: 262144]
------------------------------------------------

Speed.#1.........:    25375 H/s (6.58ms) @ Accel:64 Loops:16384 Thr:32 Vec:1
Speed.#2.........:    25601 H/s (6.52ms) @ Accel:64 Loops:16384 Thr:32 Vec:1
Speed.#3.........:    25572 H/s (6.52ms) @ Accel:64 Loops:16384 Thr:32 Vec:1
Speed.#4.........:    25571 H/s (6.52ms) @ Accel:64 Loops:16384 Thr:32 Vec:1
Speed.#5.........:    25590 H/s (6.52ms) @ Accel:64 Loops:16384 Thr:32 Vec:1
Speed.#6.........:    25378 H/s (6.58ms) @ Accel:64 Loops:16384 Thr:32 Vec:1
Speed.#7.........:    25606 H/s (6.52ms) @ Accel:64 Loops:16384 Thr:32 Vec:1
Speed.#8.........:    24461 H/s (6.52ms) @ Accel:64 Loops:16384 Thr:32 Vec:1
Speed.#*.........:   203.2 kH/s

--------------------------------------------
* Hash-Mode 13000 (RAR5) Iterations: 32799]
--------------------------------------------

Speed.#1.........:   115.5 kH/s (90.18ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#2.........:   115.5 kH/s (90.17ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#3.........:   115.5 kH/s (90.18ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#4.........:   115.5 kH/s (90.17ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#5.........:   115.5 kH/s (90.17ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#6.........:   115.5 kH/s (90.17ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#7.........:   115.3 kH/s (90.17ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#8.........:   115.4 kH/s (90.21ms) @ Accel:16 Loops:1024 Thr:256 Vec:1
Speed.#*.........:   923.6 kH/s

-----------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit) Iterations: 1999]
-----------------------------------------------------------------------

Speed.#1.........:   804.8 kH/s (48.64ms) @ Accel:32 Loops:128 Thr:256 Vec:1
Speed.#2.........:   804.9 kH/s (48.64ms) @ Accel:32 Loops:128 Thr:256 Vec:1
Speed.#3.........:   804.5 kH/s (48.65ms) @ Accel:32 Loops:128 Thr:256 Vec:1
Speed.#4.........:   804.8 kH/s (48.64ms) @ Accel:32 Loops:128 Thr:256 Vec:1
Speed.#5.........:   804.8 kH/s (48.64ms) @ Accel:32 Loops:128 Thr:256 Vec:1
Speed.#6.........:   804.8 kH/s (48.64ms) @ Accel:32 Loops:128 Thr:256 Vec:1
Speed.#7.........:   802.8 kH/s (48.64ms) @ Accel:32 Loops:128 Thr:256 Vec:1
Speed.#8.........:   797.6 kH/s (48.64ms) @ Accel:32 Loops:128 Thr:256 Vec:1
Speed.#*.........:  6429.0 kH/s

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:   134.5 kH/s (53.21ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#2.........:   134.5 kH/s (53.21ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#3.........:   134.2 kH/s (53.24ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#4.........:   134.5 kH/s (53.21ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#5.........:   134.5 kH/s (53.22ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#6.........:   134.5 kH/s (53.22ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#7.........:   134.3 kH/s (53.28ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#8.........:   134.3 kH/s (53.28ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#*.........:  1075.3 kH/s

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  7215.3 kH/s (60.52ms) @ Accel:64 Loops:249 Thr:256 Vec:1
Speed.#2.........:  7215.2 kH/s (60.52ms) @ Accel:64 Loops:249 Thr:256 Vec:1
Speed.#3.........:  7208.5 kH/s (60.59ms) @ Accel:64 Loops:249 Thr:256 Vec:1
Speed.#4.........:  7216.0 kH/s (60.51ms) @ Accel:64 Loops:249 Thr:256 Vec:1
Speed.#5.........:  7215.1 kH/s (60.52ms) @ Accel:64 Loops:249 Thr:256 Vec:1
Speed.#6.........:  7214.8 kH/s (60.52ms) @ Accel:64 Loops:249 Thr:256 Vec:1
Speed.#7.........:  7215.9 kH/s (60.51ms) @ Accel:64 Loops:249 Thr:256 Vec:1
Speed.#8.........:  7112.4 kH/s (60.53ms) @ Accel:64 Loops:249 Thr:256 Vec:1
Speed.#*.........: 57613.3 kH/s

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:    13651 H/s (49.0s) @ Accel:4096 Loops:512 Thr:64 Vec:1
Speed.#2.........:    13651 H/s (48.99ms) @ Accel:4096 Loops:512 Thr:64 Vec:1
Speed.#3.........:    13651 H/s (49.0s) @ Accel:4096 Loops:512 Thr:64 Vec:1
Speed.#4.........:    13652 H/s (48.99ms) @ Accel:4096 Loops:512 Thr:64 Vec:1
Speed.#5.........:    13652 H/s (49.0s) @ Accel:4096 Loops:512 Thr:64 Vec:1
Speed.#6.........:    13652 H/s (48.99ms) @ Accel:4096 Loops:512 Thr:64 Vec:1
Speed.#7.........:    13651 H/s (49.0s) @ Accel:4096 Loops:512 Thr:64 Vec:1
Speed.#8.........:    13652 H/s (49.0s) @ Accel:4096 Loops:512 Thr:64 Vec:1
Speed.#*.........:   109.2 kH/s

Started: Fri Aug  4 04:32:02 2023
2K
Stopped: Fri Aug  4 04:43:09 2023
```

