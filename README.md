# 🔓 HashCat Benchmark — коллекция тестов GPU

Максимально полная подборка результатов бенчмарка **`hashcat -b`** для видеокарт
**всех поколений** — от старых Maxwell/Polaris до новейших Blackwell и RDNA 3,
включая профессиональные (Tesla/A100/H100), рабочие станции и майнинговые карты.

> Каждая видеокарта — **отдельная папка**. Внутри — один или несколько документов
> (`.md`) с указанием **вендора + названия карты**, таблицей ключевых результатов
> и **полным** необработанным выводом `hashcat -b`.

---

## 📊 Что внутри

- **89 видеокарт** (AMD: 12 · Apple: 13 · Intel: 2 · NVIDIA: 62)
- **124 документов** с бенчмарками (по нескольким источникам, версиям hashcat и конфигурациям — 1×, 4×, 8× и т.д.)
- Все поколения: NVIDIA (Maxwell → Pascal → Turing → Ampere → Ada → **Blackwell**),
  AMD (Polaris → Vega → RDNA → RDNA 2 → **RDNA 3**), Intel Arc, Apple Silicon.

## 🗂️ Структура репозитория

```
HashCat-Benchmark/
├── NVIDIA GeForce RTX 4090/
│   ├── NVIDIA GeForce RTX 4090 — Chick3nman v6.2.6.md
│   ├── NVIDIA GeForce RTX 4090 — dosoos v6.2.6.md
│   └── NVIDIA GeForce RTX 4090 — PHCS-gh ?.md
├── AMD Radeon RX 7900 XT/
│   └── AMD Radeon RX 7900 XT — gartnera v6.2.6.md
├── Intel Arc B580/
│   └── Intel Arc B580 — greyltc v6.2.6-851-g6716447df.md
└── ...
```

Имя папки = **вендор + модель**. Имя файла = `модель — источник версия [конфигурация].md`.

---

## 🏆 Сводная таблица (скорость на одну карту)

Значения — **на одну видеокарту** (`Speed.#1`), режим оптимизированного ядра (`-O`).
Отсортировано по MD5. Единицы: H/s → kH/s → MH/s → GH/s → TH/s.

Основные хеш-режимы: **MD5** (0), **NTLM** (1000), **SHA2-256** (1400),
**SHA2-512** (1700), **WPA2** (22000, PBKDF2-PMKID/EAPOL), **bcrypt** (3200).

