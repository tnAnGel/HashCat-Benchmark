# NVIDIA A100 80GB

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA A100-SXM4-80GB
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [laluka](https://gist.github.com/laluka/1531f3bc655e4db3d3f0bf708af5f8ab)
- **Примечание / Note:** прогон на 8x NVIDIA A100-SXM4-80GB (все устройства одной модели); в таблице ниже приведены значения Speed.#1 — одна карта.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 67375.4 MH/s |
| 100 | SHA1 | 21877.0 MH/s |
| 1400 | SHA2-256 | 9468.5 MH/s |
| 1700 | SHA2-512 | 3183.0 MH/s |
| 1000 | NTLM | 114.2 GH/s |
| 3200 | bcrypt | 165.1 kH/s |
| 1800 | sha512crypt | 522.5 kH/s |
| 500 | md5crypt | 28662.0 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 1120.0 kH/s |
| 7500 | Kerberos AS-REQ (23) | 2132.4 MH/s |
| 13100 | Kerberos TGS-REP (23) | 1970.8 MH/s |
| 11300 | Bitcoin wallet.dat | 14544 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 822.6 kH/s |

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
* Device #9: WARNING! Kernel exec timeout is not disabled.
             This may cause "CL_OUT_OF_RESOURCES" or related errors.
             To disable the timeout, see: https://hashcat.net/q/timeoutpatch
CUDA API (CUDA 12.2)
====================
* Device #1: NVIDIA A100-SXM4-80GB, 80596/81228 MB, 108MCU
* Device #2: NVIDIA A100-SXM4-80GB, 80805/81228 MB, 108MCU
* Device #3: NVIDIA A100-SXM4-80GB, 80805/81228 MB, 108MCU
* Device #4: NVIDIA A100-SXM4-80GB, 80805/81228 MB, 108MCU
* Device #5: NVIDIA A100-SXM4-80GB, 80805/81228 MB, 108MCU
* Device #6: NVIDIA A100-SXM4-80GB, 80805/81228 MB, 108MCU
* Device #7: NVIDIA A100-SXM4-80GB, 80805/81228 MB, 108MCU
* Device #8: NVIDIA A100-SXM4-80GB, 80805/81228 MB, 108MCU

OpenCL API (OpenCL 3.0 CUDA 12.2.147) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #9: NVIDIA A100-SXM4-80GB, skipped
* Device #10: NVIDIA A100-SXM4-80GB, skipped
* Device #11: NVIDIA A100-SXM4-80GB, skipped
* Device #12: NVIDIA A100-SXM4-80GB, skipped
* Device #13: NVIDIA A100-SXM4-80GB, skipped
* Device #14: NVIDIA A100-SXM4-80GB, skipped
* Device #15: NVIDIA A100-SXM4-80GB, skipped
* Device #16: NVIDIA A100-SXM4-80GB, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 67375.4 MH/s (53.26ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#2.........: 67550.8 MH/s (53.10ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#3.........: 67555.8 MH/s (53.03ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#4.........: 67491.6 MH/s (53.07ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#5.........: 67414.8 MH/s (53.04ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#6.........: 67233.8 MH/s (53.37ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#7.........: 67578.3 MH/s (53.07ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#8.........: 66932.1 MH/s (53.56ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#*.........:   539.1 GH/s

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........: 21877.0 MH/s (82.14ms) @ Accel:64 Loops:1024 Thr:256 Vec:1
Speed.#2.........: 21794.3 MH/s (41.06ms) @ Accel:32 Loops:512 Thr:512 Vec:1
Speed.#3.........: 21823.0 MH/s (41.02ms) @ Accel:32 Loops:512 Thr:512 Vec:1
Speed.#4.........: 21811.7 MH/s (41.04ms) @ Accel:32 Loops:512 Thr:512 Vec:1
Speed.#5.........: 21830.4 MH/s (41.03ms) @ Accel:32 Loops:512 Thr:512 Vec:1
Speed.#6.........: 21736.5 MH/s (41.23ms) @ Accel:32 Loops:512 Thr:512 Vec:1
Speed.#7.........: 21818.1 MH/s (41.05ms) @ Accel:32 Loops:512 Thr:512 Vec:1
Speed.#8.........: 21584.8 MH/s (41.42ms) @ Accel:32 Loops:512 Thr:512 Vec:1
Speed.#*.........:   174.3 GH/s

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  9468.5 MH/s (95.00ms) @ Accel:16 Loops:1024 Thr:512 Vec:1
Speed.#2.........:  9486.9 MH/s (94.89ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#3.........:  9501.5 MH/s (94.79ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#4.........:  9499.8 MH/s (94.86ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#5.........:  9501.9 MH/s (94.80ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#6.........:  9463.2 MH/s (95.31ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#7.........:  9500.2 MH/s (94.84ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#8.........:  9412.7 MH/s (95.71ms) @ Accel:8 Loops:1024 Thr:1024 Vec:1
Speed.#*.........: 75834.7 MH/s

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  3183.0 MH/s (70.59ms) @ Accel:16 Loops:512 Thr:256 Vec:1
Speed.#2.........:  3181.3 MH/s (70.73ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#3.........:  3179.3 MH/s (70.63ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#4.........:  3181.7 MH/s (70.74ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#5.........:  3178.2 MH/s (70.70ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#6.........:  3170.2 MH/s (71.01ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#7.........:  3182.4 MH/s (70.64ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#8.........:  3162.8 MH/s (71.21ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#*.........: 25419.0 MH/s

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:  1120.0 kH/s (48.83ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#2.........:  1118.8 kH/s (48.77ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#3.........:  1120.9 kH/s (48.72ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#4.........:  1121.0 kH/s (48.77ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#5.........:  1121.8 kH/s (48.73ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#6.........:  1115.1 kH/s (49.00ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#7.........:  1117.4 kH/s (48.88ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#8.........:  1111.8 kH/s (49.19ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#*.........:  8946.7 kH/s

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:   114.2 GH/s (31.18ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#2.........:   114.2 GH/s (31.11ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#3.........:   114.0 GH/s (31.09ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#4.........:   114.2 GH/s (31.11ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#5.........:   114.5 GH/s (31.09ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#6.........:   113.2 GH/s (31.26ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#7.........:   114.1 GH/s (31.10ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#8.........:   113.2 GH/s (31.38ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#*.........:   911.6 GH/s

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........: 64851.3 MH/s (13.64ms) @ Accel:256 Loops:1024 Thr:32 Vec:1
Speed.#2.........: 64837.7 MH/s (13.62ms) @ Accel:256 Loops:1024 Thr:32 Vec:1
Speed.#3.........: 65050.0 MH/s (13.61ms) @ Accel:256 Loops:1024 Thr:32 Vec:1
Speed.#4.........: 65091.4 MH/s (13.62ms) @ Accel:256 Loops:1024 Thr:32 Vec:1
Speed.#5.........: 64918.9 MH/s (13.61ms) @ Accel:256 Loops:1024 Thr:32 Vec:1
Speed.#6.........: 64826.0 MH/s (13.68ms) @ Accel:256 Loops:1024 Thr:32 Vec:1
Speed.#7.........: 64864.2 MH/s (13.62ms) @ Accel:256 Loops:1024 Thr:32 Vec:1
Speed.#8.........: 64199.1 MH/s (13.73ms) @ Accel:256 Loops:1024 Thr:32 Vec:1
Speed.#*.........:   518.6 GH/s

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 69233.8 MH/s (51.72ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
Speed.#2.........: 69991.5 MH/s (51.12ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#3.........: 69994.9 MH/s (51.07ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#4.........: 69994.8 MH/s (51.12ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#5.........: 70000.0 MH/s (51.07ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#6.........: 69617.6 MH/s (51.36ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#7.........: 70106.4 MH/s (51.10ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#8.........: 69312.7 MH/s (51.57ms) @ Accel:64 Loops:1024 Thr:512 Vec:1
Speed.#*.........:   558.3 GH/s

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  5036.8 MH/s (89.30ms) @ Accel:16 Loops:512 Thr:512 Vec:1
Speed.#2.........:  5050.8 MH/s (89.18ms) @ Accel:16 Loops:512 Thr:512 Vec:1
Speed.#3.........:  5047.8 MH/s (89.08ms) @ Accel:16 Loops:512 Thr:512 Vec:1
Speed.#4.........:  5055.0 MH/s (89.17ms) @ Accel:16 Loops:512 Thr:512 Vec:1
Speed.#5.........:  5053.4 MH/s (89.07ms) @ Accel:16 Loops:512 Thr:512 Vec:1
Speed.#6.........:  5033.6 MH/s (89.43ms) @ Accel:16 Loops:512 Thr:512 Vec:1
Speed.#7.........:  5051.5 MH/s (89.12ms) @ Accel:16 Loops:512 Thr:512 Vec:1
Speed.#8.........:  5015.3 MH/s (89.93ms) @ Accel:16 Loops:512 Thr:512 Vec:1
Speed.#*.........: 40344.1 MH/s

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:  2659.2 MH/s (84.51ms) @ Accel:64 Loops:1024 Thr:32 Vec:1
Speed.#2.........:  2667.9 MH/s (84.37ms) @ Accel:16 Loops:1024 Thr:128 Vec:1
Speed.#3.........:  2667.5 MH/s (84.34ms) @ Accel:16 Loops:1024 Thr:128 Vec:1
Speed.#4.........:  2667.9 MH/s (84.40ms) @ Accel:16 Loops:1024 Thr:128 Vec:1
Speed.#5.........:  2668.7 MH/s (84.33ms) @ Accel:16 Loops:1024 Thr:128 Vec:1
Speed.#6.........:  2661.2 MH/s (84.45ms) @ Accel:16 Loops:1024 Thr:128 Vec:1
Speed.#7.........:  2667.8 MH/s (84.35ms) @ Accel:16 Loops:1024 Thr:128 Vec:1
Speed.#8.........:  2647.9 MH/s (85.07ms) @ Accel:16 Loops:1024 Thr:128 Vec:1
Speed.#*.........: 21308.0 MH/s

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........: 28662.0 kH/s (55.54ms) @ Accel:32 Loops:1000 Thr:512 Vec:1
Speed.#2.........: 28757.4 kH/s (55.46ms) @ Accel:64 Loops:500 Thr:512 Vec:1
Speed.#3.........: 28715.4 kH/s (55.40ms) @ Accel:64 Loops:500 Thr:512 Vec:1
Speed.#4.........: 28653.9 kH/s (55.46ms) @ Accel:64 Loops:500 Thr:512 Vec:1
Speed.#5.........: 28691.8 kH/s (55.41ms) @ Accel:64 Loops:500 Thr:512 Vec:1
Speed.#6.........: 28602.0 kH/s (55.73ms) @ Accel:64 Loops:500 Thr:512 Vec:1
Speed.#7.........: 28655.9 kH/s (55.56ms) @ Accel:64 Loops:500 Thr:512 Vec:1
Speed.#8.........: 28514.7 kH/s (55.96ms) @ Accel:64 Loops:500 Thr:512 Vec:1
Speed.#*.........:   229.3 MH/s

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:   165.1 kH/s (50.25ms) @ Accel:2 Loops:32 Thr:40 Vec:1
Speed.#2.........:   164.9 kH/s (50.23ms) @ Accel:2 Loops:32 Thr:40 Vec:1
Speed.#3.........:   146.1 kH/s (50.24ms) @ Accel:2 Loops:32 Thr:40 Vec:1
Speed.#4.........:   141.6 kH/s (50.24ms) @ Accel:2 Loops:32 Thr:40 Vec:1
Speed.#5.........:   139.8 kH/s (50.23ms) @ Accel:2 Loops:32 Thr:40 Vec:1
Speed.#6.........:   164.9 kH/s (50.35ms) @ Accel:2 Loops:32 Thr:40 Vec:1
Speed.#7.........:   164.6 kH/s (50.35ms) @ Accel:2 Loops:32 Thr:40 Vec:1
Speed.#8.........:   163.6 kH/s (50.67ms) @ Accel:2 Loops:32 Thr:40 Vec:1
Speed.#*.........:  1250.6 kH/s

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:   522.5 kH/s (49.41ms) @ Accel:2048 Loops:256 Thr:256 Vec:1
Speed.#2.........:   522.8 kH/s (49.31ms) @ Accel:2048 Loops:256 Thr:256 Vec:1
Speed.#3.........:   524.3 kH/s (49.30ms) @ Accel:2048 Loops:256 Thr:256 Vec:1
Speed.#4.........:   522.7 kH/s (49.32ms) @ Accel:2048 Loops:256 Thr:256 Vec:1
Speed.#5.........:   523.8 kH/s (49.30ms) @ Accel:2048 Loops:256 Thr:256 Vec:1
Speed.#6.........:   522.2 kH/s (49.51ms) @ Accel:2048 Loops:256 Thr:256 Vec:1
Speed.#7.........:   522.7 kH/s (49.38ms) @ Accel:2048 Loops:256 Thr:256 Vec:1
Speed.#8.........:   519.7 kH/s (49.70ms) @ Accel:2048 Loops:256 Thr:256 Vec:1
Speed.#*.........:  4180.7 kH/s

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:  2132.4 MH/s (52.61ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#2.........:  2132.6 MH/s (52.52ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#3.........:  2137.5 MH/s (52.46ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#4.........:  2134.8 MH/s (52.52ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#5.........:  2140.7 MH/s (52.46ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#6.........:  2136.8 MH/s (52.56ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#7.........:  2136.9 MH/s (52.49ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#8.........:  2119.2 MH/s (52.90ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#*.........: 17070.9 MH/s

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:  1970.8 MH/s (56.91ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#2.........:  1972.6 MH/s (56.81ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#3.........:  1979.5 MH/s (56.76ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#4.........:  1980.1 MH/s (56.80ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#5.........:  1976.3 MH/s (56.76ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#6.........:  1974.7 MH/s (56.91ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#7.........:  1972.7 MH/s (56.78ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#8.........:  1964.5 MH/s (57.25ms) @ Accel:256 Loops:128 Thr:32 Vec:1
Speed.#*.........: 15791.3 MH/s

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:   190.1 kH/s (48.08ms) @ Accel:4 Loops:1024 Thr:512 Vec:1
Speed.#2.........:   190.5 kH/s (49.21ms) @ Accel:16 Loops:256 Thr:512 Vec:1
Speed.#3.........:   190.5 kH/s (49.17ms) @ Accel:16 Loops:256 Thr:512 Vec:1
Speed.#4.........:   190.6 kH/s (49.18ms) @ Accel:16 Loops:256 Thr:512 Vec:1
Speed.#5.........:   190.5 kH/s (49.18ms) @ Accel:16 Loops:256 Thr:512 Vec:1
Speed.#6.........:   190.1 kH/s (49.31ms) @ Accel:16 Loops:256 Thr:512 Vec:1
Speed.#7.........:   190.3 kH/s (49.22ms) @ Accel:16 Loops:256 Thr:512 Vec:1
Speed.#8.........:   188.7 kH/s (49.66ms) @ Accel:16 Loops:256 Thr:512 Vec:1
Speed.#*.........:  1521.2 kH/s

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:   107.7 kH/s (78.48ms) @ Accel:2 Loops:1024 Thr:512 Vec:1
Speed.#2.........:   108.0 kH/s (78.37ms) @ Accel:2 Loops:1024 Thr:512 Vec:1
Speed.#3.........:   108.1 kH/s (78.31ms) @ Accel:2 Loops:1024 Thr:512 Vec:1
Speed.#4.........:   107.9 kH/s (78.32ms) @ Accel:2 Loops:1024 Thr:512 Vec:1
Speed.#5.........:   108.0 kH/s (78.33ms) @ Accel:2 Loops:1024 Thr:512 Vec:1
Speed.#6.........:   107.5 kH/s (78.67ms) @ Accel:2 Loops:1024 Thr:512 Vec:1
Speed.#7.........:   107.8 kH/s (78.51ms) @ Accel:2 Loops:1024 Thr:512 Vec:1
Speed.#8.........:   107.1 kH/s (79.01ms) @ Accel:2 Loops:1024 Thr:512 Vec:1
Speed.#*.........:   862.0 kH/s

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:  1348.8 kH/s (76.17ms) @ Accel:64 Loops:63 Thr:256 Vec:1
Speed.#2.........:  1349.0 kH/s (80.73ms) @ Accel:2 Loops:1023 Thr:512 Vec:1
Speed.#3.........:  1338.8 kH/s (80.69ms) @ Accel:2 Loops:1023 Thr:512 Vec:1
Speed.#4.........:  1337.1 kH/s (80.74ms) @ Accel:2 Loops:1023 Thr:512 Vec:1
Speed.#5.........:  1339.8 kH/s (80.70ms) @ Accel:2 Loops:1023 Thr:512 Vec:1
Speed.#6.........:  1342.8 kH/s (81.02ms) @ Accel:2 Loops:1023 Thr:512 Vec:1
Speed.#7.........:  1343.0 kH/s (80.96ms) @ Accel:2 Loops:1023 Thr:512 Vec:1
Speed.#8.........:  1338.4 kH/s (81.37ms) @ Accel:2 Loops:1023 Thr:512 Vec:1
Speed.#*.........: 10737.8 kH/s

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:  1124.4 kH/s (87.44ms) @ Accel:128 Loops:4096 Thr:32 Vec:1
Speed.#2.........:  1126.6 kH/s (87.42ms) @ Accel:128 Loops:4096 Thr:32 Vec:1
Speed.#3.........:  1102.2 kH/s (87.40ms) @ Accel:128 Loops:4096 Thr:32 Vec:1
Speed.#4.........:  1111.5 kH/s (87.42ms) @ Accel:128 Loops:4096 Thr:32 Vec:1
Speed.#5.........:  1131.5 kH/s (87.44ms) @ Accel:128 Loops:4096 Thr:32 Vec:1
Speed.#6.........:  1128.3 kH/s (87.76ms) @ Accel:128 Loops:4096 Thr:32 Vec:1
Speed.#7.........:  1139.2 kH/s (87.61ms) @ Accel:128 Loops:4096 Thr:32 Vec:1
Speed.#8.........:  1124.2 kH/s (88.13ms) @ Accel:128 Loops:4096 Thr:32 Vec:1
Speed.#*.........:  8987.9 kH/s

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:   122.9 kH/s (13.73ms) @ Accel:8 Loops:16384 Thr:256 Vec:1
Speed.#2.........:   124.6 kH/s (13.60ms) @ Accel:8 Loops:16384 Thr:256 Vec:1
Speed.#3.........:   123.5 kH/s (13.67ms) @ Accel:8 Loops:16384 Thr:256 Vec:1
Speed.#4.........:   123.8 kH/s (13.66ms) @ Accel:8 Loops:16384 Thr:256 Vec:1
Speed.#5.........:   123.8 kH/s (13.67ms) @ Accel:8 Loops:16384 Thr:256 Vec:1
Speed.#6.........:   124.8 kH/s (13.59ms) @ Accel:8 Loops:16384 Thr:256 Vec:1
Speed.#7.........:   124.0 kH/s (13.62ms) @ Accel:8 Loops:16384 Thr:256 Vec:1
Speed.#8.........:   122.8 kH/s (13.79ms) @ Accel:8 Loops:16384 Thr:256 Vec:1
Speed.#*.........:   990.2 kH/s

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:   119.5 kH/s (56.56ms) @ Accel:8 Loops:512 Thr:512 Vec:1
Speed.#2.........:   119.7 kH/s (56.55ms) @ Accel:4 Loops:512 Thr:1024 Vec:1
Speed.#3.........:   119.7 kH/s (56.51ms) @ Accel:4 Loops:512 Thr:1024 Vec:1
Speed.#4.........:   119.6 kH/s (56.56ms) @ Accel:4 Loops:512 Thr:1024 Vec:1
Speed.#5.........:   119.7 kH/s (56.51ms) @ Accel:4 Loops:512 Thr:1024 Vec:1
Speed.#6.........:   119.6 kH/s (56.63ms) @ Accel:4 Loops:512 Thr:1024 Vec:1
Speed.#7.........:   119.6 kH/s (56.53ms) @ Accel:4 Loops:512 Thr:1024 Vec:1
Speed.#8.........:   118.6 kH/s (57.03ms) @ Accel:4 Loops:512 Thr:1024 Vec:1
Speed.#*.........:   955.9 kH/s

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:   822.6 kH/s (59.87ms) @ Accel:16 Loops:128 Thr:512 Vec:1
Speed.#2.........:   824.5 kH/s (59.76ms) @ Accel:8 Loops:256 Thr:512 Vec:1
Speed.#3.........:   825.3 kH/s (59.71ms) @ Accel:8 Loops:256 Thr:512 Vec:1
Speed.#4.........:   824.2 kH/s (59.76ms) @ Accel:8 Loops:256 Thr:512 Vec:1
Speed.#5.........:   825.6 kH/s (59.71ms) @ Accel:8 Loops:256 Thr:512 Vec:1
Speed.#6.........:   823.3 kH/s (59.88ms) @ Accel:8 Loops:256 Thr:512 Vec:1
Speed.#7.........:   825.0 kH/s (59.79ms) @ Accel:8 Loops:256 Thr:512 Vec:1
Speed.#8.........:   817.3 kH/s (60.29ms) @ Accel:8 Loops:256 Thr:512 Vec:1
Speed.#*.........:  6587.7 kH/s

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:   139.2 kH/s (65.83ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#2.........:   139.6 kH/s (65.71ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#3.........:   139.6 kH/s (65.66ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#4.........:   139.5 kH/s (65.68ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#5.........:   139.6 kH/s (65.67ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#6.........:   139.1 kH/s (65.96ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#7.........:   139.3 kH/s (65.80ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#8.........:   138.5 kH/s (66.24ms) @ Accel:8 Loops:1024 Thr:256 Vec:1
Speed.#*.........:  1114.3 kH/s

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  7449.2 kH/s (55.88ms) @ Accel:8 Loops:499 Thr:512 Vec:1
Speed.#2.........:  7535.0 kH/s (37.27ms) @ Accel:16 Loops:249 Thr:512 Vec:1
Speed.#3.........:  7521.6 kH/s (37.25ms) @ Accel:16 Loops:249 Thr:512 Vec:1
Speed.#4.........:  7520.4 kH/s (37.26ms) @ Accel:16 Loops:249 Thr:512 Vec:1
Speed.#5.........:  7540.3 kH/s (37.24ms) @ Accel:16 Loops:249 Thr:512 Vec:1
Speed.#6.........:  7509.5 kH/s (37.44ms) @ Accel:16 Loops:249 Thr:512 Vec:1
Speed.#7.........:  7537.9 kH/s (37.26ms) @ Accel:16 Loops:249 Thr:512 Vec:1
Speed.#8.........:  7468.7 kH/s (37.60ms) @ Accel:16 Loops:249 Thr:512 Vec:1
Speed.#*.........: 60082.7 kH/s

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:    14544 H/s (77.34ms) @ Accel:8 Loops:512 Thr:512 Vec:1
Speed.#2.........:    14564 H/s (77.18ms) @ Accel:32 Loops:256 Thr:256 Vec:1
Speed.#3.........:    14584 H/s (77.12ms) @ Accel:32 Loops:256 Thr:256 Vec:1
Speed.#4.........:    14571 H/s (77.17ms) @ Accel:32 Loops:256 Thr:256 Vec:1
Speed.#5.........:    14590 H/s (77.13ms) @ Accel:32 Loops:256 Thr:256 Vec:1
Speed.#6.........:    14545 H/s (77.30ms) @ Accel:32 Loops:256 Thr:256 Vec:1
Speed.#7.........:    14581 H/s (77.15ms) @ Accel:32 Loops:256 Thr:256 Vec:1
Speed.#8.........:    14457 H/s (77.80ms) @ Accel:32 Loops:256 Thr:256 Vec:1
Speed.#*.........:   116.4 kH/s

Started: Sun Jan 21 12:58:48 2024
Stopped: Sun Jan 21 13:08:43 2024
```
