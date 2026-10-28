# Intel Arc 140V

- **Вендор / Vendor:** Intel
- **Видеокарта / GPU:** Intel(R) Arc(TM) 140V GPU (Lunar Lake, Core Ultra 7 258V iGPU)
- **Версия hashcat / Version:** v6.2.6-813-g686bc227c (beta)
- **Источник / Source:** [hashcat.net forum — mi7chy, "Intel Lunar Lake 258V Benchmark"](https://hashcat.net/forum/thread-12178.html)
- **Примечания / Notes:** Lenovo Yoga Slim 7i Aura Edition (Core Ultra 7 258V, 32GB RAM). OpenCL backend, Device #1. Прогон с `--force --backend-devices-virtual=1 --optimized-kernel-enable`. Некоторые режимы (3200 bcrypt, 7500, 13100) с `OpenCL kernel self-test failed`, а 1500 descrypt — `kernel autotune failure (-4), min values used`; значения приведены как в выводе.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 6573.5 MH/s |
| 100 | SHA1 | 1132.3 MH/s |
| 1400 | SHA2-256 | 500.4 MH/s |
| 1700 | SHA2-512 | 81148.6 kH/s |
| 1000 | NTLM | 8426.5 MH/s |
| 3200 | bcrypt | 3874 H/s (self-test failed) |
| 1800 | sha512crypt | 9335 H/s |
| 500 | md5crypt | 2523.5 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 154.8 kH/s |
| 7500 | Kerberos AS-REQ (23) | 52037.2 kH/s (self-test failed) |
| 13100 | Kerberos TGS-REP (23) | 46214.1 kH/s (self-test failed) |
| 11300 | Bitcoin/Litecoin wallet.dat | 246 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 103.6 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6-813-g686bc227c) starting in benchmark mode

You have enabled --force to bypass dangerous warnings and errors!
This can hide serious problems and should only be done when debugging.
Do not report hashcat issues encountered when using --force.

OpenCL API (OpenCL 3.0 ) - Platform #1 [Intel(R) Corporation]
=============================================================
* Device #1: Intel(R) Arc(TM) 140V GPU (16GB), 7328/14733 MB (2047 MB allocatable), 64MCU

Benchmark relevant options:
===========================
* --force
* --backend-devices-virtual=1
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:  6573.5 MH/s (78.67ms) @ Accel:512 Loops:512 Thr:32 Vec:4

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  1132.3 MH/s (57.24ms) @ Accel:256 Loops:128 Thr:32 Vec:4

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  500.4 MH/s (64.88ms) @ Accel:32 Loops:32 Thr:512 Vec:4

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........: 81148.6 kH/s (100.06ms) @ Accel:256 Loops:16 Thr:32 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:  154.8 kH/s (49.45ms) @ Accel:2 Loops:256 Thr:1024 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:  8426.5 MH/s (60.85ms) @ Accel:512 Loops:512 Thr:32 Vec:4

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:  269.6 MH/s (245.22ms) @ Accel:32 Loops:1024 Thr:32 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........:  6575.4 MH/s (78.41ms) @ Accel:512 Loops:512 Thr:32 Vec:4

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  385.1 MH/s (84.15ms) @ Accel:16 Loops:32 Thr:1024 Vec:4

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Kernel minimum runtime larger than default TDR
* Device #1: detected kernel autotune failure (-4), min values will be used
Speed.#1.........:  610.7 kH/s (256.55ms) @ Accel:1 Loops:1024 Thr:1 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:  2523.5 kH/s (73.42ms) @ Accel:16 Loops:1000 Thr:256 Vec:4

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

* Device #1: ATTENTION! OpenCL kernel self-test failed.
Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver
Speed.#1.........:    3874 H/s (60.30ms) @ Accel:1 Loops:4 Thr:32 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:    9335 H/s (86.09ms) @ Accel:64 Loops:512 Thr:128 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

* Device #1: ATTENTION! OpenCL kernel self-test failed.
Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver
Speed.#1.........: 52037.2 kH/s (78.19ms) @ Accel:8 Loops:1024 Thr:8 Vec:4

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

* Device #1: ATTENTION! OpenCL kernel self-test failed.
Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver
Speed.#1.........: 46214.1 kH/s (88.15ms) @ Accel:8 Loops:1024 Thr:8 Vec:4

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:    26111 H/s (51.33ms) @ Accel:256 Loops:128 Thr:16 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:    1876 H/s (84.43ms) @ Accel:64 Loops:8 Thr:64 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:    22744 H/s (65.17ms) @ Accel:16 Loops:3 Thr:512 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:    84064 H/s (179.59ms) @ Accel:4 Loops:4096 Thr:256 Vec:4

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    13004 H/s (310.33ms) @ Accel:1 Loops:16384 Thr:1024 Vec:4

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    12978 H/s (76.20ms) @ Accel:4 Loops:128 Thr:1024 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:  103.6 kH/s (73.32ms) @ Accel:128 Loops:128 Thr:16 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    10394 H/s (31.51ms) @ Accel:128 Loops:64 Thr:16 Vec:1

-------------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 100099]
-------------------------------------------------------------------

Speed.#1.........:    4306 H/s (75.57ms) @ Accel:8 Loops:128 Thr:512 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:      246 H/s (83.27ms) @ Accel:4 Loops:32 Thr:512 Vec:1

Started: Fri Oct 04 12:52:11 2024
Stopped: Fri Oct 04 13:02:40 2024
```
