# AMD Radeon 760M Graphics

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon 760M Graphics
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [hashcat forum — thread 12463, LaptopPWR, 2025-01-10](https://hashcat.net/forum/thread-12463.html)

> Встроенная GPU (RDNA 3, Phoenix) в ноутбуке Lenovo ThinkPad P14s Gen 5 AMD. Автор запускал бенчмарк **только одного режима** (`-b -m 2500`), полного прогона нет; версия hashcat в самом выводе не печатается — v6.2.6 взята из пути `hashcat-6.2.6` в последней строке.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 2500 | WPA-EAPOL-PBKDF2 | 121.9 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
OpenCL API (OpenCL 2.1 AMD-APP (3584.0)) - Platform #1 [Advanced Micro Devices, Inc.]
=====================================================================================
* Device #1: AMD Radeon 760M Graphics, 8480/17087 MB (3780 MB allocatable), 4MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

The plugin 2500 is deprecated and was replaced with plugin 22000. For more details, please read: https://hashcat.net/forum/thread-10253.html

------------------------------------------------------
* Hash-Mode 2500 (WPA-EAPOL-PBKDF2) [Iterations: 4095]
------------------------------------------------------

Speed.#1.........:  121.9 kH/s (63.76ms) @ Accel:128 Loops:512 Thr:128 Vec:1

Started: Fri Jan 10 22:20:29 2025
Stopped: Fri Jan 10 22:20:36 2025

C:\Users\Home\Desktop\HASHCAT GG\hashcat-6.2.6>pause
```
