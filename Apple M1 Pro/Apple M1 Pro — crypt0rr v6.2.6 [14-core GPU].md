# Apple M1 Pro (14-core GPU)

- **Вендор / Vendor:** Apple
- **Видеокарта / GPU:** Apple M1 Pro
- **Конфигурация / Setup:** 14-core GPU
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [crypt0rr](https://gist.github.com/crypt0rr/66a96a71fa502b6e5ea2eae81ba61c4f)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 5528.9 MH/s |
| 100 | SHA1 | 2335.3 MH/s |
| 1400 | SHA2-256 | 866.9 MH/s |
| 1700 | SHA2-512 | 223.6 MH/s |
| 1000 | NTLM | 8968.9 MH/s |
| 3200 | bcrypt | 3432 H/s |
| 1800 | sha512crypt | — |
| 500 | md5crypt | 1670.4 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 102.4 kH/s |
| 7500 | Kerberos AS-REQ (23) | 72246.4 kH/s |
| 13100 | Kerberos TGS-REP (23) | 62970.4 kH/s |
| 11300 | Bitcoin wallet.dat | 992 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 72022 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #2: Apple's OpenCL drivers (GPU) are known to be unreliable.
             You have been warned.

METAL API (Metal 306.3.5)
=========================
* Device #1: Apple M1 Pro, 5408/10922 MB, 14MCU

OpenCL API (OpenCL 1.2 (Dec 16 2022 20:37:40)) - Platform #1 [Apple]
====================================================================
* Device #2: Apple M1 Pro, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:  5528.9 MH/s (83.44ms) @ Accel:1024 Loops:512 Thr:64 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  2335.3 MH/s (49.10ms) @ Accel:512 Loops:512 Thr:32 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:   866.9 MH/s (66.36ms) @ Accel:512 Loops:256 Thr:32 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:   223.6 MH/s (64.51ms) @ Accel:256 Loops:64 Thr:64 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   102.4 kH/s (68.93ms) @ Accel:256 Loops:256 Thr:32 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:  8968.9 MH/s (51.00ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:   262.5 MH/s (54.22ms) @ Accel:16 Loops:1024 Thr:128 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........:  5742.2 MH/s (80.13ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:   392.5 MH/s (73.31ms) @ Accel:256 Loops:256 Thr:32 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:  7962.6 kH/s (180.14ms) @ Accel:4 Loops:1024 Thr:32 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:  1670.4 kH/s (48.61ms) @ Accel:512 Loops:500 Thr:32 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:     3432 H/s (62.39ms) @ Accel:16 Loops:4 Thr:8 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

* Device #1: Skipping (hash-mode 1800)
             This is due to a known Metal runtime and/or device driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........: 72246.4 kH/s (49.51ms) @ Accel:128 Loops:64 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........: 62970.4 kH/s (56.74ms) @ Accel:32 Loops:256 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:    18243 H/s (66.08ms) @ Accel:1024 Loops:64 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:     3891 H/s (71.82ms) @ Accel:512 Loops:16 Thr:32 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:    27945 H/s (36.11ms) @ Accel:8 Loops:511 Thr:32 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:   111.8 kH/s (61.70ms) @ Accel:32 Loops:4096 Thr:64 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    13602 H/s (63.91ms) @ Accel:8 Loops:16384 Thr:128 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    10493 H/s (84.25ms) @ Accel:128 Loops:128 Thr:128 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:    72022 H/s (48.70ms) @ Accel:128 Loops:64 Thr:64 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    31186 H/s (75.61ms) @ Accel:128 Loops:512 Thr:64 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:   631.4 kH/s (55.36ms) @ Accel:128 Loops:249 Thr:64 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:      992 H/s (73.21ms) @ Accel:8 Loops:1024 Thr:128 Vec:1

Started: Fri Mar 17 15:53:03 2023
Stopped: Fri Mar 17 15:55:36 2023
```
