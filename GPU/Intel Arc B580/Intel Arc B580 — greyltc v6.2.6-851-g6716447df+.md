# Intel Arc B580

- **Вендор / Vendor:** Intel
- **Видеокарта / GPU:** Intel Arc B580
- **Версия hashcat / Version:** v6.2.6-851-g6716447df+
- **Источник / Source:** [greyltc](https://gist.github.com/greyltc/fa080823980e48a198db5254f71ac5a7)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 24710.7 MH/s |
| 100 | SHA1 | 2288.9 MH/s |
| 1400 | SHA2-256 | 1280.3 MH/s |
| 1700 | SHA2-512 | 318.2 MH/s |
| 1000 | NTLM | 33346.3 MH/s |
| 3200 | bcrypt | 15405 H/s |
| 1800 | sha512crypt | 39647 H/s |
| 500 | md5crypt | 11398.2 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 579.5 kH/s |
| 7500 | Kerberos AS-REQ (23) | 194.1 MH/s |
| 13100 | Kerberos TGS-REP (23) | 175.3 MH/s |
| 11300 | Bitcoin wallet.dat | 1512 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 393.8 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6-851-g6716447df+) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

You have enabled --force to bypass dangerous warnings and errors!
This can hide serious problems and should only be done when debugging.
Do not report hashcat issues encountered when using --force.

OpenCL API (OpenCL 3.0 ) - Platform #1 [Intel(R) Corporation]
=============================================================
* Device #1: Intel(R) Graphics [0xe20b], 11520/11605 MB (11605 MB allocatable), 160MCU

Benchmark relevant options:
===========================
* --force
* --backend-devices-virtual=1
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 24710.7 MH/s (53.23ms) @ Accel:256 Loops:1024 Thr:32 Vec:4

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  2288.9 MH/s (72.16ms) @ Accel:8 Loops:128 Thr:1024 Vec:4

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  1280.3 MH/s (64.32ms) @ Accel:16 Loops:32 Thr:1024 Vec:4

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:   318.2 MH/s (65.10ms) @ Accel:2 Loops:64 Thr:1024 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   579.5 kH/s (69.67ms) @ Accel:64 Loops:512 Thr:32 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 33346.3 MH/s (78.99ms) @ Accel:32 Loops:1024 Thr:512 Vec:4

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:   543.2 MH/s (307.68ms) @ Accel:1 Loops:1024 Thr:1024 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 24996.7 MH/s (52.17ms) @ Accel:512 Loops:256 Thr:64 Vec:4

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  1582.0 MH/s (51.46ms) @ Accel:32 Loops:16 Thr:1024 Vec:4

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

* Device #1: detected kernel autotune failure (-4), min values will be used

Speed.#1.........:  1150.1 kH/s (306.57ms) @ Accel:1 Loops:1024 Thr:1 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........: 11398.2 kH/s (49.75ms) @ Accel:128 Loops:1000 Thr:32 Vec:4

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    15405 H/s (81.09ms) @ Accel:8 Loops:1 Thr:32 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:    39647 H/s (81.86ms) @ Accel:512 Loops:128 Thr:256 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#1.........:   194.1 MH/s (53.08ms) @ Accel:16 Loops:512 Thr:8 Vec:4

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#1.........:   175.3 MH/s (58.82ms) @ Accel:128 Loops:64 Thr:8 Vec:4

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:    99193 H/s (69.82ms) @ Accel:2 Loops:512 Thr:1024 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:    10959 H/s (73.01ms) @ Accel:8 Loops:8 Thr:1024 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:   123.9 kH/s (71.35ms) @ Accel:8 Loops:7 Thr:1024 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:   238.5 kH/s (168.36ms) @ Accel:8 Loops:4096 Thr:128 Vec:4

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    51309 H/s (198.63ms) @ Accel:2 Loops:16384 Thr:512 Vec:4

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    49743 H/s (51.13ms) @ Accel:8 Loops:256 Thr:256 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:   393.8 kH/s (50.67ms) @ Accel:8 Loops:128 Thr:256 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    44004 H/s (77.30ms) @ Accel:128 Loops:256 Thr:16 Vec:1

-------------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 100099]
-------------------------------------------------------------------

Speed.#1.........:    16382 H/s (50.92ms) @ Accel:32 Loops:512 Thr:32 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:     1512 H/s (68.59ms) @ Accel:16 Loops:16 Thr:512 Vec:1

Started: Wed Dec 25 12:23:37 2024
Stopped: Wed Dec 25 12:28:39 2024
```
