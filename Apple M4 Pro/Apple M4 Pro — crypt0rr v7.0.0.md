# Apple M4 Pro

- **Вендор / Vendor:** Apple
- **Видеокарта / GPU:** Apple M4 Pro
- **Версия hashcat / Version:** v7.0.0
- **Источник / Source:** [crypt0rr](https://gist.github.com/crypt0rr/c801c67c7ac8fb07478ec789acb24c7e)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 8966.1 MH/s |
| 100 | SHA1 | 3986.8 MH/s |
| 1400 | SHA2-256 | 1431.6 MH/s |
| 1700 | SHA2-512 | 292.4 MH/s |
| 1000 | NTLM | 15707.3 MH/s |
| 3200 | bcrypt | 7480 H/s |
| 1800 | sha512crypt | 45443 H/s |
| 500 | md5crypt | 4392.4 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 195.5 kH/s |
| 7500 | Kerberos AS-REQ (23) | 130.1 MH/s |
| 13100 | Kerberos TGS-REP (23) | 131.0 MH/s |
| 11300 | Bitcoin wallet.dat | 1349 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 135.1 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v7.0.0) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

METAL API (Metal 368.52)
========================
* Device #01: Apple M4 Pro, skipped

OpenCL API (OpenCL 1.2 (Jul 11 2025 19:18:49)) - Platform #1 [Apple]
====================================================================
* Device #02: Apple M4 Pro, GPU, 8192/16384 MB (1536 MB allocatable), 16MCU

Benchmark relevant options:
===========================
* --backend-devices-virtmulti=1
* --backend-devices-virthost=1
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#02........:  8966.1 MH/s (3.93ms) @ Accel:352 Loops:1024 Thr:256 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#02........:  3986.8 MH/s (8.87ms) @ Accel:352 Loops:1024 Thr:256 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#02........:  1431.6 MH/s (24.72ms) @ Accel:352 Loops:1024 Thr:256 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#02........:   292.4 MH/s (88.09ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#02........:   195.5 kH/s (44.11ms) @ Accel:352 Loops:1024 Thr:256 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#02........: 15707.3 MH/s (2.20ms) @ Accel:352 Loops:1024 Thr:256 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#02........:  4261.1 MH/s (8.30ms) @ Accel:352 Loops:1024 Thr:256 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#02........: 10094.8 MH/s (3.42ms) @ Accel:352 Loops:1024 Thr:256 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#02........:   682.8 MH/s (51.83ms) @ Accel:352 Loops:1024 Thr:256 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#02........:   283.5 MH/s (90.83ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#02........:  4392.4 kH/s (7.70ms) @ Accel:352 Loops:1000 Thr:256 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#02........:     7480 H/s (97.59ms) @ Accel:241 Loops:32 Thr:8 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#02........:    45443 H/s (54.58ms) @ Accel:128 Loops:1000 Thr:256 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#02........:   130.1 MH/s (98.95ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#02........:   131.0 MH/s (98.33ms) @ Accel:1024 Loops:1024 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#02........:    34266 H/s (41.90ms) @ Accel:352 Loops:1000 Thr:256 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#02........:     9870 H/s (75.67ms) @ Accel:96 Loops:1024 Thr:256 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#02........:   125.4 kH/s (87.45ms) @ Accel:224 Loops:512 Thr:256 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#02........:   198.8 kH/s (43.36ms) @ Accel:352 Loops:4096 Thr:256 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#02........:    32007 H/s (21.36ms) @ Accel:288 Loops:16384 Thr:256 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#02........:    18117 H/s (48.58ms) @ Accel:288 Loops:1024 Thr:256 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#02........:   135.1 kH/s (46.31ms) @ Accel:128 Loops:1000 Thr:256 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#02........:    27673 H/s (51.92ms) @ Accel:352 Loops:1024 Thr:256 Vec:1

-------------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 100099]
-------------------------------------------------------------------

Speed.#02........:     5898 H/s (59.77ms) @ Accel:352 Loops:1024 Thr:256 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#02........:     1349 H/s (95.02ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

Started: Thu Aug 14 16:03:42 2025
Stopped: Thu Aug 14 16:18:26 2025
```
