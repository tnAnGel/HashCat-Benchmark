# Intel Core i7-14700K — Hashcat v8.0.0 Python Bridge SHA-256 (partial)

- **CPU:** Intel Core i7-14700K.
- **Hashcat:** v8.0.0 release notes.
- **Режим:** 73000, SHA-256 Python plugin; 28 CPU threads.
- **Тип свидетельства:** официальный before/after report без raw stdout и подробностей повторов.
- **Источник:** [Hashcat v8.0.0 release notes, Python Bridge](https://github.com/hashcat/hashcat/blob/master/docs/releases_notes_v8.0.0.md#22-python-bridge).

| Состояние | Скорость |
|---|---:|
| Before | 16 kH/s |
| v8.0.0 | 611 kH/s |

Hashcat указывает, что результаты получены на Core i7-14700K. Это скорость встроенного Python Bridge SHA-256 plugin, не стандартного GPU/CPU `hashcat -b` режима и не прямая оценка throughput других hash-mode.
