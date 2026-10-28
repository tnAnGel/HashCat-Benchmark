# Intel Arc A770 — full raw hashcat benchmark

- **GPU:** Intel(R) Arc(TM) A770 Graphics, reported device memory `15808/15930 MB` (4095 MB allocatable), 512 MCU.
- **Hashcat:** v6.2.6.
- **Run:** `hashcat -b --force` (the raw header confirms `--force` and `--optimized-kernel-enable`).
- **Date:** 25 August 2024, from the stdout timestamps.
- **Source:** [Pastebin raw stdout](https://pastebin.com/AFDFFVm0), linked by the A770 owner in [the Reddit discussion](https://www.reddit.com/r/IntelArc/comments/1f10yfe/).
- **Evidence type:** complete public `hashcat -b` stdout. This is not a PTS result or aggregate.
- **Caveat:** `--force` was enabled. The output itself reports OpenCL kernel self-test failures for modes 7500 and 13100 and an autotune failure for mode 1500; retain those warnings when interpreting those speeds. The paste provides no driver/OS details beyond the Reddit thread's Windows 11 mention, so those details are not inferred into the run metadata.

## Full stdout

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

You have enabled --force to bypass dangerous warnings and errors!
This can hide serious problems and should only be done when debugging.
Do not report hashcat issues encountered when using --force.

OpenCL API (OpenCL 3.0 ) - Platform #1 [Intel(R) Corporation]
=============================================================
* Device #1: Intel(R) Arc(TM) A770 Graphics, 15808/15930 MB (4095 MB allocatable), 512MCU

Benchmark relevant options:
===========================
* --force
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........: 39200.1 MH/s (26.86ms) @ Accel:32 Loops:256 Thr:256 Vec:4

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........:  8112.1 MH/s (65.24ms) @ Accel:64 Loops:128 Thr:128 Vec:4

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........:  5610.1 MH/s (47.10ms) @ Accel:512 Loops:64 Thr:16 Vec:4

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  1173.7 MH/s (56.69ms) @ Accel:16 Loops:128 Thr:64 Vec:1

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   566.0 kH/s (57.01ms) @ Accel:128 Loops:128 Thr:16 Vec:1

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........: 63332.7 MH/s (33.28ms) @ Accel:128 Loops:512 Thr:64 Vec:4

---------------------
* Hash-Mode 3000 (LM)
---------------------

Speed.#1.........:  1020.6 MH/s (524.69ms) @ Accel:8 Loops:1024 Thr:128 Vec:1

--------------------------------------------
* Hash-Mode 5500 (NetNTLMv1 / NetNTLMv1+ESS)
--------------------------------------------

Speed.#1.........: 41014.1 MH/s (51.61ms) @ Accel:256 Loops:512 Thr:32 Vec:4

----------------------------
* Hash-Mode 5600 (NetNTLMv2)
----------------------------

Speed.#1.........:  2716.1 MH/s (48.67ms) @ Accel:32 Loops:32 Thr:256 Vec:4

--------------------------------------------------------
* Hash-Mode 1500 (descrypt, DES (Unix), Traditional DES)
--------------------------------------------------------

Kernel minimum runtime larger than default TDR

* Device #1: detected kernel autotune failure (-4), min values will be used

Speed.#1.........:  6957.1 kH/s (347.42ms) @ Accel:1 Loops:1024 Thr:1 Vec:1

------------------------------------------------------------------------------
* Hash-Mode 500 (md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5)) [Iterations: 1000]
------------------------------------------------------------------------------

Speed.#1.........: 12582.5 kH/s (74.71ms) @ Accel:512 Loops:250 Thr:16 Vec:4

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:    30480 H/s (64.85ms) @ Accel:4 Loops:2 Thr:16 Vec:1

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:   105.5 kH/s (61.12ms) @ Accel:64 Loops:512 Thr:1024 Vec:1

--------------------------------------------------------
* Hash-Mode 7500 (Kerberos 5, etype 23, AS-REQ Pre-Auth)
--------------------------------------------------------

* Device #1: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#1.........:   366.0 MH/s (91.06ms) @ Accel:256 Loops:32 Thr:8 Vec:4

-------------------------------------------------
* Hash-Mode 13100 (Kerberos 5, etype 23, TGS-REP)
-------------------------------------------------

* Device #1: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#1.........:   408.7 MH/s (81.48ms) @ Accel:256 Loops:32 Thr:8 Vec:4

---------------------------------------------------------------------------------
* Hash-Mode 15300 (DPAPI masterkey file v1 (context 1 and 2)) [Iterations: 23999]
---------------------------------------------------------------------------------

Speed.#1.........:   133.6 kH/s (80.98ms) @ Accel:16 Loops:64 Thr:512 Vec:1

---------------------------------------------------------------------------------
* Hash-Mode 15900 (DPAPI masterkey file v2 (context 1 and 2)) [Iterations: 12899]
---------------------------------------------------------------------------------

Speed.#1.........:    45235 H/s (56.60ms) @ Accel:8 Loops:32 Thr:256 Vec:1

------------------------------------------------------------------
* Hash-Mode 7100 (macOS v10.8+ (PBKDF2-SHA512)) [Iterations: 1023]
------------------------------------------------------------------

Speed.#1.........:   551.5 kH/s (50.37ms) @ Accel:32 Loops:7 Thr:256 Vec:1

---------------------------------------------
* Hash-Mode 11600 (7-Zip) [Iterations: 16384]
---------------------------------------------

Speed.#1.........:   245.1 kH/s (527.00ms) @ Accel:16 Loops:4096 Thr:64 Vec:4

------------------------------------------------
* Hash-Mode 12500 (RAR3-hp) [Iterations: 262144]
------------------------------------------------

Speed.#1.........:    51116 H/s (319.43ms) @ Accel:2 Loops:16384 Thr:512 Vec:4

--------------------------------------------
* Hash-Mode 13000 (RAR5) [Iterations: 32799]
--------------------------------------------

Speed.#1.........:    82799 H/s (48.96ms) @ Accel:8 Loops:128 Thr:256 Vec:1

--------------------------------------------------------------------------------
* Hash-Mode 6211 (TrueCrypt RIPEMD160 + XTS 512 bit (legacy)) [Iterations: 1999]
--------------------------------------------------------------------------------

Speed.#1.........:   415.1 kH/s (79.70ms) @ Accel:256 Loops:32 Thr:16 Vec:1

-----------------------------------------------------------------------------------
* Hash-Mode 13400 (KeePass 1 (AES/Twofish) and KeePass 2 (AES)) [Iterations: 24569]
-----------------------------------------------------------------------------------

Speed.#1.........:    33819 H/s (80.06ms) @ Accel:256 Loops:32 Thr:16 Vec:1

----------------------------------------------------------------
* Hash-Mode 6800 (LastPass + LastPass sniffed) [Iterations: 499]
----------------------------------------------------------------

Speed.#1.........:  4810.6 kH/s (31.90ms) @ Accel:4 Loops:249 Thr:256 Vec:1

--------------------------------------------------------------------
* Hash-Mode 11300 (Bitcoin/Litecoin wallet.dat) [Iterations: 200459]
--------------------------------------------------------------------

Speed.#1.........:     5859 H/s (56.67ms) @ Accel:64 Loops:64 Thr:32 Vec:1

Started: Sun Aug 25 22:11:29 2024
Stopped: Sun Aug 25 22:15:01 2024
```
