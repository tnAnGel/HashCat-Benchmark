# NVIDIA Tesla P100 (4x rig (GCP), run crashed at DES — only MD4/MD5 complete)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA Tesla P100
- **Конфигурация / Setup:** 4x rig (GCP), run crashed at DES — only MD4/MD5 complete
- **Версия hashcat / Version:** v4.0.1
- **Источник / Source:** [hashcat issue #1489](https://github.com/hashcat/hashcat/issues/1489)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 22002.1 MH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v4.0.1) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

nvmlDeviceGetFanSpeed(): Not Supported
nvmlDeviceGetFanSpeed(): Not Supported
nvmlDeviceGetFanSpeed(): Not Supported
nvmlDeviceGetFanSpeed(): Not Supported

OpenCL Platform #1: NVIDIA Corporation
======================================
* Device #1: Tesla P100-PCIE-16GB, 4069/16276 MB allocatable, 56MCU
* Device #2: Tesla P100-PCIE-16GB, 4069/16276 MB allocatable, 56MCU
* Device #3: Tesla P100-PCIE-16GB, 4069/16276 MB allocatable, 56MCU
* Device #4: Tesla P100-PCIE-16GB, 4069/16276 MB allocatable, 56MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

Hashmode: 900 - MD4

Speed.Dev.#1.....: 38020.5 MH/s (49.50ms)
Speed.Dev.#2.....: 36984.0 MH/s (49.54ms)
Speed.Dev.#3.....: 37955.2 MH/s (49.50ms)
Speed.Dev.#4.....: 37892.4 MH/s (49.62ms)
Speed.Dev.#*.....:   150.9 GH/s

Hashmode: 0 - MD5

Speed.Dev.#1.....: 22002.1 MH/s (85.46ms)
Speed.Dev.#2.....: 20740.3 MH/s (85.41ms)
Speed.Dev.#3.....: 20354.1 MH/s (85.41ms)
Speed.Dev.#4.....: 21645.3 MH/s (85.36ms)
Speed.Dev.#*.....: 84741.8 MH/s

... (does some more benchmarks and eventually reaches DES)

Hashmode: 14000 - DES (PT = $salt, key = $pass)

user@nvidia-p100-test:~/hashcat-4.0.1$
```
