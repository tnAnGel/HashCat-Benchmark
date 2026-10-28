# AMD Instinct MI50

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Instinct MI50 (четыре карты; Hashcat/backend показывает семейное имя `MI60 / MI50`)
- **Версия hashcat / Version:** в опубликованном фрагменте не указана
- **Источник / Source:** [Benchmarking the Instinct MI50 in 2026 — сырой вывод и конфигурация](https://diegostrebel.com/posts/mi50_benchmarks/)
- **Параметры / Options:** benchmark-all; `--optimized-kernel-enable`; HIP и OpenCL
- **Примечание / Note:** автор указывает 4× MI50, ROCm 6.4.3 и NixOS 25.11. Опубликован широкий фрагмент сырого вывода по многим режимам; точный SKU каждого устройства backend не различает. Табличные результаты ниже — скорость одной карты (`Speed.#01`), не суммарный результат четырёх устройств.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Одна карта | 4 карты, сумма |
|-----:|----------|-----------:|---------------:|
| 0 | MD5 | 31.791 GH/s | 128.2 GH/s |
| 1000 | NTLM | 49.817 GH/s | 199.9 GH/s |
| 1400 | SHA2-256 | см. источник | 20.027 GH/s |
| 1700 | SHA2-512 | см. источник | 4.552 GH/s |
| 22000 | WPA2-PMKID+EAPOL | 585.2 kH/s | 2343.5 kH/s |
| 3200 | bcrypt | см. источник | 100.4 kH/s |

## Исходные строки / Raw excerpt

```text
OpenCL API (OpenCL 2.1 AMD-APP (3649.0))
* Device #01: AMD Instinct MI60 / MI50, 16368/16368 MB, 60MCU
* Device #02: AMD Instinct MI60 / MI50, 16368/16368 MB, 60MCU
* Device #03: AMD Instinct MI60 / MI50, 16368/16368 MB, 60MCU
* Device #04: AMD Instinct MI60 / MI50, 16368/16368 MB, 60MCU

* Hash-Mode 0 (MD5)
Speed.#01........: 31791.0 MH/s
Speed.#*.........: 128.2 GH/s

* Hash-Mode 1000 (NTLM)
Speed.#01........: 49816.8 MH/s
Speed.#*.........: 199.9 GH/s

* Hash-Mode 22000 (WPA-PBKDF2-PMKID+EAPOL) [Iterations: 4095]
Speed.#01........: 585.2 kH/s
Speed.#*.........: 2343.5 kH/s
```
