# AMD Ryzen 9 9900X — Hashcat v7.0.0 Argon2 (official partial report)

- **CPU:** AMD Ryzen 9 9900X (12 cores / 24 threads per local CPU roster).
- **Hashcat:** v7.0.0.
- **Тип свидетельства:** два опубликованных значения в release notes Hashcat; исходный `hashcat -b` stdout и массив повторов не опубликованы.
- **Источник:** [Hashcat v7.0.0 release notes, Argon2 results](https://github.com/hashcat/hashcat/blob/master/docs/releases_notes_v7.0.0.md#22-argon2).
- **Дополнительный CPU-only результат:** [раздел CPU Speed](https://github.com/hashcat/hashcat/blob/master/docs/releases_notes_v7.0.0.md#310-cpu-speed) сообщает для mode 1000 скорость **свыше 10 GH/s** на Intel OpenCL runtime; точное число не приведено.

| Mode | Алгоритм / условия | Результат |
|---:|---|---:|
| 34000 | Argon2id, RFC 9106 recommended (`m=65536`, `t=3`, `p=1`) | 92 H/s |
| 70000 | Assimilation Bridge Argon2id reference implementation; параметры в заметке не уточнены | 109 H/s |
| 1000 | NTLM, Intel OpenCL runtime | >10 GH/s (порог, не точное значение) |

Hashcat указывает, что mode 34000 для этого CPU измерялся через Intel OpenCL runtime; для mode 70000 отмечена reference implementation с CPU SIMD. Это официальный обработанный отчёт, не сопоставимый напрямую с обычными `hashcat -b` строками.
