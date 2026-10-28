# Intel Arc A770M

- **Вендор / Vendor:** Intel
- **Видеокарта / GPU:** Intel Arc A770M
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [ConanChiles](https://gist.github.com/ConanChiles/a6902a400d60aa824b4a3dea692868f8)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 24091.4 MH/s |
| 100 | SHA1 | 10470.0 MH/s |
| 1400 | SHA2-256 | 114.2 MH/s |
| 1700 | SHA2-512 | 806.1 MH/s |
| 1000 | NTLM | 40420.5 MH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 212.4 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in backend information mode

OpenCL Info:
============

OpenCL Platform ID #1
  Vendor..: Intel(R) Corporation
  Name....: Intel(R) OpenCL HD Graphics
  Version.: OpenCL 3.0

  Backend Device ID #1
    Type...........: GPU
    Vendor.ID......: 8
    Vendor.........: Intel(R) Corporation
    Name...........: Intel(R) Arc(TM) A770M Graphics
    Version........: OpenCL 3.0 NEO
    Processor(s)...: 512
    Clock..........: 2050
    Memory.Total...: 13004 MB (limited to 4095 MB allocatable in one block)
    Memory.Free....: 12928 MB
    Local.Memory...: 64 KB
    OpenCL.Version.: OpenCL C 1.2
    Driver.Version.: 31.0.101.4091

OpenCL Platform ID #2
  Vendor..: Intel(R) Corporation
  Name....: Intel(R) OpenCL HD Graphics
  Version.: OpenCL 3.0

  Backend Device ID #2
    Type...........: GPU
    Vendor.ID......: 8
    Vendor.........: Intel(R) Corporation
    Name...........: Intel(R) Iris(R) Xe Graphics
    Version........: OpenCL 3.0 NEO
    Processor(s)...: 96
    Clock..........: 1400
    Memory.Total...: 26042 MB (limited to 2047 MB allocatable in one block)
    Memory.Free....: 12960 MB
    Local.Memory...: 64 KB
    OpenCL.Version.: OpenCL C 1.2
    Driver.Version.: 31.0.101.3430


hashcat.exe -d 1 -b
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

OpenCL API (OpenCL 3.0 ) - Platform #1 [Intel(R) Corporation]
=============================================================
* Device #1: Intel(R) Arc(TM) A770M Graphics, 12928/13004 MB (4095 MB allocatable), 512MCU

OpenCL API (OpenCL 3.0 ) - Platform #2 [Intel(R) Corporation]
=============================================================
* Device #2: Intel(R) Iris(R) Xe Graphics, skipped

Benchmark relevant options:
===========================
* --backend-devices=1
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 24091.4 MH/s (43.60ms) @ Accel:16 Loops:256 Thr:512 Vec:4

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........: 10470.0 MH/s (50.42ms) @ Accel:8 Loops:256 Thr:512 Vec:4

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:   114.2 MH/s (72.48ms) @ Accel:64 Loops:4 Thr:64 Vec:4

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:   806.1 MH/s (82.40ms) @ Accel:4 Loops:64 Thr:512 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   212.4 kH/s (76.26ms) @ Accel:8 Loops:64 Thr:256 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 40420.5 MH/s (25.78ms) @ Accel:16 Loops:256 Thr:512 Vec:4

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:   560.3 MH/s (956.11ms) @ Accel:32 Loops:1024 Thr:32 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 27280.6 MH/s (38.45ms) @ Accel:16 Loops:256 Thr:512 Vec:4

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  1582.2 MH/s (83.80ms) @ Accel:8 Loops:64 Thr:512 Vec:4

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Kernel minimum runtime larger than default TDR

* Device #1: skipped, due to kernel autotune failure (-4).

Aborting session due to kernel autotune failures, for all active devices.

You can use --force to override this, but do not report related errors.

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Started: Tue Mar 14 07:40:27 2023
Stopped: Tue Mar 14 07:43:39 2023
```
