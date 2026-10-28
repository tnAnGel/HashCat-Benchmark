# 🏆 Видеокарты — сводная таблица бенчмарков

Собранные Hashcat-бенчмарки и связанные comparison-записи по видеокартам.
Каждое устройство — отдельная папка в [`GPU/`](GPU); внутри раздельно помечены
raw-вывод, partial-фрагменты, PTS-результаты и summary-only таблицы.

- **293 папки видеокарт/графических устройств с документами результатов**; в них раздельно хранятся raw, partial, PTS и comparison-only карточки
- Для PTS-данных без исходного stdout есть отдельные `.md` внутри папки устройства; они помечены как индивидуальные обработанные результаты или профильный агрегат и не считаются raw.
- Реестры покрытия: [`COVERAGE.md`](COVERAGE.md) (десктоп/DC),
  [`MOBILE.md`](MOBILE.md) и [`MOBILE-ROSTER.md`](MOBILE-ROSTER.md) (мобильные)

```
GPU/
├── NVIDIA GeForce RTX 4090/
│   ├── NVIDIA GeForce RTX 4090 — Chick3nman v6.2.6.md
│   └── ...
├── AMD Radeon RX 7900 XTX/
└── ...
```

---

## 🏆 Сводная таблица (скорость на одну карту)

Значения — **на одну видеокарту** (`Speed.#1`), режим оптимизированного ядра (`-O`).
Отсортировано по MD5. Единицы: H/s → kH/s → MH/s → GH/s → TH/s.

Основные хеш-режимы: **MD5** (0), **NTLM** (1000), **SHA2-256** (1400),
**SHA2-512** (1700), **WPA2** (22000, PBKDF2-PMKID/EAPOL), **bcrypt** (3200).