| # | GPU | MD5 | NTLM | SHA2-256 | SHA2-512 | WPA2 | bcrypt |
|--:|-----|----:|-----:|---------:|---------:|-----:|-------:|
| 1 | [NVIDIA GeForce RTX 5090](<NVIDIA GeForce RTX 5090>) | 221 GH/s | 340 GH/s | 28.4 GH/s | 10.0 GH/s | 3.4 MH/s | 305 kH/s |
| 2 | [NVIDIA GeForce RTX 4090](<NVIDIA GeForce RTX 4090>) | 164 GH/s | 288 GH/s | 22.0 GH/s | 7.5 GH/s | 2.5 MH/s | 184 kH/s |
| 3 | [NVIDIA RTX 6000 Ada Generation](<NVIDIA RTX 6000 Ada Generation>) | 132 GH/s | 216 GH/s | 19.2 GH/s | 6.4 GH/s | 2.3 MH/s | 201 kH/s |
| 4 | [NVIDIA GeForce RTX 5080](<NVIDIA GeForce RTX 5080>) | 105 GH/s | 164 GH/s | 13.6 GH/s | 4.9 GH/s | 1.6 MH/s | 124 kH/s |
| 5 | [NVIDIA GeForce RTX 4080 SUPER](<NVIDIA GeForce RTX 4080 SUPER>) | 99.6 GH/s | 176 GH/s | 13.3 GH/s | 4.6 GH/s | 1.6 MH/s | 146 kH/s |
| 6 | [NVIDIA GeForce RTX 4080](<NVIDIA GeForce RTX 4080>) | 98.3 GH/s | 173 GH/s | 13.1 GH/s | 4.5 GH/s | 1.5 MH/s | 131 kH/s |
| 7 | [NVIDIA GeForce RTX 5070 Ti](<NVIDIA GeForce RTX 5070 Ti>) | 88.2 GH/s | 138 GH/s | 11.4 GH/s | 4.1 GH/s | 1.4 MH/s | 108 kH/s |
| 8 | [NVIDIA H100 PCIe](<NVIDIA H100 PCIe>) | 87.5 GH/s | 159 GH/s | 12.2 GH/s | 4.1 GH/s | 1.5 MH/s | 252 kH/s |
| 9 | [NVIDIA GeForce RTX 4070 Ti SUPER](<NVIDIA GeForce RTX 4070 Ti SUPER>) | 85.0 GH/s | 149 GH/s | 11.3 GH/s | 3.8 GH/s | 1.3 MH/s | 124 kH/s |
| 10 | [NVIDIA GeForce RTX 3090 Ti](<NVIDIA GeForce RTX 3090 Ti>) | 79.1 GH/s | 143 GH/s | 10.8 GH/s | 3.6 GH/s | 1.3 MH/s | 91.0 kH/s |
| 11 | [NVIDIA GeForce RTX 3090](<NVIDIA GeForce RTX 3090>) | 71.7 GH/s | 124 GH/s | 9.6 GH/s | 3.2 GH/s | 1.1 MH/s | 108 kH/s |
| 12 | [NVIDIA GeForce RTX 4070 SUPER](<NVIDIA GeForce RTX 4070 SUPER>) | 69.9 GH/s | 123 GH/s | 9.3 GH/s | 3.2 GH/s | 1.1 MH/s | 103 kH/s |
| 13 | [NVIDIA GeForce RTX 3080 Ti](<NVIDIA GeForce RTX 3080 Ti>) | 69.2 GH/s | 120 GH/s | 9.3 GH/s | 3.1 GH/s | 1.1 MH/s | 105 kH/s |
| 14 | [NVIDIA A800 80GB PCIe](<NVIDIA A800 80GB PCIe>) | 68.1 GH/s | 116 GH/s | 9.5 GH/s | 3.2 GH/s | 1.1 MH/s | 138 kH/s |
| 15 | [NVIDIA GeForce RTX 4070 Ti](<NVIDIA GeForce RTX 4070 Ti>) | 67.8 GH/s | 115 GH/s | 9.1 GH/s | 3.0 GH/s | 917 kH/s | 109 kH/s |
| 16 | [NVIDIA A100 PCIe 40GB](<NVIDIA A100 PCIe 40GB>) | 64.9 GH/s | 120 GH/s | 9.4 GH/s | 3.1 GH/s | 1.1 MH/s | 138 kH/s |
| 17 | [NVIDIA TITAN RTX](<NVIDIA TITAN RTX>) | 64.0 GH/s | 112 GH/s | 8.7 GH/s | 2.8 GH/s | — | 39.6 kH/s |
| 18 | [AMD Radeon RX 7900 XT](<AMD Radeon RX 7900 XT>) | 61.7 GH/s | 97.8 GH/s | 10.6 GH/s | 2.1 GH/s | 1.2 MH/s | 83.4 kH/s |
| 19 | [AMD Radeon RX 6950 XT](<AMD Radeon RX 6950 XT>) | 61.6 GH/s | 100.0 GH/s | 10.4 GH/s | 2.8 GH/s | 1.2 MH/s | 61.1 kH/s |
| 20 | [NVIDIA GeForce RTX 5070](<NVIDIA GeForce RTX 5070>) | 60.7 GH/s | 92.3 GH/s | 7.8 GH/s | 2.3 GH/s | 961 kH/s | 85.7 kH/s |
| 21 | [NVIDIA GeForce RTX 4070](<NVIDIA GeForce RTX 4070>) | 58.8 GH/s | 101 GH/s | 7.9 GH/s | 2.7 GH/s | 928 kH/s | 86.3 kH/s |
| 22 | [NVIDIA Tesla V100 SXM2 16GB](<NVIDIA Tesla V100 SXM2 16GB>) | 55.7 GH/s | 99.8 GH/s | 7.6 GH/s | 2.4 GH/s | 884 kH/s | 78.7 kH/s |
| 23 | [NVIDIA GeForce RTX 2080 Ti](<NVIDIA GeForce RTX 2080 Ti>) | 53.4 GH/s | 94.7 GH/s | 7.3 GH/s | 2.4 GH/s | 853 kH/s | 63.3 kH/s |
| 24 | [AMD Radeon RX 6800 XT](<AMD Radeon RX 6800 XT>) | 52.4 GH/s | 85.4 GH/s | 8.7 GH/s | 2.3 GH/s | 1.1 MH/s | 58.2 kH/s |
| 25 | [NVIDIA GeForce RTX 3080](<NVIDIA GeForce RTX 3080>) | 51.0 GH/s | 90.1 GH/s | 6.9 GH/s | 2.3 GH/s | 809 kH/s | 74.7 kH/s |
| 26 | [NVIDIA GeForce RTX 5060 Ti](<NVIDIA GeForce RTX 5060 Ti>) | 47.0 GH/s | 72.2 GH/s | 6.0 GH/s | 1.7 GH/s | 738 kH/s | 66.3 kH/s |
| 27 | [NVIDIA GeForce RTX 3070 Ti](<NVIDIA GeForce RTX 3070 Ti>) | 44.4 GH/s | 82.1 GH/s | 6.1 GH/s | 2.0 GH/s | 716 kH/s | 68.5 kH/s |
| 28 | [NVIDIA CMP 170HX](<NVIDIA CMP 170HX>) | 43.4 GH/s | 73.6 GH/s | 6.1 GH/s | 2.1 GH/s | 719 kH/s | 92.1 kH/s |
| 29 | [NVIDIA GeForce RTX 4060 Ti](<NVIDIA GeForce RTX 4060 Ti>) | 43.0 GH/s | 76.1 GH/s | 5.7 GH/s | 2.0 GH/s | 675 kH/s | 62.3 kH/s |
| 30 | [NVIDIA CMP 50HX](<NVIDIA CMP 50HX>) | 42.7 GH/s | 71.4 GH/s | 6.1 GH/s | 2.0 GH/s | 706 kH/s | 45.9 kH/s |
| 31 | [NVIDIA CMP 90HX](<NVIDIA CMP 90HX>) | 41.5 GH/s | 70.0 GH/s | 5.9 GH/s | 2.0 GH/s | 688 kH/s | 62.4 kH/s |
| 32 | [NVIDIA GeForce RTX 2080 SUPER](<NVIDIA GeForce RTX 2080 SUPER>) | 40.1 GH/s | 70.0 GH/s | 5.7 GH/s | 1.8 GH/s | — | 27.5 kH/s |
| 33 | [NVIDIA GeForce RTX 2080](<NVIDIA GeForce RTX 2080>) | 37.1 GH/s | 53.0 GH/s | 5.4 GH/s | 1.8 GH/s | — | 18.5 kH/s |
| 34 | [NVIDIA GeForce RTX 3070](<NVIDIA GeForce RTX 3070>) | 35.5 GH/s | 61.4 GH/s | 4.8 GH/s | 1.6 GH/s | 558 kH/s | 60.3 kH/s |
| 35 | [NVIDIA GeForce GTX 1080 Ti](<NVIDIA GeForce GTX 1080 Ti>) | 35.2 GH/s | 58.3 GH/s | 4.4 GH/s | 1.4 GH/s | — | 21.4 kH/s |
| 36 | [NVIDIA GeForce RTX 3060 Ti](<NVIDIA GeForce RTX 3060 Ti>) | 34.8 GH/s | 62.0 GH/s | 4.7 GH/s | 1.6 GH/s | 562 kH/s | 51.6 kH/s |
| 37 | [NVIDIA GeForce RTX 2070 SUPER](<NVIDIA GeForce RTX 2070 SUPER>) | 34.8 GH/s | 58.3 GH/s | 4.3 GH/s | 1.4 GH/s | 493 kH/s | 30.0 kH/s |
| 38 | [NVIDIA RTX A4000](<NVIDIA RTX A4000>) | 33.3 GH/s | 43.3 GH/s | 2.9 GH/s | 1.3 GH/s | 470 kH/s | 53.7 kH/s |
| 39 | [AMD Radeon VII](<AMD Radeon VII>) | 33.1 GH/s | 54.9 GH/s | 4.9 GH/s | 1.5 GH/s | — | 24.1 kH/s |
| 40 | [AMD Radeon RX 6700 XT](<AMD Radeon RX 6700 XT>) | 32.1 GH/s | 51.8 GH/s | 5.4 GH/s | 1.4 GH/s | 647 kH/s | 29.6 kH/s |
| 41 | [NVIDIA GeForce RTX 3070 Laptop GPU](<NVIDIA GeForce RTX 3070 Laptop GPU>) | 31.9 GH/s | 58.7 GH/s | 4.4 GH/s | 1.5 GH/s | 520 kH/s | 53.9 kH/s |
| 42 | [AMD Radeon RX Vega 64](<AMD Radeon RX Vega 64>) | 31.6 GH/s | 51.7 GH/s | 4.6 GH/s | 1.2 GH/s | 522 kH/s | 20.7 kH/s |
| 43 | [NVIDIA GeForce RTX 2060 SUPER](<NVIDIA GeForce RTX 2060 SUPER>) | 29.1 GH/s | 51.0 GH/s | 3.9 GH/s | 1.3 GH/s | 450 kH/s | 30.9 kH/s |
| 44 | [NVIDIA GeForce RTX 4060](<NVIDIA GeForce RTX 4060>) | 28.6 GH/s | 48.8 GH/s | 4.0 GH/s | 1.2 GH/s | 461 kH/s | 38.7 kH/s |
| 45 | [NVIDIA GeForce RTX 2060](<NVIDIA GeForce RTX 2060>) | 27.1 GH/s | 47.6 GH/s | 3.6 GH/s | 1.2 GH/s | 418 kH/s | 28.3 kH/s |
| 46 | [NVIDIA GeForce RTX 2070](<NVIDIA GeForce RTX 2070>) | 26.9 GH/s | 40.0 GH/s | 4.0 GH/s | 1.3 GH/s | — | 14.3 kH/s |
| 47 | [NVIDIA P102-100](<NVIDIA P102-100>) | 26.5 GH/s | 43.3 GH/s | 3.9 GH/s | 1.3 GH/s | 549 kH/s | 27.2 kH/s |
| 48 | [Apple M2 Ultra](<Apple M2 Ultra>) | 26.5 GH/s | 44.5 GH/s | 4.1 GH/s | 1.0 GH/s | 482 kH/s | 15.3 kH/s |
| 49 | [AMD Radeon RX 6600 XT](<AMD Radeon RX 6600 XT>) | 25.6 GH/s | 40.6 GH/s | 4.2 GH/s | 1.1 GH/s | 496 kH/s | 29.9 kH/s |
| 50 | [NVIDIA GeForce RTX 3060](<NVIDIA GeForce RTX 3060>) | 25.2 GH/s | 44.2 GH/s | 3.4 GH/s | 1.1 GH/s | 395 kH/s | 36.7 kH/s |
| 51 | [Intel Arc B580](<Intel Arc B580>) | 24.7 GH/s | 33.3 GH/s | 1.3 GH/s | 318 MH/s | 580 kH/s | 15.4 kH/s |
| 52 | [NVIDIA GeForce GTX 1080](<NVIDIA GeForce GTX 1080>) | 24.7 GH/s | 43.0 GH/s | 3.1 GH/s | 1.0 GH/s | 440 kH/s | 21.6 kH/s |
| 53 | [NVIDIA GeForce GTX 1070 Ti](<NVIDIA GeForce GTX 1070 Ti>) | 24.3 GH/s | 41.3 GH/s | 3.0 GH/s | 986 MH/s | 424 kH/s | 21.0 kH/s |
| 54 | [Intel Arc A770M](<Intel Arc A770M>) | 24.1 GH/s | 40.4 GH/s | 114 MH/s | 806 MH/s | 212 kH/s | — |
| 55 | [AMD Radeon RX 5700 XT](<AMD Radeon RX 5700 XT>) | 23.8 GH/s | 38.1 GH/s | 4.1 GH/s | 1.1 GH/s | — | 18.2 kH/s |
| 56 | [Apple M4 Max](<Apple M4 Max>) | 22.1 GH/s | 37.7 GH/s | 3.6 GH/s | 708 MH/s | 486 kH/s | 21.3 kH/s |
| 57 | [NVIDIA Tesla P100](<NVIDIA Tesla P100>) | 22.0 GH/s | — | — | — | — | — |
| 58 | [NVIDIA GeForce GTX 1070](<NVIDIA GeForce GTX 1070>) | 19.6 GH/s | 33.8 GH/s | 2.5 GH/s | 809 MH/s | 350 kH/s | 16.7 kH/s |
| 59 | [NVIDIA GeForce GTX 1660 SUPER](<NVIDIA GeForce GTX 1660 SUPER>) | 19.6 GH/s | 34.9 GH/s | 2.6 GH/s | 878 MH/s | 305 kH/s | 20.1 kH/s |
| 60 | [Apple M3 Max](<Apple M3 Max>) | 19.1 GH/s | 32.6 GH/s | 3.0 GH/s | 594 MH/s | 408 kH/s | 32.6 kH/s |
| 61 | [NVIDIA GeForce GTX 1660](<NVIDIA GeForce GTX 1660>) | 19.0 GH/s | 32.6 GH/s | 2.4 GH/s | 795 MH/s | 288 kH/s | 19.4 kH/s |
| 62 | [NVIDIA GeForce GTX 980 Ti](<NVIDIA GeForce GTX 980 Ti>) | 18.9 GH/s | 31.7 GH/s | 2.3 GH/s | 793 MH/s | — | 10.9 kH/s |
| 63 | [Apple M1 Ultra](<Apple M1 Ultra>) | 17.1 GH/s | 28.6 GH/s | 1.8 GH/s | 575 MH/s | 297 kH/s | 10.1 kH/s |
| 64 | [NVIDIA GeForce GTX TITAN X](<NVIDIA GeForce GTX TITAN X>) | 15.8 GH/s | 25.3 GH/s | 2.2 GH/s | 742 MH/s | 325 kH/s | 14.7 kH/s |
| 65 | [AMD Radeon RX 590](<AMD Radeon RX 590>) | 14.0 GH/s | 22.6 GH/s | 1.9 GH/s | 486 MH/s | 236 kH/s | 10.6 kH/s |
| 66 | [Apple M1 Max](<Apple M1 Max>) | 13.2 GH/s | 21.1 GH/s | 2.0 GH/s | 396 MH/s | 248 kH/s | 9.3 kH/s |
| 67 | [NVIDIA P104-100](<NVIDIA P104-100>) | 13.2 GH/s | 21.1 GH/s | 1.9 GH/s | 643 MH/s | 269 kH/s | 16.6 kH/s |
| 68 | [NVIDIA GeForce GTX 1060 6GB](<NVIDIA GeForce GTX 1060 6GB>) | 13.1 GH/s | 22.6 GH/s | 1.7 GH/s | 535 MH/s | 235 kH/s | 11.0 kH/s |
| 69 | [Apple M2 Max](<Apple M2 Max>) | 12.9 GH/s | 22.4 GH/s | 2.0 GH/s | 406 MH/s | 246 kH/s | 8.2 kH/s |
| 70 | [NVIDIA GeForce GTX 1650](<NVIDIA GeForce GTX 1650>) | 12.6 GH/s | 22.8 GH/s | 1.7 GH/s | 577 MH/s | 199 kH/s | 13.1 kH/s |
| 71 | [NVIDIA GeForce GTX 980](<NVIDIA GeForce GTX 980>) | 11.4 GH/s | 23.2 GH/s | 1.5 GH/s | 490 MH/s | 186 kH/s | 11.4 kH/s |
| 72 | [NVIDIA GeForce GTX 1060 3GB](<NVIDIA GeForce GTX 1060 3GB>) | 10.7 GH/s | 16.1 GH/s | 1.1 GH/s | 362 MH/s | 168 kH/s | 8.1 kH/s |
| 73 | [NVIDIA GeForce GTX 970](<NVIDIA GeForce GTX 970>) | 10.4 GH/s | 21.4 GH/s | 1.3 GH/s | 410 MH/s | — | 9.0 kH/s |
| 74 | [AMD Radeon R9 290](<AMD Radeon R9 290>) | 10.2 GH/s | 18.0 GH/s | 1.4 GH/s | 99.8 MH/s | — | 4.5 kH/s |
| 75 | [NVIDIA P106-100](<NVIDIA P106-100>) | 9.5 GH/s | 16.4 GH/s | 1.4 GH/s | 336 MH/s | — | 5.9 kH/s |
| 76 | [Apple M4 Pro](<Apple M4 Pro>) | 9.0 GH/s | 15.7 GH/s | 1.4 GH/s | 292 MH/s | 196 kH/s | 7.5 kH/s |
| 77 | [Apple M2 Pro](<Apple M2 Pro>) | 7.0 GH/s | 12.0 GH/s | 1.0 GH/s | 648 MH/s | 126 kH/s | 4.4 kH/s |
| 78 | [Apple M3 Pro](<Apple M3 Pro>) | 6.8 GH/s | 11.7 GH/s | 1.1 GH/s | 220 MH/s | 146 kH/s | 6.0 kH/s |
| 79 | [NVIDIA GeForce GTX 960](<NVIDIA GeForce GTX 960>) | 6.5 GH/s | 11.9 GH/s | 862 MH/s | 255 MH/s | — | 3.8 kH/s |
| 80 | [NVIDIA GeForce GTX 1650 Ti](<NVIDIA GeForce GTX 1650 Ti>) | 6.4 GH/s | 11.6 GH/s | 850 MH/s | 254 MH/s | 157 kH/s | 1.4 kH/s |
| 81 | [AMD Radeon RX 580](<AMD Radeon RX 580>) | 5.9 GH/s | 9.7 GH/s | 843 MH/s | 154 MH/s | 65.0 kH/s | 4.5 kH/s |
| 82 | [NVIDIA GeForce GTX 1050 Ti](<NVIDIA GeForce GTX 1050 Ti>) | 5.6 GH/s | 5.6 GH/s | 375 MH/s | 94.8 MH/s | 50.9 kH/s | 4.4 kH/s |
| 83 | [Apple M1 Pro](<Apple M1 Pro>) | 5.5 GH/s | 9.0 GH/s | 867 MH/s | 224 MH/s | 102 kH/s | 3.4 kH/s |
| 84 | [NVIDIA GeForce GTX 1050](<NVIDIA GeForce GTX 1050>) | 5.2 GH/s | 8.7 GH/s | 744 MH/s | 249 MH/s | — | 3.5 kH/s |
| 85 | [NVIDIA Tesla K80](<NVIDIA Tesla K80>) | 4.6 GH/s | 7.7 GH/s | 785 MH/s | 257 MH/s | — | 2.6 kH/s |
| 86 | [Apple M3](<Apple M3>) | 3.3 GH/s | — | 536 MH/s | — | — | — |
| 87 | [Apple M1](<Apple M1>) | 2.8 GH/s | 4.8 GH/s | 300 MH/s | 97.6 MH/s | 48.9 kH/s | 2.1 kH/s |
| 88 | [Apple M2](<Apple M2>) | 2.3 GH/s | 2.7 GH/s | 339 MH/s | 120 MH/s | 67.4 kH/s | 2.9 kH/s |
| 89 | [AMD Radeon (Pro) Vega 56](<AMD Radeon (Pro) Vega 56>) | — | — | — | — | — | — |

