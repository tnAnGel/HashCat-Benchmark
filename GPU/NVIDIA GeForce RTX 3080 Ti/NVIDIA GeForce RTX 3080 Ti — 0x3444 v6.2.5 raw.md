# NVIDIA GeForce RTX 3080 Ti Founder's Edition — hashcat v6.2.5 (raw benchmark)

- **Тип свидетельства:** полный опубликованный stdout `hashcat -b --benchmark-all`.
- **Устройство:** RTX 3080 Ti Founder's Edition 12 GB, 80 MCU; CUDA 11.6, драйвер 511.65.
- **Опции:** optimized kernel, workload profile 4.
- **Источник:** [0x3444 — исходный файл](https://github.com/0x3444/hashcat_benchmarks/blob/main/NVIDIA_GeForce_RTX_3080_Ti.txt) · [полный raw stdout](https://raw.githubusercontent.com/0x3444/hashcat_benchmarks/main/NVIDIA_GeForce_RTX_3080_Ti.txt).
- **Отличие от имеющихся данных:** уже есть v6.2.3 (OnlineHashCrack) и v6.2.6-813 (its5Q); этот отдельный Founder's Edition прогон v6.2.5 использует workload profile 4.

| Mode | Алгоритм | `Speed.#1` |
|---:|---|---:|
| 0 | MD5 | 28,857.5 MH/s |
| 100 | SHA1 | 14,562.5 MH/s |
| 1400 | SHA2-256 | 6,842.6 MH/s |
| 1700 | SHA2-512 | 2,613.7 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 1,066.5 kH/s |
| 1000 | NTLM | 36,493.9 MH/s |
| 3200 | bcrypt | 105.8 kH/s |

Результат MD5 отличается от других записей; сохраняю исходное значение и конфигурацию как опубликованы, без нормализации/пересчёта.
