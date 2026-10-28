# NVIDIA GeForce GTX 760

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce GTX 760 (2048 MB, 1137 MHz, 6 MCU)
- **Версия hashcat / Version:** cudaHashcat v1.35–v1.37
- **Источник / Source:** [hashcat forum — oclHashcat v1.36 slow on Windows 10, rico](https://hashcat.net/forum/printthread.php?tid=4612)
- **Система / System:** Windows 7 x64 для v1.35; Windows 10 x64 для v1.36/v1.37
- **Статус / Status:** частичные результаты; в источнике также описаны ошибки драйвера для отдельных режимов.

## Опубликованные успешные результаты / Published successful results

| Version | Mode | Алгоритм | Скорость (Speed) |
|---------|-----:|----------|------------------|
| v1.35 | 2500 | WPA/WPA2 | 47594 H/s |
| v1.36 | 2500 | WPA/WPA2 | 32606 H/s |
| v1.37 | 2500 | WPA/WPA2 | 47745 H/s |
| v1.37 | 100 | SHA1 | 736.0 MH/s |
| v1.37 | 5600 | NetNTLMv2 | 202.0 MH/s |

Неудачные запуски `-m 5600` с ошибкой `cuStreamSynchronize()` результатами не считаются.
