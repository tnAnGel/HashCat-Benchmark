# Apple M2 Pro (OpenCL backend (Metal skipped) — device #2)

- **Вендор / Vendor:** Apple
- **Видеокарта / GPU:** Apple M2 Pro
- **Конфигурация / Setup:** OpenCL backend (Metal skipped) — device #2
- **Версия hashcat / Version:** v6.2.6-304-g1ac309149
- **Источник / Source:** [crypt0rr](https://gist.github.com/crypt0rr/dac4ebd7713e69ae0acc007e7d382c2f)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 7040.3 MH/s |
| 100 | SHA1 | 2844.9 MH/s |
| 1400 | SHA2-256 | 1044.7 MH/s |
| 1700 | SHA2-512 | 647.6 MH/s |
| 1000 | NTLM | 12043.0 MH/s |
| 3200 | bcrypt | 4381 H/s |
| 1800 | sha512crypt | — |
| 500 | md5crypt | 2409.1 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 126.1 kH/s |
| 7500 | Kerberos AS-REQ (23) | 91720.8 kH/s |
| 13100 | Kerberos TGS-REP (23) | 76686.1 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6-304-g1ac309149) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

The device #1 has been disabled as it most likely also exists as an OpenCL device, but it is not possible to automatically map it.
You can use -d 1 to use Metal API instead of OpenCL API. In some rare cases this is more stable.

METAL API (Metal 306.3.5)
=========================
* Device #1: Apple M2 Pro, skipped

OpenCL API (OpenCL 1.2 (Dec 16 2022 20:37:40)) - Platform #1 [Apple]
====================================================================
* Device #2: Apple M2 Pro, GPU, 960/10922 MB (1024 MB allocatable), 16MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#2.........:  7040.3 MH/s (0.90ms) @ Accel:512 Loops:1024 Thr:32 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#2.........:  2844.9 MH/s (2.25ms) @ Accel:64 Loops:1024 Thr:256 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#2.........:  1044.7 MH/s (6.15ms) @ Accel:512 Loops:1024 Thr:32 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#2.........:   647.6 MH/s (9.92ms) @ Accel:64 Loops:1024 Thr:256 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#2.........:   126.1 kH/s (6.21ms) @ Accel:64 Loops:1024 Thr:128 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#2.........: 12043.0 MH/s (0.52ms) @ Accel:64 Loops:1024 Thr:256 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#2.........:   973.3 MH/s (6.60ms) @ Accel:512 Loops:1024 Thr:32 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#2.........:  7646.8 MH/s (0.83ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#2.........:   520.2 MH/s (12.37ms) @ Accel:256 Loops:1024 Thr:64 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#2.........:   662.6 MH/s (4.84ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#2.........:  2409.1 kH/s (1.10ms) @ Accel:32 Loops:1000 Thr:256 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#2.........:     4381 H/s (87.98ms) @ Accel:128 Loops:32 Thr:8 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

* Device #2: Skipping (hash-mode 1800)
             This is due to a known OpenCL runtime and/or device driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#2.........: 91720.8 kH/s (70.18ms) @ Accel:512 Loops:1024 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#2.........: 76686.1 kH/s (83.95ms) @ Accel:512 Loops:1024 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#2.........:    22835 H/s (5.86ms) @ Accel:128 Loops:1024 Thr:64 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------
```
