# NVIDIA Quadro P5000 — PKZIP benchmark fragments

- **Источники:** [Hashcat issue #2813](https://github.com/hashcat/hashcat/issues/2813), raw benchmark outputs.
- **Примечание:** устройство #2 явно идентифицировано как Quadro P5000. Режимы PKZIP не входят в основную сводную таблицу.

| Hashcat version | Mode | Speed.#2 |
|---|---:|---:|
| v6.2.1 | 17220 | 2929.7 MH/s |
| v6.2.1 | 17225 | 4126.7 MH/s |
| v6.2.6-851-g6716447df | 17220 | 9228.5 MH/s |
| v6.2.6-851-g6716447df | 17225 | 10918.5 MH/s |

```text
Hashmode: 17220 - PKZIP (Compressed)
Speed.#2.........: 2929.7 MH/s

Hashmode: 17225 - PKZIP (Mixed Multi-File)
Speed.#2.........: 4126.7 MH/s
```