| # | GPU | MD5 | NTLM | SHA2-256 | SHA2-512 | WPA2 | bcrypt |
|--:|-----|----:|-----:|---------:|---------:|-----:|-------:|
| 1 | [NVIDIA GeForce RTX 5090](<GPU/NVIDIA GeForce RTX 5090>) | 221 GH/s | 340 GH/s | 28.4 GH/s | 10.0 GH/s | 3.4 MH/s | 305 kH/s |
| 2 | [NVIDIA GeForce RTX 4090](<GPU/NVIDIA GeForce RTX 4090>) | 164 GH/s | 288 GH/s | 22.0 GH/s | 7.5 GH/s | 2.5 MH/s | 184 kH/s |
| 3 | [AMD Instinct MI300X](<GPU/AMD Instinct MI300X>) ⚠️partial, unofficial build | 163.7 GH/s | 272.3 GH/s | 25.2 GH/s | 8.59 GH/s | 3.02 MH/s | 131 kH/s |
| 4 | [NVIDIA L40S](<GPU/NVIDIA L40S>) | 148 GH/s | 259 GH/s | 20.1 GH/s | 6.7 GH/s | 2.3 MH/s | 177 kH/s |
| 5 | [NVIDIA B200](<GPU/NVIDIA B200>) | 140 GH/s | 248 GH/s | 16.4 GH/s | 5.7 GH/s | 2.4 MH/s | 420 kH/s |
| 6 | [NVIDIA RTX 6000 Ada Generation](<GPU/NVIDIA RTX 6000 Ada Generation>) | 132 GH/s | 216 GH/s | 19.2 GH/s | 6.4 GH/s | 2.3 MH/s | 201 kH/s |
| 7 | [NVIDIA L40](<GPU/NVIDIA L40>) | 121 GH/s | 206 GH/s | 18.7 GH/s | 6.2 GH/s | 2.2 MH/s | 177 kH/s |
| 8 | [NVIDIA H200](<GPU/NVIDIA H200>) | 120 GH/s | 204 GH/s | 16.4 GH/s | 5.4 GH/s | 2.2 MH/s | 352 kH/s |
| 9 | [NVIDIA GH200](<GPU/NVIDIA GH200>) ⚠️`-w 4` | 120 GH/s | 203 GH/s | 16.4 GH/s | 5.4 GH/s | 2.2 MH/s | 371 kH/s |
| 10 | [NVIDIA H100 SXM5](<GPU/NVIDIA H100 SXM5>) | 117 GH/s | 197 GH/s | 16.2 GH/s | 5.4 GH/s | 1.9 MH/s | 346 kH/s |
| 11 | [NVIDIA GeForce RTX 5080](<GPU/NVIDIA GeForce RTX 5080>) | 105 GH/s | 164 GH/s | 13.6 GH/s | 4.9 GH/s | 1.6 MH/s | 124 kH/s |
| 12 | [NVIDIA GeForce RTX 4080 SUPER](<GPU/NVIDIA GeForce RTX 4080 SUPER>) | 99.6 GH/s | 176 GH/s | 13.3 GH/s | 4.6 GH/s | 1.6 MH/s | 146 kH/s |
| 13 | [NVIDIA GeForce RTX 4080](<GPU/NVIDIA GeForce RTX 4080>) | 98.3 GH/s | 173 GH/s | 13.1 GH/s | 4.5 GH/s | 1.5 MH/s | 131 kH/s |
| 14 | [NVIDIA GeForce RTX 5070 Ti](<GPU/NVIDIA GeForce RTX 5070 Ti>) | 88.2 GH/s | 138 GH/s | 11.4 GH/s | 4.1 GH/s | 1.4 MH/s | 108 kH/s |
| 15 | [NVIDIA H100 PCIe](<GPU/NVIDIA H100 PCIe>) | 87.5 GH/s | 159 GH/s | 12.2 GH/s | 4.1 GH/s | 1.5 MH/s | 252 kH/s |
| 16 | [NVIDIA GeForce RTX 4070 Ti SUPER](<GPU/NVIDIA GeForce RTX 4070 Ti SUPER>) | 85.0 GH/s | 149 GH/s | 11.3 GH/s | 3.8 GH/s | 1.3 MH/s | 124 kH/s |
| 17 | [NVIDIA GeForce RTX 3090 Ti](<GPU/NVIDIA GeForce RTX 3090 Ti>) | 79.1 GH/s | 143 GH/s | 10.8 GH/s | 3.6 GH/s | 1.3 MH/s | 91.0 kH/s |
| 18 | [AMD Radeon RX 7900 XTX](<GPU/AMD Radeon RX 7900 XTX>) | 74.2 GH/s | 114 GH/s | 12.6 GH/s | 2.5 GH/s | 1.5 MH/s | 99.4 kH/s |
| 19 | [NVIDIA GeForce RTX 3090](<GPU/NVIDIA GeForce RTX 3090>) | 71.7 GH/s | 124 GH/s | 9.6 GH/s | 3.2 GH/s | 1.1 MH/s | 108 kH/s |
| 20 | [NVIDIA GeForce RTX 4070 SUPER](<GPU/NVIDIA GeForce RTX 4070 SUPER>) | 69.9 GH/s | 123 GH/s | 9.3 GH/s | 3.2 GH/s | 1.1 MH/s | 103 kH/s |
| 21 | [NVIDIA GeForce RTX 3080 Ti](<GPU/NVIDIA GeForce RTX 3080 Ti>) | 69.2 GH/s | 120 GH/s | 9.3 GH/s | 3.1 GH/s | 1.1 MH/s | 105 kH/s |
| 22 | [NVIDIA RTX A6000](<GPU/NVIDIA RTX A6000>) | 68.2 GH/s | 122 GH/s | 9.8 GH/s | 2.9 GH/s | 1.1 MH/s | 90.6 kH/s |
| 23 | [NVIDIA A800 80GB PCIe](<GPU/NVIDIA A800 80GB PCIe>) | 68.1 GH/s | 116 GH/s | 9.5 GH/s | 3.2 GH/s | 1.1 MH/s | 138 kH/s |
| 23a | [NVIDIA A100 SXM4 40GB](<GPU/NVIDIA A100 SXM4 40GB>) ⚠️OnlineHashCrack v6.2.3 | 68.6 GH/s | — | — | — | — | — |
| 24 | [NVIDIA GeForce RTX 4070 Ti](<GPU/NVIDIA GeForce RTX 4070 Ti>) | 67.8 GH/s | 115 GH/s | 9.1 GH/s | 3.0 GH/s | 917 kH/s | 109 kH/s |
| 25 | [NVIDIA A100 80GB](<GPU/NVIDIA A100 80GB>) | 67.4 GH/s | 114 GH/s | 9.5 GH/s | 3.2 GH/s | 1.1 MH/s | 165 kH/s |
| 26 | [NVIDIA A40](<GPU/NVIDIA A40>) ⚠️8× rig source; #1 | 65.3 GH/s | 110.7 GH/s | 9.14 GH/s | 2.69 GH/s | 1.08 MH/s | 71.7 kH/s |
| 27 | [NVIDIA A100 PCIe 40GB](<GPU/NVIDIA A100 PCIe 40GB>) | 64.9 GH/s | 120 GH/s | 9.4 GH/s | 3.1 GH/s | 1.1 MH/s | 138 kH/s |
| 28 | [NVIDIA TITAN RTX](<GPU/NVIDIA TITAN RTX>) | 64.0 GH/s | 112 GH/s | 8.7 GH/s | 2.8 GH/s | — | 39.6 kH/s |
| 29 | [AMD Radeon RX 7900 XT](<GPU/AMD Radeon RX 7900 XT>) | 61.7 GH/s | 97.8 GH/s | 10.6 GH/s | 2.1 GH/s | 1.2 MH/s | 83.4 kH/s |
| 30 | [AMD Radeon RX 6950 XT](<GPU/AMD Radeon RX 6950 XT>) | 61.6 GH/s | 100.0 GH/s | 10.4 GH/s | 2.8 GH/s | 1.2 MH/s | 61.1 kH/s |
| 31 | [NVIDIA GeForce RTX 5070](<GPU/NVIDIA GeForce RTX 5070>) | 60.7 GH/s | 92.3 GH/s | 7.8 GH/s | 2.3 GH/s | 961 kH/s | 85.7 kH/s |
| 32 | [NVIDIA GeForce RTX 4070](<GPU/NVIDIA GeForce RTX 4070>) | 58.8 GH/s | 101 GH/s | 7.9 GH/s | 2.7 GH/s | 928 kH/s | 86.3 kH/s |
| 33 | [AMD Radeon RX 6900 XT](<GPU/AMD Radeon RX 6900 XT>) | 56.4 GH/s | 91.0 GH/s | 9.4 GH/s | 2.5 GH/s | 1.1 MH/s | 72.8 kH/s |
| 34 | [NVIDIA Tesla V100 SXM2 16GB](<GPU/NVIDIA Tesla V100 SXM2 16GB>) | 55.7 GH/s | 99.8 GH/s | 7.6 GH/s | 2.4 GH/s | 884 kH/s | 78.7 kH/s |
| 35 | [NVIDIA Quadro RTX 6000](<GPU/NVIDIA Quadro RTX 6000>) | 54.6 GH/s | 96.6 GH/s | 8.1 GH/s | 2.6 GH/s | — | 29.1 kH/s |
| 36 | [NVIDIA GeForce RTX 2080 Ti](<GPU/NVIDIA GeForce RTX 2080 Ti>) | 53.4 GH/s | 94.7 GH/s | 7.3 GH/s | 2.4 GH/s | 853 kH/s | 63.3 kH/s |
| 37 | [AMD Radeon RX 9070 XT](<GPU/AMD Radeon RX 9070 XT>) | 52.6 GH/s | 92.4 GH/s | 9.3 GH/s | 2.1 GH/s | 1.1 MH/s | 68.8 kH/s |
| 38 | [AMD Radeon RX 6800 XT](<GPU/AMD Radeon RX 6800 XT>) | 52.4 GH/s | 85.4 GH/s | 8.7 GH/s | 2.3 GH/s | 1.1 MH/s | 58.2 kH/s |
| 39 | [NVIDIA GeForce RTX 3080](<GPU/NVIDIA GeForce RTX 3080>) | 51.0 GH/s | 90.1 GH/s | 6.9 GH/s | 2.3 GH/s | 809 kH/s | 74.7 kH/s |
| 40 | [NVIDIA Tesla V100 PCIe](<GPU/NVIDIA Tesla V100 PCIe>) | 50.0 GH/s | 83.4 GH/s | 6.8 GH/s | 2.2 GH/s | — | 48.9 kH/s |
| 41 | [NVIDIA RTX A5000](<GPU/NVIDIA RTX A5000>) | 48.8 GH/s | 82.2 GH/s | 6.9 GH/s | 2.3 GH/s | 816 kH/s | 85.6 kH/s |
| 42 | [NVIDIA GeForce RTX 5060 Ti](<GPU/NVIDIA GeForce RTX 5060 Ti>) | 47.0 GH/s | 72.2 GH/s | 6.0 GH/s | 1.7 GH/s | 738 kH/s | 66.3 kH/s |
| 43 | [NVIDIA A10](<GPU/NVIDIA A10G>) | 45.8 GH/s | 76.1 GH/s | 6.5 GH/s | 2.1 GH/s | 745 kH/s | 77.0 kH/s |
| 44 | [NVIDIA TITAN V](<GPU/NVIDIA TITAN V>) | 45.5 GH/s | 67.5 GH/s | 6.5 GH/s | 1.9 GH/s | — | 47.2 kH/s |
| 45 | [NVIDIA GeForce RTX 3070 Ti](<GPU/NVIDIA GeForce RTX 3070 Ti>) | 44.4 GH/s | 82.1 GH/s | 6.1 GH/s | 2.0 GH/s | 716 kH/s | 68.5 kH/s |
| 46 | [NVIDIA CMP 170HX](<GPU/NVIDIA CMP 170HX>) | 43.4 GH/s | 73.6 GH/s | 6.1 GH/s | 2.1 GH/s | 719 kH/s | 92.1 kH/s |
| 47 | [NVIDIA GeForce RTX 4060 Ti](<GPU/NVIDIA GeForce RTX 4060 Ti>) | 43.0 GH/s | 76.1 GH/s | 5.7 GH/s | 2.0 GH/s | 675 kH/s | 62.3 kH/s |
| 48 | [NVIDIA CMP 50HX](<GPU/NVIDIA CMP 50HX>) | 42.7 GH/s | 71.4 GH/s | 6.1 GH/s | 2.0 GH/s | 706 kH/s | 45.9 kH/s |
| 49 | [AMD Radeon RX 6800](<GPU/AMD Radeon RX 6800>) | 42.2 GH/s | 75.8 GH/s | 7.0 GH/s | 1.6 GH/s | 833 kH/s | 42.6 kH/s |
| 50 | [NVIDIA CMP 90HX](<GPU/NVIDIA CMP 90HX>) | 41.5 GH/s | 70.0 GH/s | 5.9 GH/s | 2.0 GH/s | 688 kH/s | 62.4 kH/s |
| 51 | [NVIDIA TITAN Xp](<GPU/NVIDIA TITAN Xp>) | 40.4 GH/s | 71.3 GH/s | 4.9 GH/s | 1.6 GH/s | — | 35.1 kH/s |
| 52 | [NVIDIA GeForce RTX 2080 SUPER](<GPU/NVIDIA GeForce RTX 2080 SUPER>) | 40.1 GH/s | 70.0 GH/s | 5.7 GH/s | 1.8 GH/s | — | 27.5 kH/s |
| 53 | [NVIDIA L4](<GPU/NVIDIA L4>) | 39.8 GH/s | 68.1 GH/s | 5.4 GH/s | 1.8 GH/s | 622 kH/s | 59.8 kH/s |
| 54 | [NVIDIA CMP 100-200](<GPU/NVIDIA CMP 100-200>) | 37.2 GH/s | 58.1 GH/s | 5.7 GH/s | 1.8 GH/s | 668 kH/s | 52.0 kH/s |
| 55 | [NVIDIA GeForce RTX 2080](<GPU/NVIDIA GeForce RTX 2080>) | 37.1 GH/s | 53.0 GH/s | 5.4 GH/s | 1.8 GH/s | — | 18.5 kH/s |
| 56 | [NVIDIA GeForce RTX 3070](<GPU/NVIDIA GeForce RTX 3070>) | 35.5 GH/s | 61.4 GH/s | 4.8 GH/s | 1.6 GH/s | 558 kH/s | 60.3 kH/s |
| 57 | [NVIDIA GeForce GTX 1080 Ti](<GPU/NVIDIA GeForce GTX 1080 Ti>) | 35.2 GH/s | 58.3 GH/s | 4.4 GH/s | 1.4 GH/s | — | 21.4 kH/s |
| 58 | [NVIDIA GeForce RTX 3060 Ti](<GPU/NVIDIA GeForce RTX 3060 Ti>) | 34.8 GH/s | 62.0 GH/s | 4.7 GH/s | 1.6 GH/s | 562 kH/s | 51.6 kH/s |
| 59 | [NVIDIA GeForce RTX 2070 SUPER](<GPU/NVIDIA GeForce RTX 2070 SUPER>) | 34.8 GH/s | 58.3 GH/s | 4.3 GH/s | 1.4 GH/s | 493 kH/s | 30.0 kH/s |
| 60 | [NVIDIA RTX A4000](<GPU/NVIDIA RTX A4000>) | 33.3 GH/s | 43.3 GH/s | 2.9 GH/s | 1.3 GH/s | 470 kH/s | 53.7 kH/s |
| 61 | [AMD Radeon VII](<GPU/AMD Radeon VII>) | 33.1 GH/s | 54.9 GH/s | 4.9 GH/s | 1.5 GH/s | — | 24.1 kH/s |
| 62 | [NVIDIA Tesla P40](<GPU/NVIDIA Tesla P40>) ⚠️2019 partial | 32.9 GH/s | 56.1 GH/s | 3.96 GH/s | 1.28 GH/s | — | 18.8 kH/s |
| 63 | [AMD Radeon RX 6700 XT](<GPU/AMD Radeon RX 6700 XT>) | 32.1 GH/s | 51.8 GH/s | 5.4 GH/s | 1.4 GH/s | 647 kH/s | 29.6 kH/s |
| 64 | [NVIDIA GeForce RTX 3070 Laptop GPU](<GPU/NVIDIA GeForce RTX 3070 Laptop GPU>) | 31.9 GH/s | 58.7 GH/s | 4.4 GH/s | 1.5 GH/s | 520 kH/s | 53.9 kH/s |
| 65 | [AMD Radeon RX 6800M](<GPU/AMD Radeon RX 6800M>) | 31.7 GH/s | 50.9 GH/s | 5.2 GH/s | 1.4 GH/s | 617 kH/s | 28.5 kH/s |
| 66 | [AMD Radeon RX Vega 64](<GPU/AMD Radeon RX Vega 64>) | 31.6 GH/s | 51.7 GH/s | 4.6 GH/s | 1.2 GH/s | 522 kH/s | 20.7 kH/s |
| 67 | [NVIDIA GeForce RTX 3080 Laptop GPU](<GPU/NVIDIA GeForce RTX 3080 Laptop GPU>) | 30.3 GH/s | 53.5 GH/s | 4.3 GH/s | 1.4 GH/s | 478 kH/s | 57.6 kH/s |
| 68 | [NVIDIA GeForce RTX 2060 SUPER](<GPU/NVIDIA GeForce RTX 2060 SUPER>) | 29.1 GH/s | 51.0 GH/s | 3.9 GH/s | 1.3 GH/s | 450 kH/s | 30.9 kH/s |
| 69 | [AMD Radeon RX Vega 64 Liquid Cooling](<GPU/AMD Radeon RX Vega 64 Liquid Cooling>) ⚠️неполный | 29.0 GH/s | 54.8 GH/s | 5.0 GH/s | 1.1 GH/s | — | — |
| 70 | [NVIDIA GeForce RTX 4060](<GPU/NVIDIA GeForce RTX 4060>) | 28.6 GH/s | 48.8 GH/s | 4.0 GH/s | 1.2 GH/s | 461 kH/s | 38.7 kH/s |
| 71 | [AMD Radeon RX 6650 XT](<GPU/AMD Radeon RX 6650 XT>) | 28.0 GH/s | 45.1 GH/s | 4.7 GH/s | 1.3 GH/s | 548 kH/s | 31.7 kH/s |
| 72 | [NVIDIA GeForce RTX 2060](<GPU/NVIDIA GeForce RTX 2060>) | 27.1 GH/s | 47.6 GH/s | 3.6 GH/s | 1.2 GH/s | 418 kH/s | 28.3 kH/s |
| 73 | [NVIDIA GeForce RTX 2070](<GPU/NVIDIA GeForce RTX 2070>) | 26.9 GH/s | 40.0 GH/s | 4.0 GH/s | 1.3 GH/s | — | 14.3 kH/s |
| 74 | [NVIDIA P102-100](<GPU/NVIDIA P102-100>) | 26.5 GH/s | 43.3 GH/s | 3.9 GH/s | 1.3 GH/s | 549 kH/s | 27.2 kH/s |
| 75 | [Apple M2 Ultra](<GPU/Apple M2 Ultra>) | 26.5 GH/s | 44.5 GH/s | 4.1 GH/s | 1.0 GH/s | 482 kH/s | 15.3 kH/s |
| 76 | [AMD Radeon RX 6600 XT](<GPU/AMD Radeon RX 6600 XT>) | 25.6 GH/s | 40.6 GH/s | 4.2 GH/s | 1.1 GH/s | 496 kH/s | 29.9 kH/s |
| 77 | [NVIDIA GeForce RTX 3060](<GPU/NVIDIA GeForce RTX 3060>) | 25.2 GH/s | 44.2 GH/s | 3.4 GH/s | 1.1 GH/s | 395 kH/s | 36.7 kH/s |
| 78 | [NVIDIA Quadro RTX 4000](<GPU/NVIDIA Quadro RTX 4000>) | 25.1 GH/s | 45.9 GH/s | 3.7 GH/s | 1.2 GH/s | 426 kH/s | 28.0 kH/s |
| 79 | [NVIDIA GeForce RTX 3060 Laptop GPU](<GPU/NVIDIA GeForce RTX 3060 Laptop GPU>) | 25.0 GH/s | 47.8 GH/s | 3.4 GH/s | 1.2 GH/s | 417 kH/s | 35.5 kH/s |
| 80 | [Intel Arc B580](<GPU/Intel Arc B580>) | 24.7 GH/s | 33.3 GH/s | 1.3 GH/s | 318 MH/s | 580 kH/s | 15.4 kH/s |
| 81 | [NVIDIA GeForce GTX 1080](<GPU/NVIDIA GeForce GTX 1080>) | 24.7 GH/s | 43.0 GH/s | 3.1 GH/s | 1.0 GH/s | 440 kH/s | 21.6 kH/s |
| 82 | [NVIDIA GeForce GTX 1070 Ti](<GPU/NVIDIA GeForce GTX 1070 Ti>) | 24.3 GH/s | 41.3 GH/s | 3.0 GH/s | 986 MH/s | 424 kH/s | 21.0 kH/s |
| 83 | [Intel Arc A770M](<GPU/Intel Arc A770M>) | 24.1 GH/s | 40.4 GH/s | 114 MH/s | 806 MH/s | 212 kH/s | — |
| 84 | [AMD Radeon RX 5700 XT](<GPU/AMD Radeon RX 5700 XT>) | 23.8 GH/s | 38.1 GH/s | 4.1 GH/s | 1.1 GH/s | — | 18.2 kH/s |
| 85 | [Apple M4 Max](<GPU/Apple M4 Max>) | 22.1 GH/s | 37.7 GH/s | 3.6 GH/s | 708 MH/s | 486 kH/s | 21.3 kH/s |
| 86 | [NVIDIA Tesla P100](<GPU/NVIDIA Tesla P100>) | 22.0 GH/s | — | — | — | — | — |
| 87 | [NVIDIA Tesla T4](<GPU/NVIDIA Tesla T4>) | 21.2 GH/s | 32.3 GH/s | 3.2 GH/s | 1.0 GH/s | — | 13.4 kH/s |
| 88 | [NVIDIA GeForce RTX 2060 Mobile](<GPU/NVIDIA GeForce RTX 2060 Mobile>) | 20.9 GH/s | 41.1 GH/s | 3.2 GH/s | 1.0 GH/s | 365 kH/s | 5.7 kH/s |
| 89 | [NVIDIA CMP 70HX](<GPU/NVIDIA CMP 70HX>) | 20.8 GH/s | 35.1 GH/s | 2.9 GH/s | 852 MH/s | 340 kH/s | 29.5 kH/s |
| 90 | [AMD Radeon RX 5600 XT](<GPU/AMD Radeon RX 5600 XT>) | 20.6 GH/s | 31.6 GH/s | 3.5 GH/s | 879 MH/s | 413 kH/s | 19.2 kH/s |
| 91 | [AMD Radeon RX 6600](<GPU/AMD Radeon RX 6600>) | 20.6 GH/s | 33.6 GH/s | 3.5 GH/s | 946 MH/s | 417 kH/s | 26.0 kH/s |
| 92 | [NVIDIA GeForce GTX 1070](<GPU/NVIDIA GeForce GTX 1070>) | 19.6 GH/s | 33.8 GH/s | 2.5 GH/s | 809 MH/s | 350 kH/s | 16.7 kH/s |
| 93 | [NVIDIA GeForce GTX 1660 SUPER](<GPU/NVIDIA GeForce GTX 1660 SUPER>) | 19.6 GH/s | 34.9 GH/s | 2.6 GH/s | 878 MH/s | 305 kH/s | 20.1 kH/s |
| 94 | [Apple M3 Max](<GPU/Apple M3 Max>) | 19.1 GH/s | 32.6 GH/s | 3.0 GH/s | 594 MH/s | 408 kH/s | 32.6 kH/s |
| 95 | [NVIDIA GeForce GTX 1660](<GPU/NVIDIA GeForce GTX 1660>) | 19.0 GH/s | 32.6 GH/s | 2.4 GH/s | 795 MH/s | 288 kH/s | 19.4 kH/s |
| 96 | [NVIDIA GeForce GTX 980 Ti](<GPU/NVIDIA GeForce GTX 980 Ti>) | 18.9 GH/s | 31.7 GH/s | 2.3 GH/s | 793 MH/s | — | 10.9 kH/s |
| 97 | [NVIDIA Quadro RTX 5000](<GPU/NVIDIA Quadro RTX 5000>) | 18.5 GH/s | 23.0 GH/s | 4.2 GH/s | 1.6 GH/s | 662 kH/s | 38.7 kH/s |
| 98 | [NVIDIA RTX A2000](<GPU/NVIDIA RTX A2000>) | 17.3 GH/s | 28.6 GH/s | 2.4 GH/s | 818 MH/s | 289 kH/s | 31.3 kH/s |
| 99 | [NVIDIA Tesla M40](<GPU/NVIDIA Tesla M40>) | 17.1 GH/s | 29.5 GH/s | 2.1 GH/s | 695 MH/s | 296 kH/s | 10.1 kH/s |
| 100 | [Apple M1 Ultra](<GPU/Apple M1 Ultra>) | 17.1 GH/s | 28.6 GH/s | 1.8 GH/s | 575 MH/s | 297 kH/s | 10.1 kH/s |
| 101 | [NVIDIA GeForce GTX TITAN X](<GPU/NVIDIA GeForce GTX TITAN X>) | 15.8 GH/s | 25.3 GH/s | 2.2 GH/s | 742 MH/s | 325 kH/s | 14.7 kH/s |
| 102 | [AMD Radeon RX 590](<GPU/AMD Radeon RX 590>) | 14.0 GH/s | 22.6 GH/s | 1.9 GH/s | 486 MH/s | 236 kH/s | 10.6 kH/s |
| 103 | [NVIDIA GeForce RTX 3050 6 GB](<GPU/NVIDIA GeForce RTX 3050 6 GB>) | 13.9 GH/s | 24.8 GH/s | 1.9 GH/s | 549 MH/s | 214 kH/s | 20.9 kH/s |
| 104 | [NVIDIA Quadro P4000](<GPU/NVIDIA Quadro P4000>) | 13.8 GH/s | 23.5 GH/s | 2.0 GH/s | 658 MH/s | 285 kH/s | 10.4 kH/s |
| 105 | [Apple M1 Max](<GPU/Apple M1 Max>) | 13.2 GH/s | 21.1 GH/s | 2.0 GH/s | 396 MH/s | 248 kH/s | 9.3 kH/s |
| 106 | [NVIDIA P104-100](<GPU/NVIDIA P104-100>) | 13.2 GH/s | 21.1 GH/s | 1.9 GH/s | 643 MH/s | 269 kH/s | 16.6 kH/s |
| 107 | [NVIDIA GeForce GTX 1060 6GB](<GPU/NVIDIA GeForce GTX 1060 6GB>) | 13.1 GH/s | 22.6 GH/s | 1.7 GH/s | 535 MH/s | 235 kH/s | 11.0 kH/s |
| 108 | [Apple M2 Max](<GPU/Apple M2 Max>) | 12.9 GH/s | 22.4 GH/s | 2.0 GH/s | 406 MH/s | 246 kH/s | 8.2 kH/s |
| 109 | [NVIDIA Quadro T2000](<GPU/NVIDIA Quadro T2000>) | 12.8 GH/s | 21.3 GH/s | 1.8 GH/s | 613 MH/s | 209 kH/s | 12.8 kH/s |
| 110 | [NVIDIA GeForce GTX 1650](<GPU/NVIDIA GeForce GTX 1650>) | 12.6 GH/s | 22.8 GH/s | 1.7 GH/s | 577 MH/s | 199 kH/s | 13.1 kH/s |
| 111 | [AMD Radeon RX 480](<GPU/AMD Radeon RX 480>) ⚠️неполный | 12.5 GH/s | 24.6 GH/s | 1.8 GH/s | 391 MH/s | — | 8.7 kH/s |
| 112 | [NVIDIA GeForce RTX 3050 Laptop GPU](<GPU/NVIDIA GeForce RTX 3050 Laptop GPU>) | 11.5 GH/s | 19.8 GH/s | 1.6 GH/s | 517 MH/s | 178 kH/s | 16.9 kH/s |
| 113 | [NVIDIA GeForce GTX 980](<GPU/NVIDIA GeForce GTX 980>) | 11.4 GH/s | 23.2 GH/s | 1.5 GH/s | 490 MH/s | 186 kH/s | 11.4 kH/s |
| 114 | [NVIDIA GeForce GTX 1060 3GB](<GPU/NVIDIA GeForce GTX 1060 3GB>) | 10.7 GH/s | 16.1 GH/s | 1.1 GH/s | 362 MH/s | 168 kH/s | 8.1 kH/s |
| 115 | [NVIDIA GeForce GTX 970](<GPU/NVIDIA GeForce GTX 970>) | 10.4 GH/s | 21.4 GH/s | 1.3 GH/s | 410 MH/s | — | 9.0 kH/s |
| 116 | [AMD Radeon Pro 5500M](<GPU/AMD Radeon Pro 5500M>) ⚠️ | 10.4 GH/s | 15.6 GH/s | 1.6 GH/s | 291 MH/s | — | 10.7 kH/s |
| 117 | [AMD Radeon R9 290](<GPU/AMD Radeon R9 290>) | 10.2 GH/s | 18.0 GH/s | 1.4 GH/s | 99.8 MH/s | — | 4.5 kH/s |
| 118 | [NVIDIA P106-100](<GPU/NVIDIA P106-100>) | 9.5 GH/s | 16.4 GH/s | 1.4 GH/s | 336 MH/s | — | 5.9 kH/s |
| 119 | [NVIDIA GeForce GTX 1060 with Max-Q Design](<GPU/NVIDIA GeForce GTX 1060 with Max-Q Design>) | 9.1 GH/s | 15.3 GH/s | 1.3 GH/s | 447 MH/s | — | 6.9 kH/s |
| 120 | [NVIDIA Jetson AGX Orin (Orin)](<GPU/NVIDIA Jetson AGX Orin (Orin)>) | 9.1 GH/s | 15.3 GH/s | 1.3 GH/s | 434 MH/s | 143 kH/s | 16.2 kH/s |
| 121 | [Apple M4 Pro](<GPU/Apple M4 Pro>) | 9.0 GH/s | 15.7 GH/s | 1.4 GH/s | 292 MH/s | 196 kH/s | 7.5 kH/s |
| 122 | [AMD Radeon RX 6400](<GPU/AMD Radeon RX 6400>) | 8.8 GH/s | 14.4 GH/s | 1.4 GH/s | 335 MH/s | 174 kH/s | 9.0 kH/s |
| 123 | [NVIDIA GeForce RTX 4050 Laptop GPU](<GPU/NVIDIA GeForce RTX 4050 Laptop GPU>) ⚠️`-w 1` | 8.3 GH/s | 7.3 GH/s | 1.5 GH/s | 807 MH/s | 341 kH/s | 18.4 kH/s |
| 124 | [Apple M2 Pro](<GPU/Apple M2 Pro>) | 7.0 GH/s | 12.0 GH/s | 1.0 GH/s | 648 MH/s | 126 kH/s | 4.4 kH/s |
| 125 | [AMD Radeon R9 M395X](<GPU/AMD Radeon R9 M395X>) ⚠️неполный | 6.9 GH/s | 11.1 GH/s | 980 MH/s | 149 MH/s | — | 3.5 kH/s |
| 126 | [Apple M3 Pro](<GPU/Apple M3 Pro>) | 6.8 GH/s | 11.7 GH/s | 1.1 GH/s | 220 MH/s | 146 kH/s | 6.0 kH/s |
| 127 | [NVIDIA T600](<GPU/NVIDIA T600>) ⚠️`-w 4` | 6.6 GH/s | 10.8 GH/s | 974 MH/s | 324 MH/s | 113 kH/s | 8.9 kH/s |
| 128 | [Intel Arc 140V](<GPU/Intel Arc 140V>) ⚠️self-test errors | 6.6 GH/s | 8.4 GH/s | 500 MH/s | 81.1 MH/s | 155 kH/s | 3.9 kH/s |
| 129 | [NVIDIA GeForce GTX 960](<GPU/NVIDIA GeForce GTX 960>) | 6.5 GH/s | 11.9 GH/s | 862 MH/s | 255 MH/s | — | 3.8 kH/s |
| 130 | [NVIDIA GeForce GTX 1650 Ti](<GPU/NVIDIA GeForce GTX 1650 Ti>) | 6.4 GH/s | 11.6 GH/s | 850 MH/s | 254 MH/s | 157 kH/s | 1.4 kH/s |
| 131 | [Apple M5](<GPU/Apple M5>) | 6.2 GH/s | 10.7 GH/s | 1.3 GH/s | 229 MH/s | 145 kH/s | 6.8 kH/s |
| 132 | [NVIDIA Tesla M60](<GPU/NVIDIA Tesla M60>) | 6.1 GH/s | 11.5 GH/s | 473 MH/s | 233 MH/s | 186 kH/s | 9.4 kH/s |
| 133 | [AMD Radeon RX 580](<GPU/AMD Radeon RX 580>) | 5.9 GH/s | 9.7 GH/s | 843 MH/s | 154 MH/s | 65.0 kH/s | 4.5 kH/s |
| 134 | [NVIDIA GeForce GTX 950](<GPU/NVIDIA GeForce GTX 950>) | 5.8 GH/s | 10.2 GH/s | 712 MH/s | 241 MH/s | 102 kH/s | 4.4 kH/s |
| 135 | [NVIDIA GeForce GTX 1050 Ti](<GPU/NVIDIA GeForce GTX 1050 Ti>) | 5.6 GH/s | 5.6 GH/s | 375 MH/s | 94.8 MH/s | 50.9 kH/s | 4.4 kH/s |
| 136 | [Apple M4](<GPU/Apple M4>) | 5.6 GH/s | 9.8 GH/s | 890 MH/s | 178 MH/s | 122 kH/s | 8.7 kH/s |
| 137 | [Apple M1 Pro](<GPU/Apple M1 Pro>) | 5.5 GH/s | 9.0 GH/s | 867 MH/s | 224 MH/s | 102 kH/s | 3.4 kH/s |
| 138 | [NVIDIA GeForce GTX 1050](<GPU/NVIDIA GeForce GTX 1050>) | 5.2 GH/s | 8.7 GH/s | 744 MH/s | 249 MH/s | — | 3.5 kH/s |
| 139 | [NVIDIA Quadro P1000](<GPU/NVIDIA Quadro P1000>) | 4.8 GH/s | 7.8 GH/s | 693 MH/s | 202 MH/s | 98.4 kH/s | 4.6 kH/s |
| 140 | [NVIDIA Jetson AGX Xavier (Xavier)](<GPU/NVIDIA Jetson AGX Xavier (Xavier)>) ⚠️неполный | 4.7 GH/s | 7.0 GH/s | 670 MH/s | 217 MH/s | — | — |
| 141 | [NVIDIA Tesla K80](<GPU/NVIDIA Tesla K80>) | 4.6 GH/s | 7.7 GH/s | 785 MH/s | 257 MH/s | — | 2.6 kH/s |
| 142 | [AMD Radeon RX 460](<GPU/AMD Radeon RX 460>) | 4.2 GH/s | 6.6 GH/s | 573 MH/s | 143 MH/s | 67.3 kH/s | 2.7 kH/s |
| 143 | [NVIDIA GeForce GTX 960M](<GPU/NVIDIA GeForce GTX 960M>) | 3.8 GH/s | 6.9 GH/s | 462 MH/s | 158 MH/s | — | 1.3 kH/s |
| 144 | [Valve Steam Deck (AMD Custom GPU 0932)](<GPU/Valve Steam Deck (AMD Custom GPU 0932)>) | 3.5 GH/s | 5.7 GH/s | 601 MH/s | 122 MH/s | 72.0 kH/s | 3.8 kH/s |
| 145 | [Apple M3](<GPU/Apple M3>) | 3.3 GH/s | — | 536 MH/s | — | — | — |
| 146 | [AMD Radeon Pro WX 3200](<GPU/AMD Radeon Pro WX 3200>) | 3.2 GH/s | 5.7 GH/s | 494 MH/s | 124 MH/s | — | 2.3 kH/s |
| 147 | [NVIDIA GeForce GTX 860M](<GPU/NVIDIA GeForce GTX 860M>) | 3.1 GH/s | 6.0 GH/s | 397 MH/s | 139 MH/s | — | 899 H/s |
| 148 | [NVIDIA Quadro P2000 Mobile](<GPU/NVIDIA Quadro P2000 Mobile>) | 2.9 GH/s | 3.7 GH/s | 621 MH/s | 241 MH/s | 120 kH/s | 5.5 kH/s |
| 149 | [NVIDIA GeForce GT 1030](<GPU/NVIDIA GeForce GT 1030>) | 2.9 GH/s | 5.7 GH/s | 370 MH/s | 111 MH/s | 54.6 kH/s | 2.4 kH/s |
| 150 | [NVIDIA Jetson Xavier NX (Xavier)](<GPU/NVIDIA Jetson Xavier NX (Xavier)>) | 2.8 GH/s | 5.1 GH/s | 415 MH/s | 134 MH/s | 48.1 kH/s | 4.3 kH/s |
| 151 | [Apple M1](<GPU/Apple M1>) | 2.8 GH/s | 4.8 GH/s | 300 MH/s | 97.6 MH/s | 48.9 kH/s | 2.1 kH/s |
| 152 | [Apple M2](<GPU/Apple M2>) | 2.3 GH/s | 2.7 GH/s | 339 MH/s | 120 MH/s | 67.4 kH/s | 2.9 kH/s |
| 153 | [NVIDIA GeForce 940M](<GPU/NVIDIA GeForce 940M>) ⚠️неполный | 2.1 GH/s | 3.8 GH/s | 271 MH/s | 92.3 MH/s | — | 709 H/s |
| 154 | [NVIDIA RTX A2000 Laptop GPU](<GPU/NVIDIA RTX A2000 Laptop GPU>) | 2.1 GH/s | 2.4 GH/s | 228 MH/s | 79.3 MH/s | 19.0 kH/s | 1.7 kH/s |
| 155 | [NVIDIA GeForce 940MX](<GPU/NVIDIA GeForce 940MX>) ⚠️неполный | 1.7 GH/s | — | — | — | — | — |
| 156 | [NVIDIA Quadro M1200](<GPU/NVIDIA Quadro M1200>) ⚠️`-w 4` | 1.4 GH/s | 1.8 GH/s | 339 MH/s | 128 MH/s | 63.6 kH/s | 1.6 kH/s |
| 157 | [NVIDIA GeForce GT 730](<GPU/NVIDIA GeForce GT 730>) | 895 MH/s | 1.4 GH/s | 112 MH/s | 26.6 MH/s | 12.3 kH/s | 156 H/s |
| 158 | [NVIDIA Jetson Nano (Tegra X1)](<GPU/NVIDIA Jetson Nano (Tegra X1)>) | 554 MH/s | 959 MH/s | 68.8 MH/s | 24.4 MH/s | — | 258 H/s |
| 159 | [NVIDIA GeForce GT 720](<GPU/NVIDIA GeForce GT 720>) | 401 MH/s | 645 MH/s | 51.2 MH/s | 14.0 MH/s | 6.0 kH/s | 69 H/s |
| 160 | [AMD Radeon (Pro) Vega 56](<GPU/AMD Radeon (Pro) Vega 56>) | — | — | — | — | — | — |
| 161 | [AMD Radeon 760M Graphics](<GPU/AMD Radeon 760M Graphics>) ⚠️полный `-w 3`, без `-O` | — | — | — | — | — | — |
| 162 | [Intel Arc A770](<GPU/Intel Arc A770>) ⚠️только m22000 | — | — | — | — | 538 kH/s | — |
| 163 | [NVIDIA GeForce GTX 1660 Ti](<GPU/NVIDIA GeForce GTX 1660 Ti>) ⚠️только m3200 | — | — | — | — | — | 12.8 kH/s |

