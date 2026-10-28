# AMD EPYC 9754

- **Вендор / Vendor:** AMD
- **Процессор / CPU:** AMD EPYC 9754 (128-Core; в системе 2x CPU — «epyc 9754 x 2»)
- **Версия hashcat / Version:** v6.2.6
- **Бэкенд / Backend:** OpenCL API (OpenCL 2.1 LINUX) — Platform #3 [Intel(R) Corporation], устройство `Device #18: AMD EPYC 9754 128-Core Processor`, 511MCU
- **Источник / Source:** [ManuB1G — hashcat forum thread 11733](https://hashcat.net/forum/thread-11733.html)
- **Примечание / Note:** Смешанный прогон CPU + 8x NVIDIA L40. Бенчмарк ограничен на CPU опцией `--backend-devices=18` (устройство #18 = CPU), поэтому все `Speed.#18` — это чистые CPU-результаты. Оптимизированные ядра (`--optimized-kernel-enable`). Единственное устройство с замерами в выводе — #18.

## Ключевые результаты / Highlights (Speed.#18 = CPU)

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 28029.6 MH/s |
| 100 | SHA1 | 21029.0 MH/s |
| 1400 | SHA2-256 | 10313.6 MH/s |
| 1700 | SHA2-512 | 3480.3 MH/s |
| 1000 | NTLM | 58727.8 MH/s |
| 3200 | bcrypt | 239.1 kH/s |
| 1800 | sha512crypt | 17736 H/s |
| 500 | md5crypt | 1911.4 kH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 1007.0 kH/s |
| 7500 | Kerberos AS-REQ (23) | 276.9 MH/s |
| 13100 | Kerberos TGS-REP (23) | 272.4 MH/s |
| 11300 | Bitcoin/Litecoin wallet.dat | 17160 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 580.6 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

CUDA API (CUDA 12.3)
====================
* Device #1: NVIDIA L40, skipped
* Device #2: NVIDIA L40, skipped
* Device #3: NVIDIA L40, skipped
* Device #4: NVIDIA L40, skipped
* Device #5: NVIDIA L40, skipped
* Device #6: NVIDIA L40, skipped
* Device #7: NVIDIA L40, skipped
* Device #8: NVIDIA L40, skipped

OpenCL API (OpenCL 3.0 PoCL 3.1+debian  Linux, None+Asserts, RELOC, SPIR, LLVM 15.0.6, SLEEF, DISTRO, POCL_DEBUG) - Platform #1 [The pocl project]
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
* Device #18: AMD EPYC 9754 128-Core Processor, 1160893/2321851 MB (290231 MB allocatable), 511MCU

Benchmark relevant options:
===========================
* --backend-devices=18
* --opencl-device-types=1,2
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#18.........: 28029.6 MH/s (8.61ms) @ Accel:1024 Loops:512 Thr:1 Vec:8

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#18.........: 21029.0 MH/s (12.00ms) @ Accel:1024 Loops:512 Thr:1 Vec:8

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#18.........: 10313.6 MH/s (25.14ms) @ Accel:1024 Loops:512 Thr:1 Vec:8

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#18.........:  3480.3 MH/s (75.72ms) @ Accel:1024 Loops:512 Thr:1 Vec:4

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#18.........:  1007.0 kH/s (59.74ms) @ Accel:1024 Loops:512 Thr:1 Vec:8

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#18.........: 58727.8 MH/s (8.68ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#18.........:  7362.6 MH/s (71.11ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#18.........: 34307.4 MH/s (7.35ms) @ Accel:1024 Loops:512 Thr:1 Vec:8

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#18.........:  2575.6 MH/s (50.89ms) @ Accel:512 Loops:512 Thr:1 Vec:8

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#18.........:  294.1 MH/s (55.19ms) @ Accel:32 Loops:1024 Thr:1 Vec:8

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#18.........:  1911.4 kH/s (61.55ms) @ Accel:512 Loops:500 Thr:1 Vec:8

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#18.........:  239.1 kH/s (64.19ms) @ Accel:511 Loops:2 Thr:1 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#18.........:    17736 H/s (3.56ms) @ Accel:1024 Loops:1024 Thr:1 Vec:4

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#18.........:  276.9 MH/s (58.83ms) @ Accel:64 Loops:512 Thr:1 Vec:8

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#18.........:  272.4 MH/s (59.43ms) @ Accel:128 Loops:256 Thr:1 Vec:8

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#18.........:  191.8 kH/s (54.86ms) @ Accel:1024 Loops:512 Thr:1 Vec:8

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#18.........:  129.6 kH/s (74.46ms) @ Accel:256 Loops:1024 Thr:1 Vec:4

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#18.........:  1503.9 kH/s (50.39ms) @ Accel:512 Loops:511 Thr:1 Vec:4

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#18.........:  172.1 kH/s (83.06ms) @ Accel:128 Loops:4096 Thr:1 Vec:8

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#18.........:    24522 H/s (81.04ms) @ Accel:64 Loops:16384 Thr:1 Vec:8

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#18.........:  128.3 kH/s (61.43ms) @ Accel:1024 Loops:512 Thr:1 Vec:8

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#18.........:  580.6 kH/s (49.71ms) @ Accel:128 Loops:1024 Thr:1 Vec:8

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#18.........:    66564 H/s (80.10ms) @ Accel:512 Loops:512 Thr:1 Vec:8

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#18.........:  6126.2 kH/s (58.24ms) @ Accel:1024 Loops:499 Thr:1 Vec:8

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#18.........:    17160 H/s (75.79ms) @ Accel:1024 Loops:512 Thr:1 Vec:4

Started: Fri Dec 15 16:54:17 2023
Stopped: Fri Dec 15 16:57:05 2023
```
