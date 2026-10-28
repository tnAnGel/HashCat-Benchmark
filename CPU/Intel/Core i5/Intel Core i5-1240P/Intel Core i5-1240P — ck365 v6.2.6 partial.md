# Intel Core i5-1240P

- **Вендор / Vendor:** Intel
- **Процессор / CPU:** Intel Core i5-1240P (12C/16T, Alder Lake-P)
- **Версия hashcat / Version:** v6.2.6
- **Бэкенд / Backend:** Intel OpenCL 3.0 Windows CPU device; смешанный тест с Intel UHD Graphics, CPU — `Device #2`
- **Источник / Source:** [hashcat forum — CPU can crack the password but GPU can't, benchmark output](https://hashcat.net/forum/thread-12544.html)
- **Параметры / Options:** `hashcat -b -m0 -D1,2 -d1,2`; optimized kernel
- **Статус / Status:** один режим; скорость CPU взята только из `Speed.#2`, GPU отдельно показал `Speed.#1`.

## Опубликованные результаты / Published results

| Mode | Алгоритм | Скорость CPU (`Speed.#2`) | Скорость GPU (`Speed.#1`, справочно) |
|-----:|----------|-------------------------:|-------------------------------------:|
| 0 | MD5 | 388.9 MH/s | 1526.9 MH/s |
