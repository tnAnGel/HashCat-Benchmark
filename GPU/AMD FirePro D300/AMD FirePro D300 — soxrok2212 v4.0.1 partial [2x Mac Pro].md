# AMD FirePro D300

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon HD / FirePro D300 Compute Engine (2 устройства в Mac Pro)
- **Версия hashcat / Version:** v4.0.1-123-g2095e27d
- **Источник / Source:** [Hashcat Forum — AMD FirePro D300 Benchmark](https://hashcat.net/forum/thread-7242.html)
- **Параметры / Options:** `--force --optimized-kernel-enable`; Apple OpenCL
- **Примечание / Note:** опубликован широкий, но не гарантированно полный набор режимов. Скорость каждой карты — `Speed.Dev.#2/#3`; суммарные цифры пары не подменяют результат одной карты. Для bcrypt и DPAPI в логе есть предупреждения о провале kernel self-test, поэтому такие режимы не выделяю как надёжные.

## Ключевые результаты / Highlights

| Mode | Алгоритм | Одна карта |
|-----:|----------|-----------:|
| 0 | MD5 | 4.443 GH/s |
| 100 | SHA1 | 1.466 GH/s |
| 1400 | SHA-256 | 620.7 MH/s |
| 1700 | SHA-512 | 76.712 MH/s |
| 1000 | NTLM | 7.027 GH/s |
| 22000 | WPA2, 4096 iterations (legacy mode 2500) | 25.194 kH/s |

## Исходные строки / Raw excerpt

```text
Hashcat Version: 4.0.1-123-g2095e27d
OpenCL Platform #1: Apple
* Device #2: AMD Radeon HD - FirePro D300 Compute Engine, 512/2048 MB allocatable, 20MCU
* Device #3: AMD Radeon HD - FirePro D300 Compute Engine, 512/2048 MB allocatable, 20MCU
* --force
* --optimized-kernel-enable
Hashmode: 0 - MD5
Speed.Dev.#2.....: 4443.0 MH/s
Speed.Dev.#3.....: 4442.7 MH/s
Hashmode: 1000 - NTLM
Speed.Dev.#2.....: 7026.8 MH/s
Speed.Dev.#3.....: 7026.9 MH/s
```
