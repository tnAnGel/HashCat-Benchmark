# NVIDIA H100 SXM5 (8x rig — Hopper DC)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA H100 SXM5
- **Конфигурация / Setup:** 8x rig — Hopper DC
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [laluka](https://gist.github.com/laluka/2ee80e40ad485adc26934109f4ab75ef)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 116.7 GH/s |
| 100 | SHA1 | 37326.2 MH/s |
| 1400 | SHA2-256 | 16165.9 MH/s |
| 1700 | SHA2-512 | 5408.6 MH/s |
| 1000 | NTLM | 197.0 GH/s |
| 3200 | bcrypt | 346.1 kH/s |
| 1800 | sha512crypt | 864.9 kH/s |
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 1917.4 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v6.2.6) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #1: WARNING! Kernel exec timeout is not disabled.
             This may cause "CL_OUT_OF_RESOURCES" or related errors.
             To disable the timeout, see: https://hashcat.net/q/timeoutpatch
* Device #9: WARNING! Kernel exec timeout is not disabled.
             This may cause "CL_OUT_OF_RESOURCES" or related errors.
             To disable the timeout, see: https://hashcat.net/q/timeoutpatch
CUDA API (CUDA 12.2)
====================
* Device #1: NVIDIA H100 80GB HBM3, 80489/81230 MB, 132MCU
* Device #2: NVIDIA H100 80GB HBM3, 80700/81230 MB, 132MCU
* Device #3: NVIDIA H100 80GB HBM3, 80700/81230 MB, 132MCU
* Device #4: NVIDIA H100 80GB HBM3, 80700/81230 MB, 132MCU
* Device #5: NVIDIA H100 80GB HBM3, 80700/81230 MB, 132MCU
* Device #6: NVIDIA H100 80GB HBM3, 80700/81230 MB, 132MCU
* Device #7: NVIDIA H100 80GB HBM3, 80700/81230 MB, 132MCU
* Device #8: NVIDIA H100 80GB HBM3, 80700/81230 MB, 132MCU

OpenCL API (OpenCL 3.0 CUDA 12.2.147) - Platform #1 [NVIDIA Corporation]
========================================================================
* Device #9: NVIDIA H100 80GB HBM3, skipped
* Device #10: NVIDIA H100 80GB HBM3, skipped
* Device #11: NVIDIA H100 80GB HBM3, skipped
* Device #12: NVIDIA H100 80GB HBM3, skipped
* Device #13: NVIDIA H100 80GB HBM3, skipped
* Device #14: NVIDIA H100 80GB HBM3, skipped
* Device #15: NVIDIA H100 80GB HBM3, skipped
* Device #16: NVIDIA H100 80GB HBM3, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#1.........:   116.7 GH/s (37.62ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#2.........:   116.7 GH/s (37.58ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#3.........:   116.7 GH/s (37.58ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#4.........:   116.8 GH/s (37.61ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#5.........:   116.8 GH/s (37.59ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#6.........:   116.8 GH/s (37.60ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#7.........:   117.0 GH/s (37.58ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#8.........:   116.8 GH/s (37.59ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#*.........:   934.6 GH/s

----------------------
* Hash-Mode 100 (SHA1)
----------------------

Speed.#1.........: 37326.2 MH/s (59.03ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#2.........: 37413.1 MH/s (58.94ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#3.........: 37400.4 MH/s (58.94ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#4.........: 37375.6 MH/s (58.98ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#5.........: 37383.3 MH/s (58.94ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#6.........: 37370.2 MH/s (58.96ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#7.........: 37380.5 MH/s (58.94ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#8.........: 37391.3 MH/s (58.95ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.#*.........:   299.0 GH/s

---------------------------
* Hash-Mode 1400 (SHA2-256)
---------------------------

Speed.#1.........: 16165.9 MH/s (68.29ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#2.........: 16155.9 MH/s (68.19ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#3.........: 16156.3 MH/s (68.18ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#4.........: 16168.7 MH/s (68.24ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#5.........: 16171.2 MH/s (68.20ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#6.........: 16167.1 MH/s (68.21ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#7.........: 16164.1 MH/s (68.20ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#8.........: 16155.9 MH/s (68.21ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.#*.........:   129.3 GH/s

---------------------------
* Hash-Mode 1700 (SHA2-512)
---------------------------

