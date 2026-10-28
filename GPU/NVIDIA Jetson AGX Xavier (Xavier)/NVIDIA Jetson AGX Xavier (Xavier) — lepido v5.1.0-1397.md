# NVIDIA Jetson AGX Xavier (Xavier)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA Jetson AGX Xavier (Xavier)
- **Версия hashcat / Version:** v5.1.0-1397-g7f4df9eb+
- **Источник / Source:** [hashcat forum — thread 8355, lepido, 2019-09-26](https://hashcat.net/forum/thread-8355.html)

> Режим питания `nvpmodel -m 0` (30 Вт). Автор опубликовал **неполный** вывод — только шесть режимов (0, 100, 1400, 1700, 2500, 1000); других строк `Speed` в исходном посте нет.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 4666.5 MH/s |
| 100 | SHA1 | 1548.2 MH/s |
| 1400 | SHA2-256 | 670.5 MH/s |
| 1700 | SHA2-512 | 217.4 MH/s |
| 1000 | NTLM | 7027.2 MH/s |
| 2500 | WPA-EAPOL-PBKDF2 | 72302 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v5.1.0-1397-g7f4df9eb+) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

clGetPlatformIDs(): CL_PLATFORM_NOT_FOUND_KHR

CUDA API (CUDA 10.0)
====================
* Device #1: Xavier, 15698 MB, 8MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#1.........:  4666.5 MH/s (57.07ms) @ Accel:32 Loops:1024 Thr:1024 Vec:1

Hashmode: 100 - SHA1

Speed.#1.........:  1548.2 MH/s (86.25ms) @ Accel:32 Loops:512 Thr:1024 Vec:1

Hashmode: 1400 - SHA2-256

Speed.#1.........:  670.5 MH/s (49.61ms) @ Accel:8 Loops:512 Thr:1024 Vec:1

Hashmode: 1700 - SHA2-512

Speed.#1.........:  217.4 MH/s (76.74ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 2500 - WPA-EAPOL-PBKDF2 (Iterations: 4095)

Speed.#1.........:    72302 H/s (56.39ms) @ Accel:8 Loops:256 Thr:1024 Vec:1

Hashmode: 1000 - NTLM

Speed.#1.........:  7027.2 MH/s (75.98ms) @ Accel:64 Loops:1024 Thr:1024 Vec:1
```
