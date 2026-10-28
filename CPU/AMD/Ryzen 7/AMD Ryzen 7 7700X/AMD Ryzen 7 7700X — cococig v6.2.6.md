# AMD Ryzen 7 7700X

- **Вендор / Vendor:** AMD
- **Процессор / CPU:** AMD Ryzen 7 7700X 8-Core Processor
- **Версия hashcat / Version:** v6.2.6
- **Бэкенд / Backend:** OpenCL API (OpenCL 3.0 PoCL 3.1+debian, LLVM 15.0.6) — `[The pocl project]`, устройство `pthread-skylake-avx512-AMD Ryzen 7 7700X 8-Core Processor`
- **Источник / Source:** [cococig (GitHub Gist)](https://gist.github.com/cococig/2b592488fcbdb8a0301b8c38acaee466)
- **Примечание / Note:** Прогон только на CPU (Device #1). Стандартный `hashcat -b` (не `--benchmark-all`) — ограниченный набор режимов.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 3346.8 MH/s |
| 100 | SHA1 | 1744.8 MH/s |
| 1400 | SHA2-256 | 762.2 MH/s |
| 1700 | SHA2-512 | 261.3 MH/s |
| 1000 | NTLM | 6156.6 MH/s |
| 3200 | bcrypt | 1011 H/s |
| 1800 | sha512crypt | 9440 H/s |
| 500 | md5crypt | 180.8 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 64203 H/s |
| 7500 | Kerberos AS-REQ (23) | 15426.7 kH/s |
| 13100 | Kerberos TGS-REP (23) | 15484.8 kH/s |
| 11300 | Bitcoin/Litecoin wallet.dat | 1265 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 52609 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

OpenCL API (OpenCL 3.0 PoCL 3.1+debian  Linux, None+Asserts, RELOC, SPIR, LLVM 15.0.6, SLEEF, DISTRO, POCL_DEBUG) - Platform #1 [The pocl project]
==================================================================================================================================================
* Device #1: pthread-skylake-avx512-AMD Ryzen 7 7700X 8-Core Processor, 6726/13516 MB (2048 MB allocatable), 16MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:  3346.8 MH/s (4.61ms) @ Accel:1024 Loops:1024 Thr:1 Vec:16

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  1744.8 MH/s (9.13ms) @ Accel:1024 Loops:1024 Thr:1 Vec:16

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:   762.2 MH/s (21.81ms) @ Accel:1024 Loops:1024 Thr:1 Vec:16

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:   261.3 MH/s (63.96ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:    64203 H/s (48.08ms) @ Accel:1024 Loops:1024 Thr:1 Vec:16

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:  6156.6 MH/s (2.51ms) @ Accel:1024 Loops:1024 Thr:1 Vec:16

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:   449.5 MH/s (36.24ms) @ Accel:1024 Loops:1024 Thr:1 Vec:16

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........:  3670.0 MH/s (4.35ms) @ Accel:1024 Loops:1024 Thr:1 Vec:16

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:   203.6 MH/s (82.09ms) @ Accel:1024 Loops:1024 Thr:1 Vec:16

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........: 16114.4 kH/s (61.07ms) @ Accel:64 Loops:1024 Thr:1 Vec:16

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:   180.8 kH/s (88.95ms) @ Accel:1024 Loops:1000 Thr:1 Vec:16

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:     1011 H/s (18.39ms) @ Accel:16 Loops:32 Thr:1 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:     9440 H/s (21.37ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........: 15426.7 kH/s (67.73ms) @ Accel:64 Loops:1024 Thr:1 Vec:16

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........: 15484.8 kH/s (67.49ms) @ Accel:128 Loops:512 Thr:1 Vec:16

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:    14256 H/s (47.47ms) @ Accel:1024 Loops:1024 Thr:1 Vec:16

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:     9838 H/s (63.62ms) @ Accel:512 Loops:1024 Thr:1 Vec:8

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:   120.8 kH/s (65.70ms) @ Accel:512 Loops:1023 Thr:1 Vec:8

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:    11814 H/s (86.07ms) @ Accel:256 Loops:4096 Thr:1 Vec:16

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:     1580 H/s (80.74ms) @ Accel:128 Loops:16384 Thr:1 Vec:16

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    10122 H/s (48.86ms) @ Accel:1024 Loops:1024 Thr:1 Vec:16

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:    52609 H/s (75.91ms) @ Accel:1024 Loops:512 Thr:1 Vec:16

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:     2536 H/s (67.16ms) @ Accel:1024 Loops:256 Thr:1 Vec:16

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:   613.2 kH/s (23.81ms) @ Accel:1024 Loops:499 Thr:1 Vec:16

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:     1265 H/s (66.00ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Started: Wed Aug 30 01:01:13 2023
Stopped: Wed Aug 30 01:06:19 2023
```
