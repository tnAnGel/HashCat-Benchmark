# Apple M2 (10-core GPU)

- **Вендор / Vendor:** Apple
- **Видеокарта / GPU:** Apple M2
- **Конфигурация / Setup:** 10-core GPU
- **Версия hashcat / Version:** v6.2.5-644-g3f20e50c8
- **Источник / Source:** [soxrok2212](https://gist.github.com/soxrok2212/35dba49d345ad91184f521ebed060826)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 2294.7 MH/s |
| 100 | SHA1 | 1087.6 MH/s |
| 1400 | SHA2-256 | 339.1 MH/s |
| 1700 | SHA2-512 | 120.0 MH/s |
| 1000 | NTLM | 2690.7 MH/s |
| 3200 | bcrypt | 2882 H/s |
| 500 | md5crypt | 692.8 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 67443 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.5-644-g3f20e50c8) starting in benchmark mode

* Device #2: Apple's OpenCL drivers (GPU) are known to be unreliable.
             You have been warned.

METAL API (Metal 263.8)
=======================
* Device #1: Apple M2, 5408/10922 MB, 10MCU

OpenCL API (OpenCL 1.2 (Jun 17 2022 18:58:24)) - Platform #1 [Apple]
====================================================================
* Device #2: Apple M2, skipped

Benchmark relevant options:
===========================
* --workload-profile=4

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:  2294.7 MH/s (291.37ms) @ Accel:2048 Loops:1024 Thr:32 Vec:1

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  1087.6 MH/s (307.24ms) @ Accel:256 Loops:1024 Thr:128 Vec:1

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:   339.1 MH/s (246.35ms) @ Accel:256 Loops:512 Thr:64 Vec:1

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:   120.0 MH/s (348.26ms) @ Accel:256 Loops:256 Thr:64 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:    67443 H/s (301.81ms) @ Accel:256 Loops:512 Thr:64 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:  2690.7 MH/s (248.34ms) @ Accel:512 Loops:1024 Thr:128 Vec:1

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:   627.5 MH/s (260.40ms) @ Accel:512 Loops:1024 Thr:32 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........:  2698.8 MH/s (247.64ms) @ Accel:1024 Loops:1024 Thr:64 Vec:1

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:   121.2 MH/s (690.34ms) @ Accel:256 Loops:256 Thr:128 Vec:1

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Speed.#1.........: 24036.1 kH/s (429.66ms) @ Accel:32 Loops:1024 Thr:32 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........:   692.8 kH/s (459.78ms) @ Accel:512 Loops:500 Thr:128 Vec:1

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:     2882 H/s (432.81ms) @ Accel:32 Loops:16 Thr:8 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Dies here...
```
