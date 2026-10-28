# AMD Radeon HD 7970

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon HD 7970 (Tahiti, 2 GB, 925 MHz, 32 MCU)
- **Версия / Version:** oclHashcat v1.01 (legacy benchmark)
- **Источник / Source:** [Hashcat Forum — oclhashcat 1.01 benchmarks fail AMD Radeon 7970](https://hashcat.net/forum/thread-3119.html)
- **Параметры / Options:** `oclhashcat64.exe -b`; Windows
- **Примечание / Note:** частичный legacy benchmark: после множества успешных режимов запуск завершился `clEnqueueNDRangeKernel() -4`. В авторском посте есть ещё отдельные режимы, запущенные по одному; модель и скорости подтверждены, но это не полный успешный `-b`.

## Ключевые результаты / Highlights

| Алгоритм | Скорость |
|----------|---------:|
| MD4 | 16.054 GH/s |
| MD5 | 8.015 GH/s |
| SHA1 | 2.516 GH/s |
| SHA256 | 1.010 GH/s |
| NTLM | 15.481 GH/s |

## Исходные строки / Raw excerpt

```text
oclHashcat v1.01 starting in benchmark-mode...
Device #1: Tahiti, 2048MB, 925Mhz, 32MCU
Hashtype: MD4
Speed.GPU.#1.: 16053.9 MH/s
Hashtype: MD5
Speed.GPU.#1.: 8014.7 MH/s
Hashtype: SHA1
Speed.GPU.#1.: 2516.3 MH/s
Hashtype: SHA256
Speed.GPU.#1.: 1009.6 MH/s
Hashtype: NTLM
Speed.GPU.#1.: 15480.5 MH/s
ERROR: clEnqueueNDRangeKernel() -4
```
