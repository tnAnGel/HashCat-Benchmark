# Intel Arc Pro B70 — OpenBenchmarking PTS Hashcat 7.1.2 (partial)

- **GPU:** Intel Arc Pro B70; результаты сравнения и масштабирования на 1–4 устройства.
- **Версия Hashcat:** 7.1.2 (`pts/hashcat-1.3.1`).
- **Тип свидетельства:** JSON-экспорт PTS с отдельными средними, массивами повторов и временем запусков; это не консольный raw stdout Hashcat.
- **Хост:** AMD Ryzen Threadripper 9980X 64-Core.
- **Результаты:** [Arc Pro B70 Initial Benchmarks](https://openbenchmarking.org/result/2604083-NE-INTELARCP47), [Arc Pro B70 Scaling](https://openbenchmarking.org/result/2605125-PTS-SCALING616).
- **Другие индивидуальные PTS-значения и повторы:** [карточка OpenBenchmarking](<Intel Arc Pro B70 — OpenBenchmarking PTS results.md>) — связанные device labels сохранены отдельными строками.

| Hashcat mode | Hash type | 1× B70 | 2× B70 | 3× B70 | 4× B70 |
|---:|---|---:|---:|---:|---:|
| 0 | MD5 | 38.7413 GH/s | — | — | — |
| 1000 | NTLM | 67.1046 GH/s | 99.9838 GH/s | 134.408 GH/s | 133.417 GH/s |
| 1400 | SHA2-256 | 6.6053 GH/s | 13.0780 GH/s | 19.6615 GH/s | 19.6122 GH/s |
| 1700 | SHA2-512 | 990.2 MH/s | 2.7032 GH/s | 4.0547 GH/s | 4.0178 GH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 940.8 kH/s | 1.8860 MH/s | 2.8380 MH/s | 2.8284 MH/s |
| 11600 | 7-Zip | 267.567 kH/s | 528.933 kH/s | 794.733 kH/s | 780.533 kH/s |

Значения 2×/3×/4× — результаты многокарточных установок, не скорость одной карты. PTS использует заявленные system labels для количества GPU; не экстраполировать линейное масштабирование: в тесте 4× некоторые режимы немного медленнее 3×.
