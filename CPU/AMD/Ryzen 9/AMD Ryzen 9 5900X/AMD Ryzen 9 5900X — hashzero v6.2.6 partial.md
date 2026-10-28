# AMD Ryzen 9 5900X

- **Вендор / Vendor:** AMD
- **Процессор / CPU:** AMD Ryzen 9 5900X 12-Core Processor (12C/24T, Zen 3)
- **Версия hashcat / Version:** v6.2.6
- **Бэкенд / Backend:** OpenCL 3.0 Windows CPU device; Radeon RX 6700 XT был `skipped`
- **Источник / Source:** [hashcat forum — Benchmark request for DDR5 CPUs, hashzero](https://hashcat.net/forum/thread-12413.html)
- **Параметры / Options:** `hashcat -b -m 15700 -D 1`; optimized kernel; 32 GB DDR4
- **Статус / Status:** один CPU-only hash mode; два замера при разных профилях памяти.

## Опубликованные результаты / Published results

| Mode | Алгоритм | Память | Скорость |
|-----:|----------|--------|---------:|
| 15700 | Ethereum Wallet, SCRYPT | DDR4-2133 (XMP выключен) | 27 H/s |
| 15700 | Ethereum Wallet, SCRYPT | DDR4-3600 (XMP включён) | 41 H/s |
