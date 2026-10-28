# AMD Ryzen 7 5800X

- **Вендор / Vendor:** AMD
- **Устройство / Device:** AMD Ryzen 7 5800X 8-Core Processor
- **Версия hashcat / Version:** v6.2.5-545-g8e200e8eb+
- **Источник / Source:** [hashcat Forum — The Mechanic](https://hashcat.net/forum/thread-10898.html)
- **Бэкенд / Backend:** OpenCL 3.0 LINUX (Intel CPU runtime), Device #4 = CPU, 16MCU
- **Примечание / Note:** CPU-only прогон (`--opencl-device-types=1`, optimized kernel), GPU-устройства (RX 6700 XT) в прогоне пропущены (skipped).

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 1648.1 MH/s |
| 100 | SHA1 | 916.8 MH/s |
| 1400 | SHA2-256 | 343.7 MH/s |
| 1700 | SHA2-512 | 122.0 MH/s |
| 1000 | NTLM | 3001.6 MH/s |
| 3200 | bcrypt | 11797 H/s |
| 1800 | sha512crypt | 8072 H/s |
| 500 | md5crypt | 135.8 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 43057 H/s |
| 7500 | Kerberos AS-REQ (23) | 12862.7 kH/s |
| 13100 | Kerberos TGS-REP (23) | 12391.1 kH/s |
| 11300 | Bitcoin wallet.dat | 585 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 31861 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.5-545-g8e200e8eb+) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

HIP API (HIP 5.1.20531)
=======================
* Device #1: AMD Radeon RX 6700 XT, skipped
* Device #2: AMD Radeon RX 6700 XT, skipped

OpenCL API (OpenCL 1.2 Intel(R) FPGA SDK for OpenCL(TM), Version 20.3) - Platform #1 [Intel(R) Corporation]
===========================================================================================================
* Device #3: Intel(R) FPGA Emulation Device, skipped

OpenCL API (OpenCL 3.0 LINUX) - Platform #2 [Intel(R) Corporation]
==================================================================
* Device #4: AMD Ryzen 7 5800X 8-Core Processor, 15979/32023 MB (8005 MB allocatable), 16MCU

OpenCL API (OpenCL 2.1 AMD-APP (3423.0)) - Platform #3 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #5: AMD Radeon RX 6700 XT, skipped
* Device #6: AMD Radeon RX 6700 XT, skipped

Benchmark relevant options:
===========================
* --opencl-device-types=1
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#4.........:  1648.1 MH/s (10.07ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#4.........:  916.8 MH/s (18.27ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#4.........:  343.7 MH/s (48.76ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#4.........:  122.0 MH/s (68.69ms) @ Accel:512 Loops:1024 Thr:1 Vec:4

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#4.........:    43057 H/s (94.77ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#4.........:  3001.6 MH/s (5.54ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#4.........:  398.0 MH/s (42.03ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#4.........:  1896.9 MH/s (8.79ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#4.........:  137.4 MH/s (61.01ms) @ Accel:512 Loops:1024 Thr:1 Vec:8

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#4.........: 16591.0 kH/s (63.08ms) @ Accel:64 Loops:1024 Thr:1 Vec:8

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#4.........:  135.8 kH/s (56.75ms) @ Accel:512 Loops:1000 Thr:1 Vec:8

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#4.........:    11797 H/s (21.13ms) @ Accel:16 Loops:32 Thr:1 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#4.........:    8072 H/s (25.24ms) @ Accel:1024 Loops:1024 Thr:1 Vec:4

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#4.........: 12862.7 kH/s (81.49ms) @ Accel:512 Loops:128 Thr:1 Vec:8

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#4.........: 12391.1 kH/s (84.59ms) @ Accel:512 Loops:128 Thr:1 Vec:8

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#4.........:    7590 H/s (89.61ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#4.........:    4142 H/s (77.38ms) @ Accel:1024 Loops:256 Thr:1 Vec:4

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#4.........:    51702 H/s (78.55ms) @ Accel:256 Loops:1023 Thr:1 Vec:4

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#4.........:    10328 H/s (49.41ms) @ Accel:128 Loops:4096 Thr:1 Vec:8

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#4.........:    1413 H/s (90.51ms) @ Accel:128 Loops:16384 Thr:1 Vec:8

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#4.........:    4254 H/s (58.29ms) @ Accel:512 Loops:1024 Thr:1 Vec:8

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#4.........:    31861 H/s (63.39ms) @ Accel:1024 Loops:256 Thr:1 Vec:8

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#4.........:    3558 H/s (95.85ms) @ Accel:512 Loops:1024 Thr:1 Vec:8

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#4.........:  270.7 kH/s (57.87ms) @ Accel:1024 Loops:499 Thr:1 Vec:8

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#4.........:      585 H/s (71.45ms) @ Accel:1024 Loops:512 Thr:1 Vec:4

Started: Sun Jul 24 13:08:40 2022
Stopped: Sun Jul 24 13:21:00 2022
```
