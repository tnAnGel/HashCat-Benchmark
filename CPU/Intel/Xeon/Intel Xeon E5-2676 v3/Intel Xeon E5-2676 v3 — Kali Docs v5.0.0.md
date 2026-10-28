# Intel Xeon E5-2676 v3

- **Вендор / Vendor:** Intel
- **Процессор / CPU:** Intel Xeon E5-2676 v3 @ 2.40GHz (Haswell-EP)
- **Версия hashcat / Version:** v5.0.0
- **Бэкенд / Backend:** OpenCL Platform #2 `Intel(R) Corporation` (нативный Intel OpenCL runtime), устройство `Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz` — Device #2. Платформа #1 `The pocl project` (`pthread-...`) была `skipped`.
- **Источник / Source:** [Kali Linux Tools — hashcat](https://www.kali.org/tools/hashcat/)
- **Примечание / Note:** ЧАСТИЧНЫЙ вывод — официальный пример из документации Kali обрезан на 3 режимах (`[...]`). GPU в системе нет: оба перечисленных устройства — один и тот же CPU (E5-2676 v3, классический AWS EC2 Xeon). Замеры сняты на Device #2 (Intel OpenCL); pocl-устройство `pthread` пропущено. Все строки Speed имеют полный тюнинг (`@ Accel/Loops/Thr/Vec` + мс). Запуск с `--optimized-kernel-enable`.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 0 | MD5 | 134.9 MH/s |
| 100 | SHA1 | 98899.4 kH/s |
| 1400 | SHA2-256 | 42768.3 kH/s |

## Полный вывод `hashcat -b` / Full benchmark output

```text
root@kali:~# hashcat -b
hashcat (v5.0.0) starting in benchmark mode...

Benchmarking uses hand-optimized kernel code by default.
You can use it in your cracking session by setting the -O option.
Note: Using optimized kernel code limits the maximum supported password length.
To disable the optimized kernel code in benchmark mode, use the -w option.

* Device #1: Not a native Intel OpenCL runtime. Expect massive speed loss.
             You can use --force to override, but do not report related errors.
OpenCL Platform #1: The pocl project
====================================
* Device #1: pthread-Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz, skipped.

OpenCL Platform #2: Intel(R) Corporation
========================================
* Device #2: Intel(R) Xeon(R) CPU E5-2676 v3 @ 2.40GHz, 986/3946 MB allocatable, 2MCU

Benchmark relevant options:
===========================
* --optimized-kernel-enable

Hashmode: 0 - MD5

Speed.#2.........:   134.9 MH/s (15.41ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 100 - SHA1

Speed.#2.........: 98899.4 kH/s (21.04ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8

Hashmode: 1400 - SHA2-256

Speed.#2.........: 42768.3 kH/s (48.86ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8
[...]
```
