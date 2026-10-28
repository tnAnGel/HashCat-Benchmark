# Intel Arc A770

- **Вендор / Vendor:** Intel
- **Видеокарта / GPU:** Intel(R) Arc(TM) A770 Graphics (8 GB)
- **Версия hashcat / Version:** v6.2.6-853-g6472ed240 (git build)
- **Источник / Source:** [RealEnder — hashcat issue #4356](https://github.com/hashcat/hashcat/issues/4356)
- **Примечание / Note:** Неполный прогон — запускался только один режим (`hashcat -b -m22000`), полного бенчмарка по всем хеш-модам в источнике нет.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 22000 | WPA-PBKDF2 (PMKID/EAPOL) | 538.1 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
$ ./hashcat -b -m22000
hashcat (v6.2.6-853-g6472ed240) starting in benchmark mode

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

OpenCL API (OpenCL 3.0 ) - Platform #1 [Intel(R) Corporation]
=============================================================
* Device #1: Intel(R) Arc(TM) A770 Graphics, 7616/7721 MB (3860 MB allocatable), 512MCU

Benchmark relevant options:
===========================
* --backend-devices-virtual=1
* --optimized-kernel-enable

-------------------------------------------------------------
* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
-------------------------------------------------------------

Speed.#1.........:   538.1 kH/s (59.66ms) @ Accel:128 Loops:128 Thr:16 Vec:1

Started: Wed Jul 23 20:32:08 2025
Stopped: Wed Jul 23 20:32:23 2025
```