### Новые частичные и legacy-записи (не ранжируются)

| GPU | MD5 | NTLM | SHA2-256 | SHA2-512 | WPA2 | bcrypt |
|-----|----:|-----:|---------:|---------:|-----:|-------:|
| [NVIDIA GeForce RTX 2070 Super Max-Q](<GPU/NVIDIA GeForce RTX 2070 Super Max-Q>) ⚠️3 режима | 25.0 GH/s | — | 3.46 GH/s | — | — | — |
| [AMD Radeon R9 390X](<GPU/AMD Radeon R9 390X>) ⚠️legacy selected modes | 12.0 GH/s | 22.2 GH/s | 1.64 GH/s | 646 MH/s | 204 kH/s | 8.13 kH/s |
| [AMD Radeon RX 580 2048SP](<GPU/AMD Radeon RX 580 2048SP>) — отдельный SKU | 10.1 GH/s | 19.6 GH/s | 1.56 GH/s | 430 MH/s | 177 kH/s | 6.28 kH/s |
| [NVIDIA Tesla P4](<GPU/NVIDIA Tesla P4>) ⚠️published table, CUDA v6.2.6 | 15.2 GH/s | 26.2 GH/s | 1.9 GH/s | 647.1 MH/s | 268.1 kH/s | 12.2 kH/s |
| [AMD Radeon 780M Graphics](<GPU/AMD Radeon 780M Graphics>) ⚠️6 режимов | 7.37 GH/s | 13.3 GH/s | 1.26 GH/s | 293 MH/s | 143 kH/s | — |
| [NVIDIA GRID K520](<GPU/NVIDIA GRID K520>) ⚠️legacy partial | 2.50 GH/s | 4.00 GH/s | 296 MH/s | 71.3 MH/s | 42.8 kH/s | 501 H/s |
| [NVIDIA GeForce GTX 760](<GPU/NVIDIA GeForce GTX 760>) ⚠️legacy, no MD5 | — | — | — | — | 47.7 kH/s | — |
| [Intel UHD Graphics 630](<GPU/Intel UHD Graphics 630>) ⚠️6 modes | — | 651 MH/s | 47.9 MH/s | 8.64 kH/s | 5.77 kH/s | 515 H/s |
| [NVIDIA GB10](<GPU/NVIDIA GB10>) ⚠️частичный фрагмент | 53.5 GH/s | 80.0 GH/s | 6.71 GH/s | 2.45 GH/s | 842 kH/s | 74.8 kH/s |
| [Intel HD Graphics 4600](<GPU/Intel HD Graphics 4600>) ⚠️3 режима | 220 MH/s | 368.3 MH/s | — | — | — | — |
| [Intel UHD Graphics 620](<GPU/Intel UHD Graphics 620>) ⚠️1 режим | 531.1 MH/s | — | — | — | — | — |
| [NVIDIA GeForce GTX 770](<GPU/NVIDIA GeForce GTX 770>) ⚠️3×legacy, per-device | 3.70 GH/s | — | 555.8 MH/s | 110.8 MH/s | — | — |
| [NVIDIA GeForce GTX 780 Ti](<GPU/NVIDIA GeForce GTX 780 Ti>) ⚠️NTLM only | — | 12.89 GH/s | — | — | — | — |
| [AMD Radeon Pro 580X](<GPU/AMD Radeon Pro 580X>) ⚠️3 modes | 10.29 GH/s | — | 1.38 GH/s | — | — | — |
| [AMD Radeon RX Vega 10 Graphics](<GPU/AMD Radeon RX Vega 10 Graphics>) ⚠️4 modes | 3.60 GH/s | — | 560.2 MH/s | 128.1 MH/s | — | — |
| [AMD Radeon RX Vega 11 Graphics](<GPU/AMD Radeon RX Vega 11 Graphics>) ⚠️WPA only | — | — | — | — | 57.6 kH/s | — |
| [AMD Radeon (TM) 520](<GPU/AMD Radeon (TM) 520>) ⚠️4 modes | 525.6 MH/s | — | 72.3 MH/s | 20.7 MH/s | — | — |
| [AMD Radeon HD 8250 (Kalindi)](<GPU/AMD Radeon HD 8250 (Kalindi)>) ⚠️4 modes | 212.5 MH/s | — | 31.4 MH/s | 6.2 MH/s | — | — |
| [AMD Radeon RX 570 Series](<GPU/AMD Radeon RX 570 Series>) ⚠️SHA1 only; 3-device series alias | — | — | — | — | — | — |
| [Apple M5 Max](<GPU/Apple M5 Max>) ⚠️WPA only; proprietary Hashcat-ng fork | — | — | — | — | 413.5 kH/s | — |
| [AMD Radeon 8060S](<GPU/AMD Radeon 8060S>) ⚠️MD5 only | 24.51 GH/s | — | — | — | — | — |
| [Intel HD Graphics 4000](<GPU/Intel HD Graphics 4000>) ⚠️NTLM only | — | 334.9 MH/s | — | — | — | — |
| [Intel HD Graphics 4400](<GPU/Intel HD Graphics 4400>) ⚠️WPA only | — | — | — | — | 2.50 kH/s | — |
| [Intel Iris Pro](<GPU/Intel Iris Pro>) ⚠️2 modes | 339.7 MH/s | — | — | — | — | — |
| [AMD Radeon R9 M370X](<GPU/AMD Radeon R9 M370X>) ⚠️3 legacy modes | 1.18 GH/s | — | — | — | — | — |
| [AMD Radeon Pro Vega II](<GPU/AMD Radeon Pro Vega II>) ⚠️partial 4× | 28.4 GH/s | — | — | — | — | — |
| [AMD Radeon Pro W6800X Duo](<GPU/AMD Radeon Pro W6800X Duo>) ⚠️partial per-device range | 26.9–38.9 GH/s | — | 6.26–6.70 GH/s | — | — | — |
| [AMD Radeon Pro W5700X](<GPU/AMD Radeon Pro W5700X>) ⚠️4 modes | 20.65 GH/s | — | 3.48 GH/s | 574 MH/s | — | — |
| [AMD Radeon HD FirePro D700](<GPU/AMD Radeon HD FirePro D700>) ⚠️oclHashcat v2.01 partial, per-device | 4.38 GH/s | 5.18 GH/s | 838 MH/s | 251 MH/s | — | 470 kH/s |
| [NVIDIA GeForce GTX 750](<GPU/NVIDIA GeForce GTX 750>) ⚠️cudaHashcat v1.21 legacy | 2.62 GH/s | 4.58 GH/s | 339 MH/s | 75.6 MH/s | — | 1.83 kH/s |
| [NVIDIA GeForce GTX 765M](<GPU/NVIDIA GeForce GTX 765M>) ⚠️cudaHashcat-lite v0.15, timed partial | 1.43 GH/s | — | — | — | — | — |
| [NVIDIA GeForce GTX 780M](<GPU/NVIDIA GeForce GTX 780M>) ⚠️legacy forum output, version unspecified | 2.00 GH/s | 2.97 GH/s | 205 MH/s | 85.9 MH/s | — | 576 H/s |
| [NVIDIA GeForce GTX 660M](<GPU/NVIDIA GeForce GTX 660M>) ⚠️oclHashcat v2.01 partial; CPU skipped | 1.55 GH/s | — | 1.54 GH/s | 1.55 GH/s | — | — |
| [NVIDIA RTX PRO 6000 Blackwell Workstation Edition](<GPU/NVIDIA RTX PRO 6000 Blackwell Workstation Edition>) ⚠️v7.1.2, 2× raw partial, OpenCL fallback; per-device #01 | 251 GH/s | — | 32.8 GH/s | 10.7 GH/s | — | — |

