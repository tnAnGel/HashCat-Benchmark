# AMD Radeon Pro 5500M

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon Pro 5500M (Compute Engine, MacBook Pro 16", macOS OpenCL)
- **Версия hashcat / Version:** v5.1.0-1527-g80a87212
- **Источник / Source:** [Azunyan1111](https://gist.github.com/Azunyan1111/8133b6cf5e2f3f9a5b8f601609876cdd)
- **Примечание / Note:** нестандартный прогон — `hashcat -b -O --force -d 3` (оптимизированные ядра, `--force`, ограничение по устройству). На macOS часть режимов упала: 3200 (bcrypt) не собрался, ряд режимов отработал с предупреждением «OpenCL kernel self-test failed». Режимы 22000 и 2500 — в выводе присутствует 2500 (WPA-EAPOL-PBKDF2), 22000 отсутствует.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 10360.1 MH/s |
| 100 | SHA1 | 4037.0 MH/s |
| 1400 | SHA2-256 | 1624.7 MH/s |
| 1700 | SHA2-512 | 290.9 MH/s (self-test failed) |
| 1000 | NTLM | 15649.3 MH/s |
| 3200 | bcrypt | — (kernel build failed) |
| 1800 | sha512crypt | 35111 H/s (self-test failed) |
| 500 | md5crypt | 3976.5 kH/s |
| 2500 | WPA-EAPOL-PBKDF2 | 115.3 kH/s |
| 7500 | Kerberos AS-REQ (23) | 124.4 MH/s |
| 13100 | Kerberos TGS-REP (23) | 87836.0 kH/s |
| 11300 | Bitcoin wallet.dat | 1394 H/s (self-test failed) |
| 6211 | TrueCrypt RIPEMD160+XTS512 | 131.3 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
./hashcat -b -O --force -d 3
hashcat (v5.1.0-1527-g80a87212) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

You have enabled --force to bypass dangerous warnings and errors!
This can hide serious problems and should only be done when debugging.
Do not report hashcat issues encountered when using --force.
OpenCL API (OpenCL 1.2 (Nov  9 2019 04:32:50)) - Platform #1 [Apple]
====================================================================
* Device #1: Intel(R) Core(TM) i9-9980HK CPU @ 2.40GHz, skipped
* Device #2: Intel(R) UHD Graphics 630, skipped
* Device #3: AMD Radeon Pro 5500M Compute Engine, 4016/4080 MB (1020 MB allocatable), 24MCU

Benchmark relevant options:
===========================
* --force
* --backend-devices=3
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#3.........: 10360.1 MH/s (76.53ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

Hashmode: 100 - SHA1

Speed.#3.........:  4037.0 MH/s (48.64ms) @ Accel:32 Loops:1024 Thr:256 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#3.........:  1624.7 MH/s (58.52ms) @ Accel:32 Loops:512 Thr:256 Vec:1

Hashmode: 1700 - SHA2-512

* Device #3: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#3.........:   290.9 MH/s (83.83ms) @ Accel:128 Loops:32 Thr:256 Vec:1

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4095)

Speed.#3.........:   115.3 kH/s (51.96ms) @ Accel:4 Loops:1024 Thr:256 Vec:1

Hashmode: 1000 - NTLM

Speed.#3.........: 15649.3 MH/s (50.60ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

Hashmode: 3000 - LM

Speed.#3.........:  8522.2 MH/s (92.79ms) @ Accel:512 Loops:1024 Thr:64 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#3.........: 10679.1 MH/s (74.19ms) @ Accel:128 Loops:1024 Thr:256 Vec:1

Hashmode: 5600 - NetNTLMv2

Speed.#3.........:   719.6 MH/s (68.88ms) @ Accel:128 Loops:64 Thr:256 Vec:1

Hashmode: 1500 - descrypt, DES (Unix), Traditional DES

Speed.#3.........:   329.6 MH/s (74.69ms) @ Accel:4 Loops:1024 Thr:256 Vec:1

Hashmode: 500 - md5crypt, MD5 (Unix), Cisco-IOS $1$ (MD5) (Iterations: 1000)

Speed.#3.........:  3976.5 kH/s (93.97ms) @ Accel:128 Loops:500 Thr:256 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

clBuildProgram(): CL_BUILD_PROGRAM_FAILURE

SC failed. No reason given.
* Device #3: Kernel /Users/admin/go/src/github.com/hashcat/hashcat/OpenCL/m03200-pure.cl build failed - proceeding without this device.


Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

* Device #3: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#3.........:    35111 H/s (67.74ms) @ Accel:16 Loops:128 Thr:256 Vec:1

Hashmode: 7500 - Kerberos 5, etype 23, AS-REQ Pre-Auth

Speed.#3.........:   124.4 MH/s (49.77ms) @ Accel:128 Loops:32 Thr:64 Vec:1

Hashmode: 13100 - Kerberos 5, etype 23, TGS-REP

Speed.#3.........: 87836.0 kH/s (50.17ms) @ Accel:128 Loops:32 Thr:64 Vec:1

Hashmode: 15300 - DPAPI masterkey file v1 (Iterations: 23999)

* Device #3: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#3.........:    19472 H/s (51.80ms) @ Accel:4 Loops:1024 Thr:256 Vec:1

Hashmode: 15900 - DPAPI masterkey file v2 (Iterations: 12899)

* Device #3: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#3.........:     6850 H/s (67.49ms) @ Accel:2 Loops:512 Thr:256 Vec:1

Hashmode: 7100 - macOS v10.8+ (PBKDF2-SHA512) (Iterations: 1023)

* Device #3: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

Speed.#3.........:    99503 H/s (58.85ms) @ Accel:32 Loops:31 Thr:256 Vec:1

Hashmode: 11600 - 7-Zip (Iterations: 16384)

Speed.#3.........:   119.1 kH/s (49.63ms) @ Accel:32 Loops:512 Thr:256 Vec:1

Hashmode: 12500 - RAR3-hp (Iterations: 262144)

Speed.#3.........:    17796 H/s (83.01ms) @ Accel:4 Loops:16384 Thr:256 Vec:1

Hashmode: 13000 - RAR5 (Iterations: 32799)

Speed.#3.........:    17865 H/s (85.24ms) @ Accel:32 Loops:256 Thr:256 Vec:1

Hashmode: 6211 - TrueCrypt RIPEMD160 + XTS 512 bit (Iterations: 1999)

Speed.#3.........:   131.3 kH/s (92.30ms) @ Accel:32 Loops:128 Thr:256 Vec:1

Hashmode: 13400 - KeePass 1 (AES/Twofish) and KeePass 2 (AES) (Iterations: 24569)

Speed.#3.........:    12964 H/s (77.11ms) @ Accel:4 Loops:1024 Thr:256 Vec:1

Hashmode: 6800 - LastPass + LastPass sniffed (Iterations: 499)

Speed.#3.........:  1120.5 kH/s (66.10ms) @ Accel:64 Loops:124 Thr:256 Vec:1

Hashmode: 11300 - Bitcoin/Litecoin wallet.dat (Iterations: 200459)

* Device #3: ATTENTION! OpenCL kernel self-test failed.

Your device driver installation is probably broken.
See also: https://hashcat.net/faq/wrongdriver

```
