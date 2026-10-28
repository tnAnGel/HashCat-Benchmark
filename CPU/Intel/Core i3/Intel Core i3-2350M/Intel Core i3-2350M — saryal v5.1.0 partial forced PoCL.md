# Intel Core i3-2350M

- **Вендор / Vendor:** Intel
- **Процессор / CPU:** Intel Core i3-2350M @ 2.30GHz (2C/4T, Sandy Bridge)
- **Версия hashcat / Version:** v5.1.0
- **Бэкенд / Backend:** PoCL 1.4 OpenCL; `pthread-Intel(R) Core(TM) i3-2350M CPU`
- **Источник / Source:** [hashcat forum — Intel Integrated GPU, saryal](https://hashcat.net/forum/thread-9150.html)
- **Параметры / Options:** `-m 0 -b --force`; `--optimized-kernel-enable`
- **Статус / Status:** один режим, принудительный PoCL запуск; участник Hashcat Forum отдельно посоветовал не использовать `--force`, поэтому пометка сохранена.

## Опубликованный результат / Published result

| Mode | Алгоритм | Скорость |
|-----:|----------|---------:|
| 0 | MD5 | 97361.7 kH/s |
