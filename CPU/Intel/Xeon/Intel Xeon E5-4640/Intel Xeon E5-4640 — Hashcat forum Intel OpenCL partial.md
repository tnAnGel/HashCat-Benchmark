# Intel Xeon E5-4640 — Hashcat Forum Intel OpenCL (partial)

- **CPU:** Intel Xeon E5-4640 @ 2.40 GHz; автор сообщает о системе с **4 CPU**. Скорость относится к этому много-сокетному узлу, не к одному процессору.
- **Hashcat version:** не указана для строки результата. В предыдущем неуспешном выводе показан v6.2.4, но это не подтверждает версию успешного прогона.
- **Backend:** Intel CPU Runtime for OpenCL; автор пишет, что заработало после установки Intel OpenCL 16.1.1.
- **Hash mode:** автор говорит о DES hashes, но номер режима и аргументы в опубликованном фрагменте отсутствуют; не приписывать автоматически mode 1500.
- **Источник:** [Hashcat Forum — Hashcat and OpenCL installation issue xeon E5-4640](https://hashcat.net/forum/thread-10534.html), посты #1 и #3.
- **Тип свидетельства:** одна опубликованная строка скорости, не полный raw stdout.

```text
Speed.#1.........: 17643.3 kH/s (58.78ms) @ Accel:16 Loops:1024 Thr:1 Vec:4
```

Успешный прогон приведён после сообщения автора о четырёх E5 CPUs и исправлении OpenCL runtime. Устройство в предыдущем `-I` выводе — один Intel Xeon E5-4640 CPU backend с 64 MCU. Оставлять как partial и не сравнивать напрямую с обычным одно-сокетным `hashcat -b`.
