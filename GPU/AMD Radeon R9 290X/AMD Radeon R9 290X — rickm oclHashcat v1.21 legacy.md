# AMD Radeon R9 290X

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon R9 290X (Hawaii, 3 GB)
- **Версия / Version:** oclHashcat v1.21 (legacy benchmark)
- **Источник / Source:** [Hashcat Forum — AMD Radeon R9 290X speed and noise](https://hashcat.net/forum/thread-3510.html)
- **Параметры / Options:** встроенный benchmark; Catalyst 14.10, od6config
- **Примечание / Note:** исторический формат `Speed.GPU.#1`, не современный `hashcat -b`. Автор прямо пишет, что устройство — AMD R9 290X; Hashcat выводит codename Hawaii. В отдельной [теме-сравнении](https://hashcat.net/forum/thread-2798.html) опубликованы более поздние результаты после Catalyst 13.12, а также отмечены драйверные/температурные факторы.

## Ключевые результаты / Highlights

| Алгоритм | Скорость |
|----------|---------:|
| MD4 | 23.189 GH/s |
| MD5 | 11.552 GH/s |
| SHA1 | 3.699 GH/s |
| SHA256 | 1.531 GH/s |
| SHA512 | 241.7 MH/s |

## Исходные строки / Raw excerpt

```text
I acquired a AMD R9 290X ... last version of oclHashcat (1.21)
Device #1: Hawaii, 3072MB, 1000Mhz, 44MCU
Hashtype: MD4
Speed.GPU.#1.: 23188.8 MH/s
Hashtype: MD5
Speed.GPU.#1.: 11552.2 MH/s
Hashtype: SHA1
Speed.GPU.#1.: 3698.8 MH/s
Hashtype: SHA256
Speed.GPU.#1.: 1531.1 MH/s
Hashtype: SHA512
Speed.GPU.#1.: 241.7 MH/s
```
