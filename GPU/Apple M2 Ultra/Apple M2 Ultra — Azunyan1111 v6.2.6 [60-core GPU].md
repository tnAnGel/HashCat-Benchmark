# Apple M2 Ultra (60-core GPU)

- **Вендор / Vendor:** Apple
- **Видеокарта / GPU:** Apple M2 Ultra
- **Конфигурация / Setup:** 60-core GPU
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [Azunyan1111](https://gist.github.com/Azunyan1111/38c4c478cf59a608771a5dd6e2da4623)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 26450.7 MH/s |
| 100 | SHA1 | 10899.2 MH/s |
| 1400 | SHA2-256 | 4148.7 MH/s |
| 1700 | SHA2-512 | 1016.7 MH/s |
| 1000 | NTLM | 44537.3 MH/s |
| 3200 | bcrypt | 15266 H/s |
| 1800 | sha512crypt | — |
| 500 | md5crypt | 9313.3 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 482.3 kH/s |
| 7500 | Kerberos AS-REQ (23) | 115.9 MH/s |
| 13100 | Kerberos TGS-REP (23) | 114.9 MH/s |
| 11300 | Bitcoin wallet.dat | 4827 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 143.3 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #2: Apple's OpenCL drivers (GPU) are known to be unreliable.
             You have been warned.

METAL API (Metal 306.7.4)
=========================
* Device #1: Apple M2 Ultra, 49088/98304 MB, 60MCU

OpenCL API (OpenCL 1.2 (Apr 14 2023 18:59:55)) - Platform #1 [Apple]
====================================================================
* Device #2: Apple M2 Ultra, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 26450.7 MH/s (75.33ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........: 10899.2 MH/s (91.62ms) @ Accel:512 Loops:1024 Thr:32 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  4148.7 MH/s (59.97ms) @ Accel:512 Loops:256 Thr:32 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  1016.7 MH/s (61.19ms) @ Accel:512 Loops:64 Thr:32 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   482.3 kH/s (62.99ms) @ Accel:512 Loops:128 Thr:32 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 44537.3 MH/s (89.65ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:  2877.3 MH/s (83.28ms) @ Accel:128 Loops:1024 Thr:32 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 28087.0 MH/s (70.97ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  1924.0 MH/s (64.69ms) @ Accel:512 Loops:128 Thr:32 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........: 52329.5 kH/s (146.60ms) @ Accel:2 Loops:1024 Thr:64 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:  9313.3 kH/s (91.21ms) @ Accel:256 Loops:1000 Thr:64 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    15266 H/s (61.23ms) @ Accel:16 Loops:4 Thr:8 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

* Device #1: Skipping (hash-mode 1800)
             This is due to a known Metal runtime and/or device driver issue (not a hashcat issue)
             You can use --force to override, but do not report related errors.

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........:   115.9 MH/s (134.97ms) @ Accel:8 Loops:1024 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........:   114.9 MH/s (136.11ms) @ Accel:8 Loops:1024 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:    84626 H/s (61.48ms) @ Accel:512 Loops:128 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:    25841 H/s (93.06ms) @ Accel:1024 Loops:16 Thr:32 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:   340.9 kH/s (86.37ms) @ Accel:256 Loops:31 Thr:64 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:   473.5 kH/s (61.21ms) @ Accel:64 Loops:4096 Thr:32 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    57671 H/s (65.73ms) @ Accel:32 Loops:16384 Thr:32 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    48705 H/s (78.27ms) @ Accel:512 Loops:128 Thr:32 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:   143.3 kH/s (51.16ms) @ Accel:4 Loops:1024 Thr:64 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:   142.2 kH/s (71.60ms) @ Accel:256 Loops:256 Thr:64 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  2997.8 kH/s (61.43ms) @ Accel:256 Loops:124 Thr:64 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:     4827 H/s (64.58ms) @ Accel:512 Loops:64 Thr:32 Vec:1

Started: Mon Jun 19 19:27:34 2023
Stopped: Mon Jun 19 19:34:31 2023
```
