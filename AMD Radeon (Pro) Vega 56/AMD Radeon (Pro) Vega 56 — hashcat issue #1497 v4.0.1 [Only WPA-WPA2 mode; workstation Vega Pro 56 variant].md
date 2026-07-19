# AMD Radeon (Pro) Vega 56 (Only WPA/WPA2 mode; workstation Vega Pro 56 variant (gfx901))

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon (Pro) Vega 56
- **Конфигурация / Setup:** Only WPA/WPA2 mode; workstation Vega Pro 56 variant (gfx901)
- **Версия hashcat / Version:** v4.0.1
- **Источник / Source:** [hashcat issue #1497](https://github.com/hashcat/hashcat/issues/1497)

## Ключевые результаты / Highlights

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 2500 | WPA/WPA2 (legacy) | — |

## Полный вывод `hashcat -b` / Full benchmark output

```text
hashcat (v4.0.1) starting in benchmark mode...

OpenCL Platform [#1]: Advanced Micro Devices, Inc.
* Device [#1]: gfx901, 6732/8176 MB allocatable, 56MCU
* Device [#2]: Intel(R) Xeon(R) W-2140B CPU @ 3.20GHz, skipped.

Benchmark relevant options:
* --workload-profile=3

Hashmode: 2500 - WPA/WPA2

Speed.Dev.[#1].....: 352.0 kH/s (77.70ms)

macOS:

hashcat -m 2500 -w 3 -b
hashcat (v4.0.1) starting in benchmark mode...

OpenCL Platform [#1]: Apple
* Device [#1]: Intel(R) Xeon(R) W-2140B CPU @ 3.20GHz, skipped.
* Device [#2]: AMD Radeon Pro Vega 56 Compute Engine, 2044/8176 MB allocatable, 56MCU

Benchmark relevant options:
* --workload-profile=3

Hashmode: 2500 - WPA/WPA2

Speed.Dev.[#2].....: 199.8 kH/s (68.96ms)
```
