# AMD Ryzen 7 3700X — benchmark fragment

- **Процессор:** AMD Ryzen 7 3700X.
- **Версия:** hashcat v6.2.2.
- **Запуск:** `hashcat -m 0 -D 1 -b`.
- **Режим:** MD5 (mode 0), CPU `Speed.#1 1363.5 MH/s`.
- **Источник:** [Hashcat issue #3021](https://github.com/hashcat/hashcat/issues/3021).
- **Примечание:** backend device назван `pthread-AMD Ryzen 7 3700X`; Radeon RX 580 явно `skipped`, поэтому измерение относится к CPU.

```text
* Device #1: pthread-AMD Ryzen 7 3700X
* Device #2: AMD Radeon RX 580, skipped

* Hash-Mode 0 (MD5)
Speed.#1.........: 1363.5 MH/s
```
