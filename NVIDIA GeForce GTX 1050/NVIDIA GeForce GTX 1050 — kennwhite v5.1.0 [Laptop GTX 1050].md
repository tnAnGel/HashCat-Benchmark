# NVIDIA GeForce GTX 1050 (Laptop GTX 1050)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce GTX 1050
- **Конфигурация / Setup:** Laptop GTX 1050
- **Версия hashcat / Version:** v5.1.0
- **Источник / Source:** [kennwhite](https://github.com/kennwhite/hashcatbenchmark)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 5208.2 MH/s |
| 100 | SHA1 | 2043.0 MH/s |
| 1400 | SHA2-256 | 743.6 MH/s |
| 1700 | SHA2-512 | 249.2 MH/s |
| 1000 | NTLM | 8656.0 MH/s |
| 3200 | bcrypt | 3546 H/s |
| 1800 | sha512crypt | 39253 H/s |
| 2500 | WPA/WPA2 (legacy) | 100.8 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v5.1.0) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

OpenCL Platform #1: NVIDIA Corporation
======================================
* Device #1: GeForce GTX 1050, 1024/4096 MB allocatable, 5MCU

OpenCL Platform #2: Intel(R) Corporation
========================================
* Device #2: Intel(R) HD Graphics 630, skipped.
* Device #3: Intel(R) Core(TM) i7-7700HQ CPU @ 2.80GHz, skipped.

Benchmark relevant options:
===========================
* --benchmark-all
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#1.........:  5208.2 MH/s (63.22ms) @ Accel:256 Loops:256 Thr:1024 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........:  2043.0 MH/s (50.46ms) @ Accel:256 Loops:128 Thr:640 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........:  8656.0 MH/s (76.12ms) @ Accel:256 Loops:512 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:   743.6 MH/s (55.51ms) @ Accel:128 Loops:64 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:   249.2 MH/s (51.83ms) @ Accel:128 Loops:32 Thr:640 Vec:1

Hashmode: 1800 - sha512crypt $6$, SHA512 (Unix) (Iterations: 5000)

Speed.#1.........:    39253 H/s (51.33ms) @ Accel:512 Loops:128 Thr:32 Vec:1

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4096)

Speed.#1.........:   100.8 kH/s (50.10ms) @ Accel:128 Loops:32 Thr:1024 Vec:1

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:     3546 H/s (43.65ms) @ Accel:16 Loops:8 Thr:8 Vec:1

Hashmode: 5500 - NetNTLMv1 / NetNTLMv1+ESS

Speed.#1.........:  5192.8 MH/s (63.35ms) @ Accel:256 Loops:256 Thr:1024 Vec:1
```
