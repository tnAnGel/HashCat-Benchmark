# AMD Instinct MI250X / MI250

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Instinct MI250X/MI250 (8 устройств в сервере; SKU в логе неразличима)
- **Версия hashcat / Version:** v6.2.6 (OpenCL)
- **Источник / Source:** [Hashcat Forum — AMD MI250 Instinct, полный stdout одного режима](https://hashcat.net/forum/thread-11889.html)
- **Параметры / Options:** `./hashcat -b -w4 -m1000`
- **Примечание / Note:** опубликован только NTLM (`-m 1000`), не полный `--benchmark-all`. HIP-вариант не собрал kernel (`HIPRTC_ERROR_COMPILATION`); приведён ниже рабочий OpenCL-прогон. Скорость на одну карту — строка `Speed.#1`; `Speed.#*` — восемь карт вместе. Hashcat и автор указывают семейство MI250X/MI250, без однозначной версии SKU.

## Результат / Result

| Mode | Алгоритм | Одна карта (диапазон) | 8 карт, сумма |
|-----:|----------|----------------------:|--------------:|
| 1000 | NTLM | 9.333–9.577 GH/s | 75.718 GH/s |

## Исходный вывод / Raw output

```text
hashcat (v6.2.6) starting in benchmark mode
OpenCL API (OpenCL 2.1 AMD-APP (3602.0))
* Device #1: AMD Instinct MI250X/MI250, 65408/65520 MB, 104MCU
...
* Device #8: AMD Instinct MI250X/MI250, 65408/65520 MB, 104MCU

* Hash-Mode 1000 (NTLM)
Speed.#1.........:  9333.3 MH/s (93.23ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#2.........:  9431.5 MH/s (92.30ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#3.........:  9415.0 MH/s (92.50ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#4.........:  9549.7 MH/s (91.21ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#5.........:  9576.7 MH/s (90.92ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#6.........:  9520.6 MH/s (91.46ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#7.........:  9513.1 MH/s (91.52ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#8.........:  9377.8 MH/s (92.81ms) @ Accel:128 Loops:1024 Thr:64 Vec:1
Speed.#*.........: 75717.6 MH/s
```
