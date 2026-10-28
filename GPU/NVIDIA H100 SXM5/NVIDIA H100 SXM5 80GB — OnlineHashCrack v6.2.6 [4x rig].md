# NVIDIA H100 SXM 80GB (4x rig)

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA H100 SXM 80GB
- **Конфигурация / Setup:** 4 карты; `Speed.#*` — агрегат стенда
- **Версия hashcat / Version:** v6.2.6 (в оглавлении страницы указано v6.2.5; текст описания и фактический вывод — v6.2.6)
- **Источник / Source:** [OnlineHashCrack — полный вывод](https://www.onlinehashcrack.com/tools-benchmark-hashcat-nvidia-H100-SXM.php)
- **Параметры / Options:** `-b --benchmark-all -O -w 4`
- **Примечание / Note:** версия на странице указана противоречиво; сохранена версия из сырого вывода. Скорость — сумма четырёх карт.

## Результат / Result

```text
* Hash-Mode 0 (MD5)
Speed.#*.........: 483.7 GH/s
```
