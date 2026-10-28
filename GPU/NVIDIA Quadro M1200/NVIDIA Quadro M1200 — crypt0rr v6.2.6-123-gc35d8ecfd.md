# NVIDIA Quadro M1200

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA Quadro M1200
- **Версия hashcat / Version:** v6.2.6-123-gc35d8ecfd
- **Источник / Source:** [crypt0rr — gist](https://gist.github.com/crypt0rr/5a2e40f0382ee8004ff7011941778624)

> Мобильная (ноутбучная) Quadro на Maxwell. Прогон выполнен с `--workload-profile=4`.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 1411.4 MH/s |
| 100 | SHA1 | 904.3 MH/s |
| 1400 | SHA2-256 | 339.1 MH/s |
| 1700 | SHA2-512 | 128.1 MH/s |
| 1000 | NTLM | 1800.5 MH/s |
| 3200 | bcrypt | 1621 H/s |
| 1800 | sha512crypt | 7618 H/s |
| 500 | md5crypt | 210.5 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 63601 H/s |
| 7500 | Kerberos AS-REQ (23) | 34076.9 kH/s |
| 13100 | Kerberos TGS-REP (23) | 34545.7 kH/s |
| 11300 | Bitcoin wallet.dat | 663 H/s |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 41628 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6-123-gc35d8ecfd) starting in benchmark mode

* Device #1: WARNING! Kernel exec timeout is not disabled.
             This may cause "CL_OUT_OF_RESOURCES" or related errors.
             To disable the timeout, see: https://hashcat.net/q/timeoutpatch
* Device #2: WARNING! Kernel exec timeout is not disabled.
             This may cause "CL_OUT_OF_RESOURCES" or related errors.
             To disable the timeout, see: https://hashcat.net/q/timeoutpatch
CUDA API (CUDA 12.0)
====================
* Device #1: Quadro M1200, 4005/4042 MB, 5MCU

OpenCL API (OpenCL 3.0 CUDA 12.0.147) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #2: Quadro M1200, skipped

Benchmark relevant options:
===========================
* --workload-profile=4

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:  1411.4 MH/s (235.41ms) @ Accel:128 Loops:1024 Thr:512 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:   904.3 MH/s (367.75ms) @ Accel:256 Loops:1024 Thr:256 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:   339.1 MH/s (245.41ms) @ Accel:32 Loops:1024 Thr:512 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:   128.1 MH/s (325.12ms) @ Accel:16 Loops:1024 Thr:512 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:    63601 H/s (315.30ms) @ Accel:32 Loops:1024 Thr:512 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:  1800.5 MH/s (368.59ms) @ Accel:512 Loops:1024 Thr:256 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:  3613.4 MH/s (365.55ms) @ Accel:8192 Loops:1024 Thr:32 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........:  1786.2 MH/s (369.85ms) @ Accel:1024 Loops:512 Thr:256 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:   137.3 MH/s (303.41ms) @ Accel:256 Loops:1024 Thr:32 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........:   157.7 MH/s (264.07ms) @ Accel:256 Loops:1024 Thr:32 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:   210.5 kH/s (368.80ms) @ Accel:256 Loops:1000 Thr:64 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:     1621 H/s (285.34ms) @ Accel:8 Loops:32 Thr:12 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:     7618 H/s (213.02ms) @ Accel:512 Loops:512 Thr:32 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

Speed.#1.........: 34076.9 kH/s (306.89ms) @ Accel:256 Loops:256 Thr:32 Vec:1

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

Speed.#1.........: 34545.7 kH/s (302.71ms) @ Accel:256 Loops:256 Thr:32 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:    10935 H/s (317.08ms) @ Accel:32 Loops:1024 Thr:512 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:     4634 H/s (347.87ms) @ Accel:64 Loops:1024 Thr:64 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:    57746 H/s (325.36ms) @ Accel:32 Loops:1023 Thr:128 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:    11365 H/s (447.20ms) @ Accel:256 Loops:512 Thr:128 Vec:1

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:     4592 H/s (276.48ms) @ Accel:8 Loops:16384 Thr:512 Vec:1

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:     5497 H/s (461.27ms) @ Accel:32 Loops:1024 Thr:512 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:    41628 H/s (451.29ms) @ Accel:16 Loops:1024 Thr:512 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:     5150 H/s (329.62ms) @ Accel:32 Loops:1024 Thr:256 Vec:1

-------------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 100099]
-------------------------------------------------------------------

Speed.#1.........:     1807 H/s (460.38ms) @ Accel:32 Loops:1024 Thr:512 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:      663 H/s (309.95ms) @ Accel:256 Loops:64 Thr:512 Vec:1

Started: Thu Mar 16 16:44:09 2023
Stopped: Thu Mar 16 16:53:39 2023
```
