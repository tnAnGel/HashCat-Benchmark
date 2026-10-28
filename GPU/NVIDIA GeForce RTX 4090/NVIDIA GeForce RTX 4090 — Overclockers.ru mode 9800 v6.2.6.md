# NVIDIA GeForce RTX 4090 — Hashcat mode 9800

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GeForce RTX 4090
- **Конфигурация / Setup:** 1× and 2× RTX 4090; power limit 80% or 100%
- **Версия hashcat / Version:** v6.2.6
- **Источник / Source:** [Overclockers.ru — тема «Тестируем видеокарты в hashcat»](https://forums.overclockers.ru/viewtopic.php?f=31&t=626128), сообщение от 14.10.2023
- **Параметры / Options:** `hashcat -b -m 9800`; автор сравнивает CUDA off/on и power limit
- **Примечание / Note:** узкий тест одного режима (KeePass), не полный общий benchmark и не сопоставим напрямую с mode 0 в рейтинге.

## Результаты / Results

| GPU | Power limit | CUDA | Mode 9800 |
|-----|------------:|------|----------:|
| 1× RTX 4090 | 80% | off | 3399.9 MH/s |
| 1× RTX 4090 | 100% | off | 3409.1 MH/s |
| 1× RTX 4090 | 80% | 12.2 | 3576.2 MH/s |
| 1× RTX 4090 | 100% | 12.2 | 3609.9 MH/s |
| 2× RTX 4090 | 80% | 12.2 | 6965.7 MH/s |
| 2× RTX 4090 | 100% | 12.2 | 7273.9 MH/s |
