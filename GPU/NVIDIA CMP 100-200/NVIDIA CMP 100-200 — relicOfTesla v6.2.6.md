# NVIDIA CMP 100-200

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA CMP 100-200
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [relicOfTesla](https://hashcat.net/forum/thread-13625.html)
- **Особенности прогона / Run options:** в треде два прогона одной и той же карты — через CUDA (`--backend-devices=1`, `Speed.#1`) и через OpenCL (`--backend-devices=7`, `Speed.#7`); в таблице приведён CUDA-прогон

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 37163.9 MH/s |
| 100 | SHA1 | 12793.5 MH/s |
| 1400 | SHA2-256 | 5718.0 MH/s |
| 1700 | SHA2-512 | 1781.9 MH/s |
| 1000 | NTLM | 58118.1 MH/s |
| 3200 | bcrypt | 52036 H/s |
| 1800 | sha512crypt | 300.5 kH/s |
| 500 | md5crypt | 14660.7 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 667.7 kH/s |
| 7500 | Kerberos AS-REQ (23) | 947.8 MH/s |
| 13100 | Kerberos TGS-REP (23) | 912.6 MH/s |
| 11300 | Bitcoin wallet.dat | 8497 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 515.9 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

### Прогон 1 — CUDA-бэкенд (`--backend-devices=1`)

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

CUDA API (CUDA 12.4)
====================
* Device #1: NVIDIA CMP 100-200, 5740/6016 MB, 68MCU
* Device #2: NVIDIA CMP 50HX, skipped
* Device #3: NVIDIA CMP 50HX, skipped
* Device #4: NVIDIA CMP 50HX, skipped
* Device #5: NVIDIA CMP 50HX, skipped
* Device #6: NVIDIA CMP 50HX, skipped

OpenCL API (OpenCL 3.0 CUDA 12.4.131) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #7: NVIDIA CMP 100-200, skipped
* Device #8: NVIDIA CMP 50HX, skipped
* Device #9: NVIDIA CMP 50HX, skipped
* Device #10: NVIDIA CMP 50HX, skipped
* Device #11: NVIDIA CMP 50HX, skipped
* Device #12: NVIDIA CMP 50HX, skipped

OpenCL API (OpenCL 1.2 ) - Platform #2 [Intel(R) Corporation]
=============================================================
* Device #13: Intel(R) HD Graphics 4600, skipped
* Device #14: Intel(R) Core(TM) i3-4360 CPU @ 3.70GHz, skipped

Benchmark relevant options:
===========================
* --backend-devices=1
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 37163.9 MH/s (14.10ms) @ Accel:256 Loops:128 Thr:256 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........: 12793.5 MH/s (21.30ms) @ Accel:256 Loops:128 Thr:128 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  5718.0 MH/s (48.78ms) @ Accel:32 Loops:256 Thr:512 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  1781.9 MH/s (76.78ms) @ Accel:16 Loops:256 Thr:512 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:  667.7 kH/s (50.65ms) @ Accel:16 Loops:512 Thr:256 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 58118.1 MH/s (8.58ms) @ Accel:2048 Loops:128 Thr:32 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........: 36447.2 MH/s (30.14ms) @ Accel:128 Loops:1024 Thr:128 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 38820.2 MH/s (13.55ms) @ Accel:512 Loops:128 Thr:128 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  2869.3 MH/s (48.62ms) @ Accel:32 Loops:256 Thr:256 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:  1496.4 MH/s (46.76ms) @ Accel:8 Loops:1024 Thr:128 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........: 14660.7 kH/s (59.02ms) @ Accel:128 Loops:250 Thr:512 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    52036 H/s (53.08ms) @ Accel:2 Loops:32 Thr:24 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:  300.5 kH/s (85.39ms) @ Accel:16384 Loops:256 Thr:32 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:  947.8 MH/s (74.25ms) @ Accel:256 Loops:128 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:  912.6 MH/s (76.95ms) @ Accel:256 Loops:128 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:  112.7 kH/s (51.99ms) @ Accel:16 Loops:256 Thr:512 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:    61015 H/s (89.63ms) @ Accel:16 Loops:128 Thr:512 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:  759.8 kH/s (86.92ms) @ Accel:64 Loops:31 Thr:512 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:  528.7 kH/s (91.19ms) @ Accel:32 Loops:4096 Thr:128 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:        0 H/s (0.00ms) @ Accel:32 Loops:4096 Thr:128 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    69591 H/s (61.59ms) @ Accel:16 Loops:128 Thr:1024 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:  515.9 kH/s (61.33ms) @ Accel:64 Loops:64 Thr:256 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    84524 H/s (67.79ms) @ Accel:32 Loops:128 Thr:512 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  4177.5 kH/s (48.32ms) @ Accel:16 Loops:124 Thr:1024 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:    8497 H/s (82.73ms) @ Accel:16 Loops:128 Thr:1024 Vec:1

Started: Sat May 30 23:05:52 2026
Stopped: Sat May 30 23:12:39 2026
```

### Прогон 2 — OpenCL-бэкенд (`--backend-devices=7`)

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

CUDA API (CUDA 12.4)
====================
* Device #1: NVIDIA CMP 100-200, skipped
* Device #2: NVIDIA CMP 50HX, skipped
* Device #3: NVIDIA CMP 50HX, skipped
* Device #4: NVIDIA CMP 50HX, skipped
* Device #5: NVIDIA CMP 50HX, skipped
* Device #6: NVIDIA CMP 50HX, skipped

OpenCL API (OpenCL 3.0 CUDA 12.4.131) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #7: NVIDIA CMP 100-200, 5696/6016 MB (1504 MB allocatable), 68MCU
* Device #8: NVIDIA CMP 50HX, skipped
* Device #9: NVIDIA CMP 50HX, skipped
* Device #10: NVIDIA CMP 50HX, skipped
* Device #11: NVIDIA CMP 50HX, skipped
* Device #12: NVIDIA CMP 50HX, skipped

OpenCL API (OpenCL 1.2 ) - Platform #2 [Intel(R) Corporation]
=============================================================
* Device #13: Intel(R) HD Graphics 4600, skipped
* Device #14: Intel(R) Core(TM) i3-4360 CPU @ 3.70GHz, skipped

Benchmark relevant options:
===========================
* --backend-devices=7
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#7.........: 40760.5 MH/s (27.70ms) @ Accel:512 Loops:1024 Thr:32 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#7.........: 13631.7 MH/s (83.30ms) @ Accel:64 Loops:1024 Thr:256 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#7.........:  5835.2 MH/s (48.60ms) @ Accel:64 Loops:256 Thr:256 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#7.........:  1716.5 MH/s (82.85ms) @ Accel:8 Loops:1024 Thr:256 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#7.........:  680.2 kH/s (50.28ms) @ Accel:8 Loops:1024 Thr:256 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#7.........: 67864.3 MH/s (16.55ms) @ Accel:128 Loops:1024 Thr:128 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#7.........: 37602.4 MH/s (30.08ms) @ Accel:128 Loops:1024 Thr:128 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#7.........: 42059.6 MH/s (26.87ms) @ Accel:64 Loops:1024 Thr:256 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#7.........:  2955.0 MH/s (48.03ms) @ Accel:64 Loops:128 Thr:256 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#7.........:  1531.8 MH/s (46.36ms) @ Accel:8 Loops:1024 Thr:128 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#7.........: 16468.9 kH/s (56.89ms) @ Accel:64 Loops:1000 Thr:256 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#7.........:    60703 H/s (94.94ms) @ Accel:8 Loops:32 Thr:11 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#7.........:  268.7 kH/s (48.20ms) @ Accel:4096 Loops:512 Thr:32 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#7.........:  904.2 MH/s (78.62ms) @ Accel:256 Loops:128 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#7.........:  860.2 MH/s (82.65ms) @ Accel:256 Loops:128 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#7.........:  117.8 kH/s (48.93ms) @ Accel:8 Loops:1024 Thr:256 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#7.........:    62639 H/s (85.21ms) @ Accel:8 Loops:512 Thr:256 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#7.........:  771.1 kH/s (86.81ms) @ Accel:4 Loops:1023 Thr:256 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#7.........:  549.6 kH/s (90.82ms) @ Accel:128 Loops:4096 Thr:32 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#7.........:    94238 H/s (91.82ms) @ Accel:64 Loops:16384 Thr:32 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#7.........:    67997 H/s (63.74ms) @ Accel:32 Loops:256 Thr:256 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#7.........:  514.8 kH/s (60.86ms) @ Accel:4 Loops:1024 Thr:256 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#7.........:    85084 H/s (67.95ms) @ Accel:512 Loops:128 Thr:32 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#7.........:  4234.6 kH/s (49.42ms) @ Accel:64 Loops:124 Thr:256 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#7.........:    8125 H/s (87.42ms) @ Accel:8 Loops:1024 Thr:256 Vec:1

Started: Sat May 30 23:13:09 2026
Stopped: Sat May 30 23:19:48 2026
```
