# NVIDIA GeForce GTX 1660 Ti

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce GTX 1660 Ti (Mobile / Laptop — система на ноутбучном CPU Intel Core i7-9750H)
- **Версия hashcat / Version:** v5.1.0-1447-gc4dd0206
- **Источник / Source:** [hashcat.net forum, thread-8777 (hiwire)](https://hashcat.net/forum/thread-8777.html)
- **Примечание / Note:** Устройство печатается как «GeForce GTX 1660 Ti» (мобильная версия печатается так же, как десктоп). Не полный прогон `hashcat -b`: приведён только один режим — 3200 (bcrypt), запущенный как `hashcat -b -m 3200`. Device #1 = CUDA GTX 1660 Ti (Device #2 CPU и Device #3 OpenCL-дубликат пропущены). Опция `--optimized-kernel-enable`.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 3200 | bcrypt | 12822 H/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v5.1.0-1447-gc4dd0206) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

/usr/local/share/hashcat/OpenCL/m03200-optimized.cl: Optimized kernel requested but not needed - falling back to pure kernel

* Device #1: WARNING! Kernel exec timeout is not disabled.
            This may cause "CL_OUT_OF_RESOURCES" or related errors.
            To disable the timeout, see: https://hashcat.net/q/timeoutpatch
* Device #3: WARNING! Kernel exec timeout is not disabled.
            This may cause "CL_OUT_OF_RESOURCES" or related errors.
            To disable the timeout, see: https://hashcat.net/q/timeoutpatch
nvmlDeviceGetFanSpeed(): Not Supported

CUDA API (CUDA 10.1)
====================
* Device #1: GeForce GTX 1660 Ti, 5391/5944 MB, 24MCU

OpenCL API (OpenCL 2.1 LINUX) - Platform #1 [Intel(R) Corporation]
==================================================================
* Device #2: Intel(R) Core(TM) i7-9750H CPU @ 2.60GHz, skipped

OpenCL API (OpenCL 1.2 CUDA 10.1.0) - Platform #2 [NVIDIA Corporation]
======================================================================
* Device #3: GeForce GTX 1660 Ti, skipped

Benchmark relevant options:
===========================
* --optimized-kernel-enable

Hashmode: 3200 - bcrypt $2*$, Blowfish (Unix) (Iterations: 32)

Speed.#1.........:    12822 H/s (43.13ms) @ Accel:2 Loops:32 Thr:12 Vec:1

Started: Mon Nov 18 17:36:01 2019
Stopped: Mon Nov 18 17:36:06 2019
```
