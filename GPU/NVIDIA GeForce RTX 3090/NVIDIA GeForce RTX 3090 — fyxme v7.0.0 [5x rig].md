# NVIDIA GeForce RTX 3090 (5x rig) — hashcat v7.0.0 (raw benchmark)

- **Тип свидетельства:** полный raw stdout benchmark mode, опубликованный в GitHub Gist.
- **Конфигурация:** 5 × RTX 3090; таблица содержит индивидуальные `Speed.#01–#05` и суммарный `Speed.#*`. Ниже отдельно приведены карта #01 и итог стенда.
- **Hashcat / runtime:** v7.0.0, CUDA 12.9; команда `hashcat -w 4 -O -b`; workload profile 4.
- **Дата публикации:** 2025-08-18.
- **Источник:** [Gist — описание и raw benchmark](https://gist.github.com/fyxme/bac0a4144d196c779cda545122f1539a/78dd215d03da8fc7cdbc54b02f93143d50917a8f) · [raw stdout](https://gist.githubusercontent.com/fyxme/bac0a4144d196c779cda545122f1539a/raw/78dd215d03da8fc7cdbc54b02f93143d50917a8f/RTX_3090_5x.v7_0_0.O-w4.18_Aug_2025.hcb).
- **Отличие от имеющихся данных:** новые Hashcat v7.0.0 и 5-карточная конфигурация; имеющиеся RTX 3090 raw-записи относятся к v6.x и другим rig sizes.

| Mode | Алгоритм | GPU #01 | 5× суммарно `Speed.#*` |
|---:|---|---:|---:|
| 0 | MD5 | 63,727.9 MH/s | 328.1 GH/s |
| 100 | SHA1 | 22,810.8 MH/s | 117.2 GH/s |
| 1400 | SHA2-256 | 8,701.1 MH/s | 44,404.3 MH/s |
| 1700 | SHA2-512 | 2,947.4 MH/s | 15,065.0 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 1,066.5 kH/s | 5,443.0 kH/s |
| 1000 | NTLM | 105.4 GH/s | 536.1 GH/s |
| 3200 | bcrypt | 110.1 kH/s | 553.7 kH/s |
