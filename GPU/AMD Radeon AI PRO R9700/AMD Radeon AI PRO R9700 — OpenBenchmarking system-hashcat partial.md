# AMD Radeon AI PRO R9700 — OpenBenchmarking system/hashcat (partial)

- **GPU:** XFX AMD Radeon AI Pro R9700 8GB (PTS system label; clocks reported as 210/405 MHz).
- **Версия Hashcat:** 7.1.2, профиль `system/hashcat-1.0.0`.
- **Тип свидетельства:** отдельные PTS JSON result-файлы с массивами повторов; это не raw stdout Hashcat.
- **Хост:** AMD Ryzen 9 9950X3D2 16-Core.
- **Источники:** [SHA-512 / mode 1700](https://openbenchmarking.org/result/2608162-NE-HASHCATSH47), [SHA2-256 / mode 1400](https://openbenchmarking.org/result/2608164-NE-HASHCATSH76), [7-Zip / mode 11600](https://openbenchmarking.org/result/2608169-NE-HASHCAT7Z12), [Kerberos 5 TGS-REP / mode 13100](https://openbenchmarking.org/result/2608169-NE-HASHCATKE77).
- **Другие индивидуальные PTS-значения и повторы:** [карточка OpenBenchmarking](<AMD Radeon AI PRO R9700 — OpenBenchmarking PTS results.md>); профиль и тип данных сохранены в этой карточке.

| Mode | Тип хеша | Среднее PTS |
|---:|---|---:|
| 1400 | SHA2-256 | 14.1439 GH/s |
| 1700 | SHA2-512 | 3.50903 GH/s |
| 11600 | 7-Zip | 1.78987 MH/s |
| 13100 | Kerberos 5 TGS-REP | 1.94917 GH/s |

Это подтверждает несколько режимов для модели, но не полный `hashcat -b`; не объединять с агрегатами PTS в качестве raw-прогона.