**Новые источники в этом проходе:** GTX 750 (legacy benchmark-mode публикация), GTX 660M, GTX 765M, GT 650M, GTX 780M (частичные/старые публикации), RTX PRO 6000 Blackwell Workstation Edition (2×, v7.1.2; per-device и суммарные скорости); дополнительный двухкарточный Mac Pro v2.01 прогон FirePro D700.

**Только нестандартный legacy-режим:** [NVIDIA GeForce GT 650M](<GPU/NVIDIA GeForce GT 650M>) — опубликована строка WPA/WPA2 5227 H/s; остальные видимые строки того же вывода отброшены из-за явно неправдоподобных скоростей/аварийного завершения. Не считать результатом современного mode 22000.

**Отдельная частичная карточка без стандартных режимов:** [NVIDIA Quadro P5000](<GPU/NVIDIA Quadro P5000>) — PKZIP modes 17220/17225.

> ⚠️ Цифры взяты из разных прогонов (разные драйверы, ОС, версии hashcat, разгон),
> поэтому это **ориентир**, а не строгое сравнение. Точные условия — в каждом
> отдельном документе. Прочерк «—» означает, что режим пропущен/не тестировался
> в исходном прогоне либо файл в старом формате oclHashcat без номеров режимов.
> Пометка ⚠️`-w 1` — прогон сделан с `--workload-profile=1`, карта сильно
> недогружена, сравнивать с остальными строками напрямую нельзя.

