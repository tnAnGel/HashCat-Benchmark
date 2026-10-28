# NVIDIA GRID K520

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** NVIDIA GRID K520 (4095 MB, 797 MHz, 8 MCU; AWS EC2 g2.2xlarge)
- **Версия hashcat / Version:** cudaHashcat v1.33
- **Источник / Source:** [hashcat forum — cudaHashCat64 on AWS EC2, Radical_Ronin, 2015-03-02](https://hashcat.net/forum/showthread.php?mode=threaded&pid=23603&tid=4143)
- **Статус / Status:** фрагмент опубликованного benchmark-mode запуска; ниже приведены отдельные режимы, не полный перечень.

## Выбранные опубликованные результаты / Selected published results

| Mode | Алгоритм | Скорость (Speed) |
|-----:|----------|------------------|
| 900 | MD4 | 4003.8 MH/s |
| 0 | MD5 | 2501.7 MH/s |
| 100 | SHA1 | 688.3 MH/s |
| 1400 | SHA256 | 296.4 MH/s |
| 1000 | NTLM | 4002.9 MH/s |
| 5600 | NetNTLMv2 | 179.6 MH/s |
| 2500 | WPA/WPA2 | 42815 H/s |
| 3200 | bcrypt | 501 H/s |

Исходный пост также подтверждает устройство через PCI ID: `NVIDIA Corporation GK104GL [GRID K520]`.
