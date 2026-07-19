# NVIDIA Tesla V100 SXM2 16GB (8x rig)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA Tesla V100 SXM2 16GB
- **Конфигурация / Setup:** 8x rig
- **Версия hashcat / Version:** v4.1.0
- **Источник / Source:** [synch-cc](https://gist.github.com/synch-cc/a133ca2ffd5577ec9433299e138d4ce8)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 56113.3 MH/s |
| 100 | SHA1 | 17133.3 MH/s |
| 1400 | SHA2-256 | 7648.2 MH/s |
| 1700 | SHA2-512 | 2413.6 MH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
~~~~hashcat (v4.1.0) starting in benchmark mode...

OpenCL Platform #1: NVIDIA Corporation
======================================
* Device #1: Tesla V100-SXM2-16GB, 4040/16160 MB allocatable, 80MCU
* Device #2: Tesla V100-SXM2-16GB, 4040/16160 MB allocatable, 80MCU
* Device #3: Tesla V100-SXM2-16GB, 4040/16160 MB allocatable, 80MCU
* Device #4: Tesla V100-SXM2-16GB, 4040/16160 MB allocatable, 80MCU
* Device #5: Tesla V100-SXM2-16GB, 4040/16160 MB allocatable, 80MCU
* Device #6: Tesla V100-SXM2-16GB, 4040/16160 MB allocatable, 80MCU
* Device #7: Tesla V100-SXM2-16GB, 4040/16160 MB allocatable, 80MCU
* Device #8: Tesla V100-SXM2-16GB, 4040/16160 MB allocatable, 80MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.Dev.#1.....: 56113.3 MH/s (23.82ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#2.....: 56083.8 MH/s (23.83ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#3.....: 55950.2 MH/s (23.90ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#4.....: 55940.5 MH/s (23.89ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#5.....: 56028.0 MH/s (23.85ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#6.....: 56100.6 MH/s (23.82ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#7.....: 56041.6 MH/s (23.85ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#8.....: 56073.9 MH/s (23.84ms) @ Accel:16 Loops:1024 Thr:1024 Vec:4
Speed.Dev.#*.....:   448.3 GH/s

Hashmode: 100 - SHA1

Speed.Dev.#1.....: 17133.3 MH/s (78.25ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#2.....: 17133.7 MH/s (78.30ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#3.....: 17081.1 MH/s (78.49ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#4.....: 17075.1 MH/s (78.51ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#5.....: 17095.4 MH/s (78.39ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#6.....: 17133.4 MH/s (78.31ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#7.....: 17109.0 MH/s (78.38ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#8.....: 17117.0 MH/s (78.31ms) @ Accel:32 Loops:1024 Thr:512 Vec:1
Speed.Dev.#*.....:   136.9 GH/s

Hashmode: 1400 - SHA-256

Speed.Dev.#1.....:  7648.2 MH/s (87.63ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#2.....:  7648.1 MH/s (87.63ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#3.....:  7622.5 MH/s (87.92ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#4.....:  7649.6 MH/s (87.65ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#5.....:  7624.3 MH/s (87.87ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#6.....:  7631.8 MH/s (87.62ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#7.....:  7634.0 MH/s (87.84ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#8.....:  7631.7 MH/s (87.83ms) @ Accel:16 Loops:512 Thr:1024 Vec:1
Speed.Dev.#*.....: 61090.2 MH/s

Hashmode: 1700 - SHA-512

Speed.Dev.#1.....:  2413.6 MH/s (43.32ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#2.....:  2415.0 MH/s (43.32ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#3.....:  2406.1 MH/s (43.46ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#4.....:  2415.0 MH/s (43.33ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#5.....:  2408.7 MH/s (43.48ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#6.....:  2414.6 MH/s (43.32ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#7.....:  2407.9 MH/s (43.41ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#8.....:  2411.1 MH/s (43.38ms) @ Accel:32 Loops:64 Thr:640 Vec:1
Speed.Dev.#*.....: 19292.1 MH/s
```