---

## Полный указатель папок устройств

В каталоге 293 GPU-папки с карточками результатов. Сводные PHCS/PTS и сторонние опубликованные таблицы не являются raw.

<!-- FULL_GPU_INDEX_START -->
| GPU-папка | Документов | Тип свидетельств |
|---|---:|---|
| [AMD FirePro D300](<GPU/AMD FirePro D300>) | 1 | source/partial |
| [AMD Instinct MI250X-MI250](<GPU/AMD Instinct MI250X-MI250>) | 1 | source/partial |
| [AMD Instinct MI300X](<GPU/AMD Instinct MI300X>) | 2 | source/partial, published rates (non-raw) |
| [AMD Instinct MI50](<GPU/AMD Instinct MI50>) | 1 | source/partial |
| [AMD Radeon (Pro) Vega 56](<GPU/AMD Radeon (Pro) Vega 56>) | 1 | source/partial |
| [AMD Radeon (TM) 520](<GPU/AMD Radeon (TM) 520>) | 1 | source/partial |
| [AMD Radeon 32GB (PTS alias)](<GPU/AMD Radeon 32GB (PTS alias)>) | 1 | PTS |
| [AMD Radeon 680M](<GPU/AMD Radeon 680M>) | 1 | source/partial |
| [AMD Radeon 760M Graphics](<GPU/AMD Radeon 760M Graphics>) | 2 | source/partial |
| [AMD Radeon 780M Graphics](<GPU/AMD Radeon 780M Graphics>) | 1 | source/partial |
| [AMD Radeon 8060S](<GPU/AMD Radeon 8060S>) | 3 | PTS, source/partial |
| [AMD Radeon 890M](<GPU/AMD Radeon 890M>) | 1 | PTS |
| [AMD Radeon AI PRO R9700](<GPU/AMD Radeon AI PRO R9700>) | 3 | PTS, source/partial |
| [AMD Radeon HD 6990](<GPU/AMD Radeon HD 6990>) | 1 | source/partial |
| [AMD Radeon HD 7970](<GPU/AMD Radeon HD 7970>) | 1 | source/partial |
| [AMD Radeon HD 8250 (Kalindi)](<GPU/AMD Radeon HD 8250 (Kalindi)>) | 1 | source/partial |
| [AMD Radeon HD FirePro D700](<GPU/AMD Radeon HD FirePro D700>) | 2 | source/partial |
| [AMD Radeon Pro 5500M](<GPU/AMD Radeon Pro 5500M>) | 3 | source/partial |
| [AMD Radeon Pro 560](<GPU/AMD Radeon Pro 560>) | 1 | source/partial |
| [AMD Radeon Pro 580X](<GPU/AMD Radeon Pro 580X>) | 1 | source/partial |
| [AMD Radeon Pro Vega II](<GPU/AMD Radeon Pro Vega II>) | 1 | source/partial |
| [AMD Radeon Pro W5700X](<GPU/AMD Radeon Pro W5700X>) | 1 | source/partial |
| [AMD Radeon Pro W6800X Duo](<GPU/AMD Radeon Pro W6800X Duo>) | 1 | source/partial |
| [AMD Radeon PRO W7500](<GPU/AMD Radeon PRO W7500>) | 1 | PTS |
| [AMD Radeon PRO W7600](<GPU/AMD Radeon PRO W7600>) | 2 | PTS |
| [AMD Radeon PRO W7700](<GPU/AMD Radeon PRO W7700>) | 2 | PTS |
| [AMD Radeon PRO W7900](<GPU/AMD Radeon PRO W7900>) | 2 | PTS |
| [AMD Radeon Pro WX 3200](<GPU/AMD Radeon Pro WX 3200>) | 1 | source/partial |
| [AMD Radeon R9 270X](<GPU/AMD Radeon R9 270X>) | 1 | source/partial |
| [AMD Radeon R9 280X](<GPU/AMD Radeon R9 280X>) | 1 | source/partial |
| [AMD Radeon R9 290](<GPU/AMD Radeon R9 290>) | 2 | PHCS summary, source/partial |
| [AMD Radeon R9 290X](<GPU/AMD Radeon R9 290X>) | 1 | source/partial |
| [AMD Radeon R9 390X](<GPU/AMD Radeon R9 390X>) | 1 | source/partial |
| [AMD Radeon R9 M370X](<GPU/AMD Radeon R9 M370X>) | 1 | source/partial |
| [AMD Radeon R9 M395X](<GPU/AMD Radeon R9 M395X>) | 1 | source/partial |
| [AMD Radeon RX 460](<GPU/AMD Radeon RX 460>) | 1 | source/partial |
| [AMD Radeon RX 470-590 (PTS combined alias)](<GPU/AMD Radeon RX 470-590 (PTS combined alias)>) | 2 | PHCS summary, PTS |
| [AMD Radeon RX 480](<GPU/AMD Radeon RX 480>) | 1 | source/partial |
| [AMD Radeon RX 5500 XT](<GPU/AMD Radeon RX 5500 XT>) | 1 | source/partial |
| [AMD Radeon RX 560 XT](<GPU/AMD Radeon RX 560 XT>) | 1 | PHCS summary |
| [AMD Radeon RX 5600 XT](<GPU/AMD Radeon RX 5600 XT>) | 2 | PHCS summary, source/partial |
| [AMD Radeon RX 570 Series](<GPU/AMD Radeon RX 570 Series>) | 1 | source/partial |
| [AMD Radeon RX 5700](<GPU/AMD Radeon RX 5700>) | 1 | PTS |
| [AMD Radeon RX 5700 XT](<GPU/AMD Radeon RX 5700 XT>) | 2 | PHCS summary, source/partial |
| [AMD Radeon RX 580](<GPU/AMD Radeon RX 580>) | 2 | PTS, source/partial |
| [AMD Radeon RX 580 2048SP](<GPU/AMD Radeon RX 580 2048SP>) | 3 | PHCS summary, raw/source/partial |
| [AMD Radeon RX 590](<GPU/AMD Radeon RX 590>) | 2 | PHCS summary, source/partial |
| [AMD Radeon RX 6400](<GPU/AMD Radeon RX 6400>) | 1 | source/partial |
| [AMD Radeon RX 6600](<GPU/AMD Radeon RX 6600>) | 2 | PHCS summary, source/partial |
| [AMD Radeon RX 6600 XT](<GPU/AMD Radeon RX 6600 XT>) | 2 | PHCS summary, source/partial |
| [AMD Radeon RX 6650 XT](<GPU/AMD Radeon RX 6650 XT>) | 2 | PHCS summary, source/partial |
| [AMD Radeon RX 6700 XT](<GPU/AMD Radeon RX 6700 XT>) | 2 | PHCS summary, source/partial |
| [AMD Radeon RX 6800](<GPU/AMD Radeon RX 6800>) | 3 | PHCS summary, PTS, source/partial |
| [AMD Radeon RX 6800 XT](<GPU/AMD Radeon RX 6800 XT>) | 3 | PHCS summary, PTS, source/partial |
| [AMD Radeon RX 6800M](<GPU/AMD Radeon RX 6800M>) | 1 | source/partial |
| [AMD Radeon RX 6900 XT](<GPU/AMD Radeon RX 6900 XT>) | 3 | PHCS summary, PTS, source/partial |
| [AMD Radeon RX 6950 XT](<GPU/AMD Radeon RX 6950 XT>) | 2 | PHCS summary, source/partial |
| [AMD Radeon RX 7600](<GPU/AMD Radeon RX 7600>) | 1 | PTS |
| [AMD Radeon RX 7600 XT](<GPU/AMD Radeon RX 7600 XT>) | 1 | PTS |
| [AMD Radeon RX 7700 XT](<GPU/AMD Radeon RX 7700 XT>) | 1 | PTS |
| [AMD Radeon RX 7800 XT](<GPU/AMD Radeon RX 7800 XT>) | 2 | PHCS summary, PTS |
| [AMD Radeon RX 7900 GRE](<GPU/AMD Radeon RX 7900 GRE>) | 1 | PTS |
| [AMD Radeon RX 7900 XT](<GPU/AMD Radeon RX 7900 XT>) | 3 | PHCS summary, PTS, source/partial |
| [AMD Radeon RX 7900 XTX](<GPU/AMD Radeon RX 7900 XTX>) | 4 | PHCS summary, PTS, source/partial |
| [AMD Radeon RX 9060 XT](<GPU/AMD Radeon RX 9060 XT>) | 1 | PTS |
| [AMD Radeon RX 9070](<GPU/AMD Radeon RX 9070>) | 1 | PTS |
| [AMD Radeon RX 9070 GRE](<GPU/AMD Radeon RX 9070 GRE>) | 1 | PTS |
| [AMD Radeon RX 9070 XT](<GPU/AMD Radeon RX 9070 XT>) | 3 | PHCS summary, PTS, source/partial |
| [AMD Radeon RX Vega 10 Graphics](<GPU/AMD Radeon RX Vega 10 Graphics>) | 1 | source/partial |
| [AMD Radeon RX Vega 11 Graphics](<GPU/AMD Radeon RX Vega 11 Graphics>) | 1 | source/partial |
| [AMD Radeon RX Vega 64](<GPU/AMD Radeon RX Vega 64>) | 1 | source/partial |
| [AMD Radeon RX Vega 64 Liquid Cooling](<GPU/AMD Radeon RX Vega 64 Liquid Cooling>) | 1 | source/partial |
| [AMD Radeon Vega 8](<GPU/AMD Radeon Vega 8>) | 1 | PTS |
| [AMD Radeon VII](<GPU/AMD Radeon VII>) | 1 | source/partial |
| [Apple M1](<GPU/Apple M1>) | 1 | source/partial |
| [Apple M1 Max](<GPU/Apple M1 Max>) | 1 | source/partial |
| [Apple M1 Pro](<GPU/Apple M1 Pro>) | 1 | source/partial |
| [Apple M1 Ultra](<GPU/Apple M1 Ultra>) | 1 | source/partial |
| [Apple M2](<GPU/Apple M2>) | 1 | source/partial |
| [Apple M2 Max](<GPU/Apple M2 Max>) | 1 | source/partial |
| [Apple M2 Pro](<GPU/Apple M2 Pro>) | 1 | source/partial |
| [Apple M2 Ultra](<GPU/Apple M2 Ultra>) | 1 | source/partial |
| [Apple M3](<GPU/Apple M3>) | 1 | source/partial |
| [Apple M3 Max](<GPU/Apple M3 Max>) | 1 | source/partial |
| [Apple M3 Pro](<GPU/Apple M3 Pro>) | 1 | source/partial |
| [Apple M4](<GPU/Apple M4>) | 1 | source/partial |
| [Apple M4 Max](<GPU/Apple M4 Max>) | 1 | source/partial |
| [Apple M4 Pro](<GPU/Apple M4 Pro>) | 1 | source/partial |
| [Apple M5](<GPU/Apple M5>) | 1 | source/partial |
| [Apple M5 Max](<GPU/Apple M5 Max>) | 1 | source/partial |
| [Intel 2GB (PTS alias)](<GPU/Intel 2GB (PTS alias)>) | 1 | PTS |
| [Intel Arc 140V](<GPU/Intel Arc 140V>) | 2 | PTS, source/partial |
| [Intel Arc A310](<GPU/Intel Arc A310>) | 1 | Hashcat-ng summary only (non-upstream) |
| [Intel Arc A380](<GPU/Intel Arc A380>) | 2 | PTS, Hashcat-ng summary only (non-upstream) |
| [Intel Arc A580](<GPU/Intel Arc A580>) | 1 | PTS |
| [Intel Arc A750](<GPU/Intel Arc A750>) | 1 | PTS |
| [Intel Arc A770](<GPU/Intel Arc A770>) | 5 | PTS, raw, source/partial |
| [Intel Arc A770M](<GPU/Intel Arc A770M>) | 2 | raw, source/partial |
| [Intel Arc B570](<GPU/Intel Arc B570>) | 1 | PTS |
| [Intel Arc B580](<GPU/Intel Arc B580>) | 4 | PHCS summary, PTS, source/partial |
| [Intel Arc Graphics (Meteor Lake iGPU)](<GPU/Intel Arc Graphics (Meteor Lake iGPU)>) | 1 | PTS |
| [Intel Arc Pro B50](<GPU/Intel Arc Pro B50>) | 2 | PTS |
| [Intel Arc Pro B70](<GPU/Intel Arc Pro B70>) | 2 | PTS, source/partial |
| [Intel BMG-G21 (PTS chip alias)](<GPU/Intel BMG-G21 (PTS chip alias)>) | 1 | PTS |
| [Intel BMG-G31](<GPU/Intel BMG-G31>) | 1 | PTS |
| [Intel BMG-G31 (PTS chip alias)](<GPU/Intel BMG-G31 (PTS chip alias)>) | 1 | PTS |
| [Intel HD Graphics 4000](<GPU/Intel HD Graphics 4000>) | 1 | source/partial |
| [Intel HD Graphics 4400](<GPU/Intel HD Graphics 4400>) | 1 | source/partial |
| [Intel HD Graphics 4600](<GPU/Intel HD Graphics 4600>) | 3 | PTS, source/partial |
| [Intel HD Graphics 630](<GPU/Intel HD Graphics 630>) | 1 | source/partial |
| [Intel Iris Pro](<GPU/Intel Iris Pro>) | 1 | source/partial |
| [Intel Iris Xe Graphics (Alder Lake GT2)](<GPU/Intel Iris Xe Graphics (Alder Lake GT2)>) | 2 | PTS |
| [Intel Iris Xe Graphics (Raptor Lake-P)](<GPU/Intel Iris Xe Graphics (Raptor Lake-P)>) | 1 | raw/partial |
| [Intel Iris Xe Graphics (Tiger Lake-LP GT2)](<GPU/Intel Iris Xe Graphics (Tiger Lake-LP GT2)>) | 2 | PTS, source/partial |
| [Intel Panther Lake Graphics (PTS alias)](<GPU/Intel Panther Lake Graphics (PTS alias)>) | 1 | PTS |
| [Intel UHD Graphics 620](<GPU/Intel UHD Graphics 620>) | 1 | source/partial |
| [Intel UHD Graphics 630](<GPU/Intel UHD Graphics 630>) | 1 | source/partial |
| [Intel UHD Graphics 770](<GPU/Intel UHD Graphics 770>) | 2 | PTS, source/partial |
| [NVIDIA A100 80GB](<GPU/NVIDIA A100 80GB>) | 1 | source/partial |
| [NVIDIA A100 PCIe 40GB](<GPU/NVIDIA A100 PCIe 40GB>) | 2 | source/partial |
| [NVIDIA A100 SXM4 40GB](<GPU/NVIDIA A100 SXM4 40GB>) | 2 | PHCS summary, source/partial |
| [NVIDIA A10G](<GPU/NVIDIA A10G>) | 3 | PHCS summary, source/partial |
| [NVIDIA A40](<GPU/NVIDIA A40>) | 1 | source/partial |
| [NVIDIA A800 80GB PCIe](<GPU/NVIDIA A800 80GB PCIe>) | 1 | source/partial |
| [NVIDIA B200](<GPU/NVIDIA B200>) | 2 | PHCS summary, source/partial |
| [NVIDIA CMP 100-200](<GPU/NVIDIA CMP 100-200>) | 2 | PHCS summary, source/partial |
| [NVIDIA CMP 170HX](<GPU/NVIDIA CMP 170HX>) | 2 | PHCS summary, source/partial |
| [NVIDIA CMP 50HX](<GPU/NVIDIA CMP 50HX>) | 3 | PHCS summary, source/partial |
| [NVIDIA CMP 70HX](<GPU/NVIDIA CMP 70HX>) | 2 | PHCS summary, source/partial |
| [NVIDIA CMP 90HX](<GPU/NVIDIA CMP 90HX>) | 3 | PHCS summary, source/partial |
| [NVIDIA GB10](<GPU/NVIDIA GB10>) | 1 | source/partial |
| [NVIDIA GeForce 940M](<GPU/NVIDIA GeForce 940M>) | 1 | source/partial |
| [NVIDIA GeForce 940MX](<GPU/NVIDIA GeForce 940MX>) | 1 | source/partial |
| [NVIDIA GeForce GT 1030](<GPU/NVIDIA GeForce GT 1030>) | 1 | source/partial |
| [NVIDIA GeForce GT 650M](<GPU/NVIDIA GeForce GT 650M>) | 1 | source/partial |
| [NVIDIA GeForce GT 720](<GPU/NVIDIA GeForce GT 720>) | 1 | source/partial |
| [NVIDIA GeForce GT 730](<GPU/NVIDIA GeForce GT 730>) | 1 | source/partial |
| [NVIDIA GeForce GTX 1050](<GPU/NVIDIA GeForce GTX 1050>) | 1 | source/partial |
| [NVIDIA GeForce GTX 1050 3GB Laptop](<GPU/NVIDIA GeForce GTX 1050 3GB Laptop>) | 1 | source/partial |
| [NVIDIA GeForce GTX 1050 Ti](<GPU/NVIDIA GeForce GTX 1050 Ti>) | 2 | PHCS summary, source/partial |
| [NVIDIA GeForce GTX 1050 Ti (Laptop)](<GPU/NVIDIA GeForce GTX 1050 Ti (Laptop)>) | 1 | source/partial |
| [NVIDIA GeForce GTX 1060](<GPU/NVIDIA GeForce GTX 1060>) | 2 | PHCS summary, PTS |
| [NVIDIA GeForce GTX 1060 (Laptop)](<GPU/NVIDIA GeForce GTX 1060 (Laptop)>) | 1 | source/partial |
| [NVIDIA GeForce GTX 1060 3GB](<GPU/NVIDIA GeForce GTX 1060 3GB>) | 1 | source/partial |
| [NVIDIA GeForce GTX 1060 6GB](<GPU/NVIDIA GeForce GTX 1060 6GB>) | 1 | source/partial |
| [NVIDIA GeForce GTX 1060 with Max-Q Design](<GPU/NVIDIA GeForce GTX 1060 with Max-Q Design>) | 1 | source/partial |
| [NVIDIA GeForce GTX 1070](<GPU/NVIDIA GeForce GTX 1070>) | 4 | PHCS summary, source/partial |
| [NVIDIA GeForce GTX 1070 (Laptop)](<GPU/NVIDIA GeForce GTX 1070 (Laptop)>) | 1 | source/partial |
| [NVIDIA GeForce GTX 1070 Ti](<GPU/NVIDIA GeForce GTX 1070 Ti>) | 3 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce GTX 1070 with Max-Q Design](<GPU/NVIDIA GeForce GTX 1070 with Max-Q Design>) | 1 | source/partial |
| [NVIDIA GeForce GTX 1080](<GPU/NVIDIA GeForce GTX 1080>) | 6 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce GTX 1080 (Laptop)](<GPU/NVIDIA GeForce GTX 1080 (Laptop)>) | 1 | source/partial |
| [NVIDIA GeForce GTX 1080 Ti](<GPU/NVIDIA GeForce GTX 1080 Ti>) | 9 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce GTX 1080 with Max-Q Design](<GPU/NVIDIA GeForce GTX 1080 with Max-Q Design>) | 1 | source/partial |
| [NVIDIA GeForce GTX 1650](<GPU/NVIDIA GeForce GTX 1650>) | 3 | PHCS summary, source/partial |
| [NVIDIA GeForce GTX 1650 Ti](<GPU/NVIDIA GeForce GTX 1650 Ti>) | 2 | PHCS summary, source/partial |
| [NVIDIA GeForce GTX 1650 Ti + AMD Radeon](<GPU/NVIDIA GeForce GTX 1650 Ti + AMD Radeon>) | 1 | PTS |
| [NVIDIA GeForce GTX 1660](<GPU/NVIDIA GeForce GTX 1660>) | 2 | PHCS summary, source/partial |
| [NVIDIA GeForce GTX 1660 SUPER](<GPU/NVIDIA GeForce GTX 1660 SUPER>) | 4 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce GTX 1660 Ti](<GPU/NVIDIA GeForce GTX 1660 Ti>) | 2 | PTS, source/partial |
| [NVIDIA GeForce GTX 660](<GPU/NVIDIA GeForce GTX 660>) | 1 | source/partial |
| [NVIDIA GeForce GTX 660 Ti](<GPU/NVIDIA GeForce GTX 660 Ti>) | 1 | source/partial |
| [NVIDIA GeForce GTX 660M](<GPU/NVIDIA GeForce GTX 660M>) | 1 | source/partial |
| [NVIDIA GeForce GTX 690](<GPU/NVIDIA GeForce GTX 690>) | 1 | source/partial |
| [NVIDIA GeForce GTX 750](<GPU/NVIDIA GeForce GTX 750>) | 1 | source/partial |
| [NVIDIA GeForce GTX 750 Ti](<GPU/NVIDIA GeForce GTX 750 Ti>) | 2 | PHCS summary, source/partial |
| [NVIDIA GeForce GTX 760](<GPU/NVIDIA GeForce GTX 760>) | 1 | source/partial |
| [NVIDIA GeForce GTX 765M](<GPU/NVIDIA GeForce GTX 765M>) | 1 | source/partial |
| [NVIDIA GeForce GTX 770](<GPU/NVIDIA GeForce GTX 770>) | 2 | source/partial |
| [NVIDIA GeForce GTX 780 Ti](<GPU/NVIDIA GeForce GTX 780 Ti>) | 1 | source/partial |
| [NVIDIA GeForce GTX 780M](<GPU/NVIDIA GeForce GTX 780M>) | 1 | source/partial |
| [NVIDIA GeForce GTX 860M](<GPU/NVIDIA GeForce GTX 860M>) | 1 | source/partial |
| [NVIDIA GeForce GTX 950](<GPU/NVIDIA GeForce GTX 950>) | 2 | PTS, source/partial |
| [NVIDIA GeForce GTX 950M](<GPU/NVIDIA GeForce GTX 950M>) | 1 | source/partial |
| [NVIDIA GeForce GTX 960](<GPU/NVIDIA GeForce GTX 960>) | 2 | PTS, source/partial |
| [NVIDIA GeForce GTX 960M](<GPU/NVIDIA GeForce GTX 960M>) | 1 | source/partial |
| [NVIDIA GeForce GTX 965M](<GPU/NVIDIA GeForce GTX 965M>) | 1 | source/partial |
| [NVIDIA GeForce GTX 970](<GPU/NVIDIA GeForce GTX 970>) | 2 | PHCS summary, source/partial |
| [NVIDIA GeForce GTX 970M](<GPU/NVIDIA GeForce GTX 970M>) | 1 | source/partial |
| [NVIDIA GeForce GTX 980](<GPU/NVIDIA GeForce GTX 980>) | 1 | source/partial |
| [NVIDIA GeForce GTX 980 Ti](<GPU/NVIDIA GeForce GTX 980 Ti>) | 2 | source/partial |
| [NVIDIA GeForce GTX 980M](<GPU/NVIDIA GeForce GTX 980M>) | 1 | source/partial |
| [NVIDIA GeForce GTX TITAN X](<GPU/NVIDIA GeForce GTX TITAN X>) | 2 | source/partial |
| [NVIDIA GeForce MX230](<GPU/NVIDIA GeForce MX230>) | 1 | PTS |
| [NVIDIA GeForce RTX 2060](<GPU/NVIDIA GeForce RTX 2060>) | 6 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 2060 Mobile](<GPU/NVIDIA GeForce RTX 2060 Mobile>) | 1 | source/partial |
| [NVIDIA GeForce RTX 2060 SUPER](<GPU/NVIDIA GeForce RTX 2060 SUPER>) | 3 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 2070](<GPU/NVIDIA GeForce RTX 2070>) | 3 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 2070 SUPER](<GPU/NVIDIA GeForce RTX 2070 SUPER>) | 4 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 2070 Super Max-Q](<GPU/NVIDIA GeForce RTX 2070 Super Max-Q>) | 2 | PHCS summary, source/partial |
| [NVIDIA GeForce RTX 2080](<GPU/NVIDIA GeForce RTX 2080>) | 5 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 2080 SUPER](<GPU/NVIDIA GeForce RTX 2080 SUPER>) | 4 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 2080 Ti](<GPU/NVIDIA GeForce RTX 2080 Ti>) | 6 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 2080 Ti + Intel UHD 630 + NVIDIA GeForce RTX 2080 Ti](<GPU/NVIDIA GeForce RTX 2080 Ti + Intel UHD 630 + NVIDIA GeForce RTX 2080 Ti>) | 1 | PTS |
| [NVIDIA GeForce RTX 3050 6 GB](<GPU/NVIDIA GeForce RTX 3050 6 GB>) | 2 | PHCS summary, source/partial |
| [NVIDIA GeForce RTX 3050 Laptop GPU](<GPU/NVIDIA GeForce RTX 3050 Laptop GPU>) | 1 | source/partial |
| [NVIDIA GeForce RTX 3050 Ti Laptop GPU](<GPU/NVIDIA GeForce RTX 3050 Ti Laptop GPU>) | 1 | PHCS summary |
| [NVIDIA GeForce RTX 3060](<GPU/NVIDIA GeForce RTX 3060>) | 4 | PHCS summary, PTS, raw/source |
| [NVIDIA GeForce RTX 3060 Laptop GPU](<GPU/NVIDIA GeForce RTX 3060 Laptop GPU>) | 3 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 3060 Ti](<GPU/NVIDIA GeForce RTX 3060 Ti>) | 3 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 3070](<GPU/NVIDIA GeForce RTX 3070>) | 5 | PHCS summary, PTS, raw/source |
| [NVIDIA GeForce RTX 3070 Laptop GPU](<GPU/NVIDIA GeForce RTX 3070 Laptop GPU>) | 1 | source/partial |
| [NVIDIA GeForce RTX 3070 Ti](<GPU/NVIDIA GeForce RTX 3070 Ti>) | 4 | PHCS summary, PTS, raw/source |
| [NVIDIA GeForce RTX 3080](<GPU/NVIDIA GeForce RTX 3080>) | 7 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 3080 Laptop GPU](<GPU/NVIDIA GeForce RTX 3080 Laptop GPU>) | 1 | source/partial |
| [NVIDIA GeForce RTX 3080 Ti](<GPU/NVIDIA GeForce RTX 3080 Ti>) | 5 | PHCS summary, PTS, raw/source |
| [NVIDIA GeForce RTX 3090](<GPU/NVIDIA GeForce RTX 3090>) | 9 | PHCS summary, PTS, raw/source |
| [NVIDIA GeForce RTX 3090 Ti](<GPU/NVIDIA GeForce RTX 3090 Ti>) | 4 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 4050 Laptop GPU](<GPU/NVIDIA GeForce RTX 4050 Laptop GPU>) | 2 | PHCS summary, source/partial |
| [NVIDIA GeForce RTX 4060](<GPU/NVIDIA GeForce RTX 4060>) | 3 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 4060 Laptop GPU](<GPU/NVIDIA GeForce RTX 4060 Laptop GPU>) | 2 | PHCS summary, source/partial |
| [NVIDIA GeForce RTX 4060 Ti](<GPU/NVIDIA GeForce RTX 4060 Ti>) | 2 | PHCS summary, source/partial |
| [NVIDIA GeForce RTX 4070](<GPU/NVIDIA GeForce RTX 4070>) | 4 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 4070 Laptop GPU](<GPU/NVIDIA GeForce RTX 4070 Laptop GPU>) | 1 | PTS |
| [NVIDIA GeForce RTX 4070 SUPER](<GPU/NVIDIA GeForce RTX 4070 SUPER>) | 3 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 4070 Ti](<GPU/NVIDIA GeForce RTX 4070 Ti>) | 3 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 4070 Ti SUPER](<GPU/NVIDIA GeForce RTX 4070 Ti SUPER>) | 4 | PHCS summary, PTS, raw/source |
| [NVIDIA GeForce RTX 4080](<GPU/NVIDIA GeForce RTX 4080>) | 3 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 4080 SUPER](<GPU/NVIDIA GeForce RTX 4080 SUPER>) | 4 | PHCS summary, PTS, raw/source |
| [NVIDIA GeForce RTX 4090](<GPU/NVIDIA GeForce RTX 4090>) | 8 | PHCS summary, PTS, raw/source |
| [NVIDIA GeForce RTX 4090 D](<GPU/NVIDIA GeForce RTX 4090 D>) | 1 | source/partial |
| [NVIDIA GeForce RTX 5060 Ti](<GPU/NVIDIA GeForce RTX 5060 Ti>) | 3 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 5070](<GPU/NVIDIA GeForce RTX 5070>) | 2 | PHCS summary, source/partial |
| [NVIDIA GeForce RTX 5070 Ti](<GPU/NVIDIA GeForce RTX 5070 Ti>) | 2 | PHCS summary, source/partial |
| [NVIDIA GeForce RTX 5080](<GPU/NVIDIA GeForce RTX 5080>) | 4 | PHCS summary, PTS, source/partial |
| [NVIDIA GeForce RTX 5090](<GPU/NVIDIA GeForce RTX 5090>) | 5 | PHCS summary, PTS, raw/source |
| [NVIDIA GeForce RTX 5090 Laptop GPU + Intel](<GPU/NVIDIA GeForce RTX 5090 Laptop GPU + Intel>) | 1 | PTS |
| [NVIDIA GeForce RTX 5090 Laptop GPU + Intel (hybrid PTS system)](<GPU/NVIDIA GeForce RTX 5090 Laptop GPU + Intel (hybrid PTS system)>) | 1 | PTS |
| [NVIDIA GeForce TITAN RTX](<GPU/NVIDIA GeForce TITAN RTX>) | 1 | PHCS summary |
| [NVIDIA GeForce TITAN V](<GPU/NVIDIA GeForce TITAN V>) | 1 | PHCS summary |
| [NVIDIA GeForce TITAN X](<GPU/NVIDIA GeForce TITAN X>) | 1 | PHCS summary |
| [NVIDIA GH200](<GPU/NVIDIA GH200>) | 3 | PTS, source/partial |
| [NVIDIA GRID K520](<GPU/NVIDIA GRID K520>) | 1 | source/partial |
| [NVIDIA H100 80GB HBM3](<GPU/NVIDIA H100 80GB HBM3>) | 1 | PHCS summary |
| [NVIDIA H100 PCIe](<GPU/NVIDIA H100 PCIe>) | 2 | source/partial |
| [NVIDIA H100 SXM5](<GPU/NVIDIA H100 SXM5>) | 2 | source/partial |
| [NVIDIA H200](<GPU/NVIDIA H200>) | 1 | source/partial |
| [NVIDIA Jetson AGX Orin (Orin)](<GPU/NVIDIA Jetson AGX Orin (Orin)>) | 1 | source/partial |
| [NVIDIA Jetson AGX Xavier (Xavier)](<GPU/NVIDIA Jetson AGX Xavier (Xavier)>) | 1 | source/partial |
| [NVIDIA Jetson Nano (Tegra X1)](<GPU/NVIDIA Jetson Nano (Tegra X1)>) | 2 | source/raw |
| [NVIDIA Jetson Xavier NX (Xavier)](<GPU/NVIDIA Jetson Xavier NX (Xavier)>) | 1 | source/partial |
| [NVIDIA L4](<GPU/NVIDIA L4>) | 1 | source/partial |
| [NVIDIA L40](<GPU/NVIDIA L40>) | 1 | source/partial |
| [NVIDIA L40S](<GPU/NVIDIA L40S>) | 2 | PHCS summary, source/partial |
| [NVIDIA P102-100](<GPU/NVIDIA P102-100>) | 1 | source/partial |
| [NVIDIA P104-100](<GPU/NVIDIA P104-100>) | 3 | PHCS summary, source/partial |
| [NVIDIA P106-100](<GPU/NVIDIA P106-100>) | 2 | PHCS summary, source/partial |
| [NVIDIA Quadro M1200](<GPU/NVIDIA Quadro M1200>) | 2 | PTS, source/partial |
| [NVIDIA Quadro P1000](<GPU/NVIDIA Quadro P1000>) | 1 | source/partial |
| [NVIDIA Quadro P2000](<GPU/NVIDIA Quadro P2000>) | 1 | PTS |
| [NVIDIA Quadro P2000 Mobile](<GPU/NVIDIA Quadro P2000 Mobile>) | 1 | source/partial |
| [NVIDIA Quadro P4000](<GPU/NVIDIA Quadro P4000>) | 1 | source/partial |
| [NVIDIA Quadro P5000](<GPU/NVIDIA Quadro P5000>) | 1 | source/partial |
| [NVIDIA Quadro RTX 4000](<GPU/NVIDIA Quadro RTX 4000>) | 3 | PTS, source/partial |
| [NVIDIA Quadro RTX 5000](<GPU/NVIDIA Quadro RTX 5000>) | 1 | source/partial |
| [NVIDIA Quadro RTX 5000 with Max-Q Design](<GPU/NVIDIA Quadro RTX 5000 with Max-Q Design>) | 1 | PTS |
| [NVIDIA Quadro RTX 6000](<GPU/NVIDIA Quadro RTX 6000>) | 1 | source/partial |
| [NVIDIA Quadro T2000](<GPU/NVIDIA Quadro T2000>) | 1 | source/partial |
| [NVIDIA RTX 2000 Ada Generation](<GPU/NVIDIA RTX 2000 Ada Generation>) | 2 | PTS |
| [NVIDIA RTX 4000 Ada Generation](<GPU/NVIDIA RTX 4000 Ada Generation>) | 2 | PTS |
| [NVIDIA RTX 6000 Ada Generation](<GPU/NVIDIA RTX 6000 Ada Generation>) | 4 | PHCS summary, PTS, source/partial |
| [NVIDIA RTX A1000](<GPU/NVIDIA RTX A1000>) | 2 | PTS |
| [NVIDIA RTX A2000](<GPU/NVIDIA RTX A2000>) | 1 | source/partial |
| [NVIDIA RTX A2000 Laptop GPU](<GPU/NVIDIA RTX A2000 Laptop GPU>) | 1 | source/partial |
| [NVIDIA RTX A400](<GPU/NVIDIA RTX A400>) | 1 | PTS |
| [NVIDIA RTX A4000](<GPU/NVIDIA RTX A4000>) | 3 | PHCS summary, PTS, source/partial |
| [NVIDIA RTX A5000](<GPU/NVIDIA RTX A5000>) | 2 | PHCS summary, source/partial |
| [NVIDIA RTX A6000](<GPU/NVIDIA RTX A6000>) | 2 | source/partial |
| [NVIDIA RTX PRO 2000 Blackwell](<GPU/NVIDIA RTX PRO 2000 Blackwell>) | 2 | PTS |
| [NVIDIA RTX PRO 4000 Blackwell](<GPU/NVIDIA RTX PRO 4000 Blackwell>) | 2 | PTS |
| [NVIDIA RTX PRO 4500 Blackwell](<GPU/NVIDIA RTX PRO 4500 Blackwell>) | 2 | PTS |
| [NVIDIA RTX PRO 5000 Blackwell](<GPU/NVIDIA RTX PRO 5000 Blackwell>) | 2 | PTS |
| [NVIDIA RTX PRO 6000 Blackwell Max-Q Workstation Edition](<GPU/NVIDIA RTX PRO 6000 Blackwell Max-Q Workstation Edition>) | 2 | PTS |
| [NVIDIA RTX PRO 6000 Blackwell Server Edition](<GPU/NVIDIA RTX PRO 6000 Blackwell Server Edition>) | 1 | PHCS summary |
| [NVIDIA RTX PRO 6000 Blackwell Workstation Edition](<GPU/NVIDIA RTX PRO 6000 Blackwell Workstation Edition>) | 4 | PHCS summary, PTS, source/partial |
| [NVIDIA T400](<GPU/NVIDIA T400>) | 1 | PTS |
| [NVIDIA T600](<GPU/NVIDIA T600>) | 1 | source/partial |
| [NVIDIA Tesla K20m](<GPU/NVIDIA Tesla K20m>) | 1 | source/partial |
| [NVIDIA Tesla K80](<GPU/NVIDIA Tesla K80>) | 2 | PHCS summary, source/partial |
| [NVIDIA Tesla M40](<GPU/NVIDIA Tesla M40>) | 1 | source/partial |
| [NVIDIA Tesla M6](<GPU/NVIDIA Tesla M6>) | 1 | PTS |
| [NVIDIA Tesla M60](<GPU/NVIDIA Tesla M60>) | 2 | PHCS summary, source/partial |
| [NVIDIA Tesla P100](<GPU/NVIDIA Tesla P100>) | 3 | PHCS summary, source/partial |
| [NVIDIA Tesla P4](<GPU/NVIDIA Tesla P4>) | 1 | source/partial |
| [NVIDIA Tesla P40](<GPU/NVIDIA Tesla P40>) | 1 | source/partial |
| [NVIDIA Tesla T4](<GPU/NVIDIA Tesla T4>) | 3 | PHCS summary, source/partial |
| [NVIDIA Tesla V100 PCIe](<GPU/NVIDIA Tesla V100 PCIe>) | 1 | source/partial |
| [NVIDIA Tesla V100 SXM2 16GB](<GPU/NVIDIA Tesla V100 SXM2 16GB>) | 8 | PHCS summary, raw/source |
| [NVIDIA TITAN RTX](<GPU/NVIDIA TITAN RTX>) | 2 | source/partial |
| [NVIDIA TITAN V](<GPU/NVIDIA TITAN V>) | 1 | source/partial |
| [NVIDIA TITAN Xp](<GPU/NVIDIA TITAN Xp>) | 1 | source/partial |
| [NVIDIA TU117GL](<GPU/NVIDIA TU117GL>) | 1 | PTS |
| [Valve Steam Deck (AMD Custom GPU 0932)](<GPU/Valve Steam Deck (AMD Custom GPU 0932)>) | 1 | source/partial |
<!-- FULL_GPU_INDEX_END -->

