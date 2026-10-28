# Intel Core i7-14700K — Hashcat v7.0.0 Argon2 (official partial report)

- **CPU:** Intel Core i7-14700K (20 cores / 28 threads per local CPU roster).
- **Hashcat:** v7.0.0.
- **Тип свидетельства:** два опубликованных значения в release notes Hashcat; исходный `hashcat -b` stdout и массив повторов не опубликованы.
- **Источник:** [Hashcat v7.0.0 release notes, Argon2 results](https://github.com/hashcat/hashcat/blob/master/docs/releases_notes_v7.0.0.md#22-argon2).

| Mode | Алгоритм / условия | Результат |
|---:|---|---:|
| 34000 | Argon2id, RFC 9106 recommended (`m=65536`, `t=3`, `p=1`) | 96 H/s |
| 70000 | Assimilation Bridge Argon2id reference implementation; параметры в заметке не уточнены | 110 H/s |

В заметке Hashcat отдельно поясняет, что mode 34000 через OpenCL не использует современные CPU SIMD полностью, а mode 70000 использует reference implementation с SIMD. Это официальный обработанный отчёт, не сопоставимый напрямую с обычными `hashcat -b` строками.