Speed.#1.........:  5408.6 MH/s (50.92ms) @ Accel:32 Loops:128 Thr:512 Vec:1
Speed.#2.........:  5404.4 MH/s (50.96ms) @ Accel:16 Loops:256 Thr:512 Vec:1
Speed.#3.........:  5403.8 MH/s (50.93ms) @ Accel:16 Loops:256 Thr:512 Vec:1
Speed.#4.........:  5400.5 MH/s (51.00ms) @ Accel:16 Loops:256 Thr:512 Vec:1
Speed.#5.........:  5405.4 MH/s (50.94ms) @ Accel:16 Loops:256 Thr:512 Vec:1
Speed.#6.........:  5400.4 MH/s (50.94ms) @ Accel:16 Loops:256 Thr:512 Vec:1
Speed.#7.........:  5407.6 MH/s (50.95ms) @ Accel:16 Loops:256 Thr:512 Vec:1
Speed.#8.........:  5408.1 MH/s (50.97ms) @ Accel:16 Loops:256 Thr:512 Vec:1
Speed.#*.........: 43238.8 MH/s

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:  1917.4 kH/s (70.02ms) @ Accel:32 Loops:256 Thr:512 Vec:1
Speed.#2.........:  1920.9 kH/s (69.82ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#3.........:  1920.7 kH/s (69.82ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#4.........:  1918.1 kH/s (69.92ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#5.........:  1920.3 kH/s (69.83ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#6.........:  1918.4 kH/s (69.91ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#7.........:  1918.1 kH/s (69.90ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#8.........:  1918.4 kH/s (69.92ms) @ Accel:8 Loops:1024 Thr:512 Vec:1
Speed.#*.........: 15352.4 kH/s

-----------------------
* Hash-Mode 1000 (NTLM)
-----------------------

Speed.#1.........:   197.0 GH/s (22.10ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#2.........:   196.8 GH/s (22.10ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#3.........:   197.8 GH/s (22.07ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#4.........:   197.5 GH/s (22.10ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#5.........:   197.3 GH/s (22.08ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#6.........:   197.4 GH/s (22.08ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#7.........:   197.3 GH/s (22.08ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#8.........:   197.4 GH/s (22.08ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1
Speed.#*.........:  1578.6 GH/s

... (Hash-Modes 3000 LM, 5500 NetNTLMv1, 5600 NetNTLMv2, 1500 descrypt, 500 md5crypt, then bcrypt below) ...

----------------------------------------------------------------
* Hash-Mode 3200 (bcrypt $2*$, Blowfish (Unix)) [Iterations: 32]
----------------------------------------------------------------

Speed.#1.........:   346.1 kH/s (76.18ms) @ Accel:4 Loops:32 Thr:56 Vec:1
Speed.#2.........:   347.2 kH/s (76.16ms) @ Accel:4 Loops:32 Thr:56 Vec:1
Speed.#3.........:   345.2 kH/s (76.16ms) @ Accel:4 Loops:32 Thr:56 Vec:1
Speed.#4.........:   346.4 kH/s (76.19ms) @ Accel:4 Loops:32 Thr:56 Vec:1
Speed.#5.........:   346.9 kH/s (76.16ms) @ Accel:4 Loops:32 Thr:56 Vec:1
Speed.#6.........:   346.0 kH/s (76.16ms) @ Accel:4 Loops:32 Thr:56 Vec:1
Speed.#7.........:   345.0 kH/s (76.16ms) @ Accel:4 Loops:32 Thr:56 Vec:1
Speed.#8.........:   346.3 kH/s (76.17ms) @ Accel:4 Loops:32 Thr:56 Vec:1
Speed.#*.........:  2769.2 kH/s

--------------------------------------------------------------------
* Hash-Mode 1800 (sha512crypt $6$, SHA512 (Unix)) [Iterations: 5000]
--------------------------------------------------------------------

Speed.#1.........:   864.9 kH/s (59.84ms) @ Accel:256 Loops:1024 Thr:1024 Vec:1
Speed.#2.........:   865.3 kH/s (59.88ms) @ Accel:256 Loops:1024 Thr:1024 Vec:1
Speed.#3.........:   865.5 kH/s (59.86ms) @ Accel:256 Loops:1024 Thr:1024 Vec:1
Speed.#4.........:   864.9 kH/s (59.89ms) @ Accel:256 Loops:1024 Thr:1024 Vec:1
Speed.#5.........:   865.2 kH/s (59.88ms) @ Accel:256 Loops:1024 Thr:1024 Vec:1
Speed.#6.........:   865.9 kH/s (59.85ms) @ Accel:256 Loops:1024 Thr:1024 Vec:1
Speed.#7.........:   865.3 kH/s (59.88ms) @ Accel:256 Loops:1024 Thr:1024 Vec:1
Speed.#8.........:   865.3 kH/s (59.88ms) @ Accel:256 Loops:1024 Thr:1024 Vec:1
Speed.#*.........:  6922.3 kH/s

... (additional Hash-Modes 7500/13100 Kerberos, 15300/15900 DPAPI, 7100 macOS, 11600 7-Zip, 12500 RAR3-hp, 13000 RAR5, 6211 TrueCrypt, 13400 KeePass, 6800 LastPass, 11300 Bitcoin wallet.dat also present in source) ...

Started: Tue Jan 23 20:18:01 2024
Stopped: Tue Jan 23 20:27:28 2024
```