## 📖 Как читать результаты

Строка вида:

```
Speed.#1.........: 164.1 GH/s (69.78ms) @ Accel:512 Loops:1024 Thr:64 Vec:1
```

- `Speed.#1` — скорость устройства №1 (одна карта); `Speed.#*` — суммарно по всем;
- `GH/s` — миллиардов хешей в секунду;
- `Accel/Loops/Thr/Vec` — параметры автотюнинга ядра.

## 🔬 Как снять свой бенчмарк

```bash
hashcat -b                       # стандартный набор режимов
hashcat -b -O                    # оптимизированные ядра (быстрее, ограничение длины)
hashcat -b --benchmark-all       # ВСЕ поддерживаемые режимы
hashcat -b -m 3200               # конкретный режим (bcrypt)
```

## Новые частичные результаты

- [NVIDIA GeForce GTX 1660 SUPER](<GPU/NVIDIA GeForce GTX 1660 SUPER>) — пример из стартового поста, hashcat v6.1.1.
- [NVIDIA GeForce GTX 660](<GPU/NVIDIA GeForce GTX 660>) — частичная выборка режимов, Overclockers.ru.
- [NVIDIA GeForce RTX 3080](<GPU/NVIDIA GeForce RTX 3080>) — отдельный результат с workload profile 3.
- [NVIDIA GeForce GTX 770](<GPU/NVIDIA GeForce GTX 770>) — дополнительный прогон.
- [NVIDIA GeForce GTX 690](<GPU/NVIDIA GeForce GTX 690>) — mixed rig; скорости GTX 690 отделены от UHD 770.
- [NVIDIA GeForce RTX 4090](<GPU/NVIDIA GeForce RTX 4090>) — отдельный тюнинг-тест Hashcat mode 9800, v6.2.6.
- [AMD Radeon RX 5500 XT](<GPU/AMD Radeon RX 5500 XT>) — partial; лог сообщает `Insufficient memory available` в mode 0.
- [AMD Radeon 680M](<GPU/AMD Radeon 680M>) — только заявленная автором строка NTLM, без заголовка устройства.
- [Intel UHD Graphics 770](<GPU/Intel UHD Graphics 770>) — отдельный и смешанный прогоны; CPU Core i7-12700K отдельно не тестировался.
- [NVIDIA Quadro RTX 4000](<GPU/NVIDIA Quadro RTX 4000>) — Hashcat v7.1.2, проверяемый raw mode 22000; pure-kernel fallback.
- Таблицу рейтинга из [GermanAizek gist](https://gist.github.com/GermanAizek/f968d0bb213b2b7c8d9b35bbc4d031e4) не включал: автор уточняет, что это результаты проприетарного Hashcat-ng fork, а не оригинального Hashcat.
- [Intel UHD Graphics 630](<GPU/Intel UHD Graphics 630>) — v6.2.6, шесть режимов.
- [Intel HD Graphics 630](<GPU/Intel HD Graphics 630>) — v5.1.0-719, iTunes mode 14800; поздний исправленный результат.
- [AMD Radeon Pro 560](<GPU/AMD Radeon Pro 560>) — v5.1.0-719, iTunes mode 14800.
- [NVIDIA Tesla P4](<GPU/NVIDIA Tesla P4>) — v6.2.6; опубликованная таблица 25 режимов в двух runtime, без raw stdout (см. отдельную карточку).

Эти три карточки содержат опубликованные режимы, но не полный стандартный набор;
поэтому они не добавлены в основную таблицу сравнения.

## 🕳️ Известные пробелы

Подходящий сырой вывод пока не найден для: **AMD RDNA3 середины** (RX 7800 XT / 7700 XT /
7600 / 7900 GRE; для RX 7800 XT опубликованы PTS и PHCS aggregates без отдельного raw-файла),
**RDNA4** (RX 9070 / 9060 XT), **Instinct MI50/MI100/MI210/MI250/MI300A**
(для MI300X есть частичный нестандартный прогон), **Radeon Pro W6800/W7800/W7900**,
**RTX A4500**, **RTX 2000–5000 Ada**, desktop **RTX 3050 8GB** и **RTX 5050/5060**,
**Tesla K40**, **V100 32GB**, **A16/A30**, **B100/GB200**, **Apple M3 Ultra**, desktop
**Intel Arc** кроме A770 и большинство ноутбучных RTX (у RTX 4070 Laptop есть только
один PTS-режим без raw stdout). Tesla P40 добавлена по частичному
выводу 2019 года; A40 — по полному 8-карточному логу, MI300X — по частичному логу
сторонней сборки. Полный трекер — в [`COVERAGE.md`](COVERAGE.md).

## 🙏 Источники

Данные собраны из публичных бенчмарков сообщества hashcat:

- [its5Q/hashcat-benchmarks](https://github.com/its5Q/hashcat-benchmarks)
- [dosoos/hashcat_speeds](https://github.com/dosoos/hashcat_speeds)
- [siseci/hashcat-benchmark-comparison](https://github.com/siseci/hashcat-benchmark-comparison)
- [PHCS-gh/Hashcat-benchmark](https://github.com/PHCS-gh/Hashcat-benchmark)
- [whitefight18/hashcat_benchmark](https://github.com/whitefight18/hashcat_benchmark)
- Гисты: Chick3nman, epixoip, gartnera, greyltc, ConanChiles, pandada8, gerry, synch-cc,
  soxrok2212, rarecoil и др.
- GitHub issues: hashcat/hashcat #1489, #1497 (Tesla P100, Vega 56)
- [Overclockers.ru — тема о тестировании GPU в Hashcat](https://forums.overclockers.ru/viewtopic.php?f=31&t=626128)
- [DRIgnazGortngschirl/Benchmark-Scores-of-HashCAT](https://github.com/DRIgnazGortngschirl/Benchmark-Scores-of-HashCAT)
- Оригинальный тест Apple M3 Max — из этого репозитория.

Точная ссылка на источник указана **в каждом** документе.

## ⚖️ Дисклеймер

Материал предназначен для **легального** аудита паролей, оценки стойкости хешей,
образовательных целей и подбора оборудования. Используйте только на системах,
для которых у вас есть разрешение.
