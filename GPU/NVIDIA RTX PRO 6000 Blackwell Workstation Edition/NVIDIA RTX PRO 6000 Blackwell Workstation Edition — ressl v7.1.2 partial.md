# NVIDIA RTX PRO 6000 Blackwell Workstation Edition

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** RTX PRO 6000 Blackwell Workstation Edition, 2 устройства
- **Версия / Version:** Hashcat v7.1.2
- **Источник / Source:** [ressl — raw benchmark output](https://gist.github.com/ressl/2cee75aa14d3b770ae9f6b0e0a7ec3fc)
- **Тип данных / Evidence:** опубликованный raw benchmark-mode log, частичный набор режимов
- **Backend:** CUDA RTC не инициализировалась; Hashcat переключился на OpenCL

## Результаты на каждую карту

| Mode | Алгоритм | Device #01 | Device #02 | Суммарно 2 GPU |
|---:|---|---:|---:|---:|
| 900 | MD4 | 440.6 GH/s | 436.5 GH/s | 877.1 GH/s |
| 0 | MD5 | 251.0 GH/s | 249.1 GH/s | 500.1 GH/s |
| 100 | SHA1 | 85.802 GH/s | 85.6323 GH/s | 171.4 GH/s |
| 1400 | SHA-256 | 32.8153 GH/s | 32.8930 GH/s | 65.7083 GH/s |
| 1700 | SHA-512 | 10.7208 GH/s | 10.6885 GH/s | 21.4093 GH/s |

В таблице явно сохранены и скорости отдельных устройств, и агрегат двух GPU;
агрегированную цифру нельзя трактовать как скорость одной карты. В присланном
логе отсутствует mode 23800, поэтому это не полный all-mode отчёт.