> ⚠️ Цифры взяты из разных прогонов (разные драйверы, ОС, версии hashcat, разгон),
> поэтому это **ориентир**, а не строгое сравнение. Точные условия — в каждом
> отдельном документе. Прочерк «—» означает, что режим пропущен/не тестировался
> в исходном прогоне либо файл в старом формате oclHashcat без номеров режимов.

---

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

## 🕳️ Известные пробелы

Реальный (не выдуманный) полный вывод `hashcat -b` не удалось найти для: **AMD Radeon RX 7900 XTX**,
**RX 6900 XT**, **RX 570**, **RX 6600** (не XT), **NVIDIA TITAN V**, **RTX 3050** (десктопная),
**RTX 4050 Laptop**, **Intel Arc A380**, **Arc A750**. По части из них есть только сводные таблицы
рейтингов (одно число, без сырого вывода) или посты на форуме hashcat.net, недоступном из окружения,
в котором собирался этот репозиторий — туда данные не включались, чтобы не подсовывать нецельный
или переоформленный результат вместо настоящего вывода консоли.

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
- [DRIgnazGortngschirl/Benchmark-Scores-of-HashCAT](https://github.com/DRIgnazGortngschirl/Benchmark-Scores-of-HashCAT)
- Оригинальный тест Apple M3 Max — из этого репозитория.

Точная ссылка на источник указана **в каждом** документе.

## ⚖️ Дисклеймер

Материал предназначен для **легального** аудита паролей, оценки стойкости хешей,
образовательных целей и подбора оборудования. Используйте только на системах,
для которых у вас есть разрешение.
