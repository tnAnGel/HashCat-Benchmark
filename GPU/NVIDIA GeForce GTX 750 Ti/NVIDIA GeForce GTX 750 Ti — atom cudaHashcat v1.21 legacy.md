# NVIDIA GeForce GTX 750 Ti

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** Zotac GeForce GTX 750 Ti, 2 GB, 5 MCU
- **Версия / Version:** cudaHashcat v1.21 (legacy benchmark)
- **Источник / Source:** [Hashcat Forum — GTX 750 TI, автор atom](https://hashcat.net/forum/showthread.php?mode=threaded&pid=19577&tid=3404)
- **Параметры / Options:** `benchmark-mode`; workload указан в логе
- **Примечание / Note:** полный старый формат вывода `Speed.GPU.#1`, не современный `hashcat -b`. Автор — администратор Hashcat; отмечает, что релизная ветка добавляла низкоуровневые оптимизации Maxwell `sm_50`. Сохраняю как исторический результат, не смешивая напрямую с текущими прогонами.

## Ключевые результаты / Highlights

| Алгоритм | Скорость |
|----------|---------:|
| MD4 | 5.538 GH/s |
| MD5 | 3.023 GH/s |
| SHA1 | 1.065 GH/s |
| SHA256 | 408.5 MH/s |
| bcrypt | 1915 H/s |
| NTLM | 5.186 GH/s |

## Исходные строки / Raw excerpt

```text
cudaHashcat v1.21 starting in benchmark-mode...
Device #1: GeForce GTX 750 Ti, 2047MB, 1110Mhz, 5MCU
Hashtype: MD4
Speed.GPU.#1.: 5537.8 MH/s
Hashtype: MD5
Speed.GPU.#1.: 3022.7 MH/s
Hashtype: SHA1
Speed.GPU.#1.: 1065.3 MH/s
Hashtype: SHA256
Speed.GPU.#1.: 408.5 MH/s
Hashtype: NTLM
Speed.GPU.#1.: 5185.9 MH/s
```
