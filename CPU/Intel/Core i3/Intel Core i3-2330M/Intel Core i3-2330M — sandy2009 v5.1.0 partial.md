# Intel Core i3-2330M

- **Вендор / Vendor:** Intel
- **Процессор / CPU:** Intel Core i3-2330M @ 2.20GHz (2C/4T, Sandy Bridge)
- **Версия hashcat / Version:** v5.1.0-1152-g62d5d2df
- **Бэкенд / Backend:** Intel OpenCL 2.1; PoCL устройство пропущено, результат `Speed.#2` относится к Intel CPU device
- **Источник / Source:** [hashcat forum — hashcat --benchmark, sandy2009](https://hashcat.net/forum/thread-8450.html)
- **Статус / Status:** неполный вывод; устройство PoCL также перечислено, но помечено `skipped`.

## Опубликованные результаты / Published results

| Mode | Алгоритм | Скорость (Speed.#2 = CPU) |
|-----:|----------|---------------------------:|
| 0 | MD5 | 20095.9 kH/s |
| 100 | SHA1 | 9659.3 kH/s |
| 1400 | SHA2-256 | 3659.5 kH/s |
| 1700 | SHA2-512 | 1119.6 kH/s |
| 1000 | NTLM | 36199.6 kH/s |
| 2500 | WPA-EAPOL-PBKDF2 | 428 H/s |
| 3200 | bcrypt | 284 H/s |
