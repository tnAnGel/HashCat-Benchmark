# AMD Radeon R9 270X

- **Вендор / Vendor:** AMD
- **Видеокарта / GPU:** AMD Radeon R9 270X (указана автором поста; device line не опубликована)
- **Версия / Version:** oclHashcat (контекст треда — v1.01; версия этого ответа отдельно не подтверждена)
- **Источник / Source:** [Hashcat Forum — oclhashcat 1.01 benchmarks fail AMD Radeon 7970, ответ с R9 270X](https://hashcat.net/forum/thread-3119.html)
- **Параметры / Options:** встроенный benchmark; упомянуты WHQL 13.12 и SDK 2.9
- **Примечание / Note:** только два режима из запуска, затем `clEnqueueNDRangeKernel() -4`. Автор прямо называет R9 270X, но в опубликованном фрагменте нет строки `Device #N`; считать частичным и несколько менее надёжно идентифицированным свидетельством.

## Результаты / Results

| Алгоритм | Скорость |
|----------|---------:|
| SSHA-1 | 1772.0 MH/s |
| DES (Unix) | 60941.9 kH/s |

## Исходные строки / Raw excerpt

```text
Trying out oclhashcat ... benchmark ... on R9 270X, WHQL 13.12 drivers and SDK 2.9.
Hashtype: SSHA-1(Base64), nsldaps, Netscape LDAP SSHA
Speed.GPU.#1.: 1772.0 MH/s
Hashtype: descrypt, DES (Unix), Traditional DES
Speed.GPU.#1.: 60941.9 kH/s
ERROR: clEnqueueNDRangeKernel() -4
```
