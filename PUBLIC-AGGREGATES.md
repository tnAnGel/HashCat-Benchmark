# Публичные агрегаты Hashcat — кандидаты без локального raw stdout

Этот реестр объясняет публичные обработанные результаты и ограничения их
интерпретации. Индивидуальные значения, когда они полезны для каталога, лежат
отдельными `.md` внутри папок [`GPU/`](GPU) и [`CPU/`](CPU), а не в выгрузках
CSV. Comparison-only и PTS-значения не заменяют raw stdout и не считаются
сопоставимым полным `hashcat -b`.

## OpenBenchmarking: индивидуальные PTS-записи (не raw stdout)

У этих записей есть отдельный публичный ID, и модель GPU указана в описании
системы. PTS публикует извлечённые значения по режимам, но это не исходный
консольный stdout Hashcat, поэтому значение не представляется как raw; обработанная
запись лежит в отдельной `.md`-карточке соответствующей папки `GPU/`.

- **Intel Arc Pro B50** — [result `2602079-NE-HASHCAT2068`](https://openbenchmarking.org/result/2602079-NE-HASHCAT2068), Hashcat 7.0. Заголовок результата указывает B50 16GB с отключённой ECC, а поле Graphics на странице — B50 2GB, поэтому объём памяти отмечен как противоречивый.
- **AMD Radeon 8060S** — [result `2505218-NE-HASHCAT0141`](https://openbenchmarking.org/result/2505218-NE-HASHCAT0141), Hashcat 6.2.4; система также указывает Ryzen AI MAX+ 395 как хост, не как тестируемый CPU.

Значения ниже — три PTS-повтора на режим в единицах метрики PTS (не исходные
строки `Speed` из stdout Hashcat). Пустые серии означают, что режим был
опубликован, но измерение отсутствовало.

### Intel Arc Pro B50 — Hashcat 7.0

| Режим | PTS trials |
|---|---:|
| MD5 | 16920500000, 16656900000, 16776600000 |
| SHA1 | 7522000000, 7520100000, 7499100000 |
| 7-Zip | 133400, 133900, 134100 |
| bcrypt | нет значений |
| SHA-256 | 2667800000, 2657700000, 2654700000 |
| SHA-512 | 382900000, 380500000, 379900000 |
| LastPass | нет значений |
| TrueCrypt RIPEMD160 + XTS | 215100, 215300, 215100 |
| Kerberos 5 TGS-REP etype 23 | 187300000, 187200000, 186900000 |

### AMD Radeon 8060S — Hashcat 6.2.4

| Режим | PTS trials |
|---|---:|
| MD5 | 31418600000, 31908700000, 31785700000 |
| SHA1 | 13255700000, 13158400000, 13164500000 |
| 7-Zip | 647000, 644500, 645800 |
| SHA-512 | 1409800000, 1433900000, 1468400000 |
| TrueCrypt RIPEMD160 + XTS | 393100, 390800, 392000 |

Это **индивидуальные обработанные значения**, а не агрегированные средние по
разным компьютерам. Исходные выгрузки доступны через параметр `export=csv-all`
на страницах результатов; PTS не даёт из этих страниц полный сырой stdout
Hashcat. В репозитории они разложены по отдельным per-device `.md` в `GPU/`,
отдельно от raw-карточек.

### Ещё индивидуальные PTS-прогоны

Результаты ниже — отдельные PTS-прогоны, но значения сведены/усреднены из
повторов. Они дают подтверждение теста модели, однако не заменяют исходные
строки `Speed.#N`.

| GPU | Версия / режим | Публичные значения | PTS result |
|---|---|---:|---|
| AMD Radeon RX 9070 | 6.2.4 / MD5, SHA1, SHA-512, 7-Zip, TrueCrypt | SHA1 19.718 GH/s; SHA-512 2.1411 GH/s; есть и другие режимы | [2506064-PTS-NEWGPUCO48](https://openbenchmarking.org/result/2506064-PTS-NEWGPUCO48) |
| AMD Radeon RX 9060 XT | 6.2.4 / MD5, SHA1, SHA-512 и др. | MD5 30.2054–30.4498 GH/s; SHA1 12.7655–12.7901 GH/s; SHA-512 1.4015–1.4051 GH/s | [2506067](https://openbenchmarking.org/result/2506067-PTS-NEWGPUCO98), [2506064](https://openbenchmarking.org/result/2506064-PTS-NEWGPUCO48) |
| AMD Radeon 8060S | 7.1.2 / 12 режимов | MD5 25.3882–25.3922 GH/s; NTLM 46.561–46.7924 GH/s; SHA1 11.5708–11.6220 GH/s; WPA 586.4–591.8 kH/s | [2602146-NE-HASHCAT2072](https://openbenchmarking.org/result/2602146-NE-HASHCAT2072) |
| AMD Radeon Pro W7900 | 7.0 / MD5, SHA-256 | aggregate MD5 60.685 GH/s (7 результатов); SHA-256 11.126 GH/s (7) | [individual result](https://openbenchmarking.org/result/2405093-NE-HASHCATTE58) |
| NVIDIA RTX A4500 | 6.2.4 / MD5, SHA1, SHA-512 | MD5 87.8816 / 87.1732 / 86.3359 GH/s; SHA1 около 28.5 GH/s | [2308073-NE-CATPALACE31](https://openbenchmarking.org/result/2308073-NE-CATPALACE31) |
| NVIDIA RTX 2000 Ada | 7.1.2 / SHA-256 | 3.3143 / 3.2943 / 3.2950 / 3.2911 / 3.2839 GH/s | [2605138-PTS-NVIDIART24](https://openbenchmarking.org/result/2605138-PTS-NVIDIART24) |
| NVIDIA RTX 4000 Ada | 7.1.2 / SHA-256 | 6.5751 / 6.5545 / 6.5397 / 6.5409 / 6.5348 GH/s | [2605138-PTS-NVIDIART24](https://openbenchmarking.org/result/2605138-PTS-NVIDIART24) |
| NVIDIA RTX 2000 Ada Laptop GPU | 7.0 / SHA-256 | 2.4869 / 2.5466 / 2.4805 GH/s | [2510073-NE-HASHCATSH20](https://openbenchmarking.org/result/2510073-NE-HASHCATSH20) |
| NVIDIA Quadro RTX 5000 with Max-Q Design | 6.2.4 / MD5, SHA-1, SHA-512, 7-Zip | 24.855 GH/s; 8.719 GH/s; 1.064 GH/s; 383.1 kH/s (5 each) | [PTS result/profile](https://openbenchmarking.org/test/pts/hashcat%26eval%3D56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9) |
| NVIDIA Quadro P2000 (desktop) | 6.2.4 / SHA-1, SHA-512, 7-Zip | 5.250 GH/s; 219.1 MH/s; 208.8 kH/s (3 each) | [PTS SHA-1 profile](https://openbenchmarking.org/performance/test/pts/hashcat/b5a7b3b27cec5d9e085c3d68a1cad8cda5ef0f24) |
| NVIDIA Tesla M6 | 6.2.4 / MD5, SHA-1, SHA-512, 7-Zip | 8.795 GH/s; 2.979 GH/s; 330.3 MH/s; 119.1 kH/s (3 each) | [PTS result/profile](https://openbenchmarking.org/test/pts/hashcat%26eval%3D56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9) |
| NVIDIA GeForce MX230 | 6.1.1 / MD5 | 2.018 GH/s (7) | [PTS profile](https://openbenchmarking.org/test/pts/hashcat%26eval%3D56eb2bb43fd8ce50f21bde1f712a2c57b37a8ac9) |
| Intel Arc A380 | 6.2.4 / MD5 | mean ≈10.089 GH/s | [2310172](https://openbenchmarking.org/result/2310172-PTS-INTELARC33) |
| Intel Arc A580 | 6.2.4 / MD5 | mean ≈26.187 GH/s | [2310172](https://openbenchmarking.org/result/2310172-PTS-INTELARC33) |
| Intel Arc A750 | 6.2.4 / MD5 | mean ≈31.010 GH/s | [2412092](https://openbenchmarking.org/result/2412092-NE-INTELGPU196) |
| Intel Arc A580 DG2 | 7.1.2 / MD5 and SHA-256 | 26.264 GH/s (13); 6.160 GH/s (4) | [MD5](https://openbenchmarking.org/performance/test/pts/hashcat/2f1e49c858bdaf551168a2c36422c3bcd6dbf083), [SHA-256](https://openbenchmarking.org/performance/test/pts/hashcat/71ae6c8974b17ccdfcf3f872aab62d85c629e59e) |
| Intel Arc B570 BMG G21 | 7.1.2 / SHA-256 | 3.724 GH/s (3) | [PTS SHA-256](https://openbenchmarking.org/performance/test/pts/hashcat/71ae6c8974b17ccdfcf3f872aab62d85c629e59e) |
| Intel Arc B570 | 6.2.4 / SHA-512 | mean ≈528.533 MH/s | [2506064](https://openbenchmarking.org/result/2506064-PTS-NEWGPUCO48) |
| Intel Arc Pro B70 | 7.1.2 / MD5 | mean ≈38.541 GH/s | [2604157](https://openbenchmarking.org/result/2604157-PTS-INTELCOM83) |
| Intel HD Graphics 4600 | 7.1.2 / MD5 | mean ≈3.789 GH/s | [2605317-TWEA-TTTT52384](https://openbenchmarking.org/result/2605317-TWEA-TTTT52384) |
| Intel Iris Xe TGL GT2 | 7.1.2 / MD5, SHA-256, SHA-512 | ≈3.045 GH/s; 542.285 MH/s; 98.354 MH/s | [aggregates](https://openbenchmarking.org/performance/test/pts/hashcat/2f1e49c858bdaf551168a2c36422c3bcd6dbf083) |
| MSI Intel Iris Xe ADL GT2 | 7.1.2 / MD5, SHA-256, SHA-512 | ≈2.852 GH/s; 500.689 MH/s; 93.879 MH/s | [aggregates](https://openbenchmarking.org/performance/test/pts/hashcat/bb70ab4002871eaf41c4c257184d478de05cb604) |

У Radeon 8060S PTS показывает `Processor` как AMD Ryzen AI MAX+ 395 и `Graphics`
как 8060S; поэтому её PTS-результат относится к графическому устройству, не CPU.

**Неоднозначный PTS алиас:** [результат на Ryzen AI 9 HX 370](https://openbenchmarking.org/result/2602234-NE-DDD90727817)
показывает `Radeon 880M / 890M` как одну общую graphics device string. Без
уточнения конкретного APU/устройства нельзя разнести его скорости на две модели.

### Индивидуальные PTS result-файлы (JSON; без stdout Hashcat)

На странице [Find More Test Results](https://openbenchmarking.org/test/pts/hashcat%26search)
видимые на странице публичные result-файлы разнесены по папкам GPU в отдельные
карточки OpenBenchmarking PTS. В карточках сохранены 1132 из 1146 строк
индивидуальных измерений по result ID, включая точные значения повторов, даты,
версии Hashcat, аргументы, hardware labels и ссылки на исходные записи. Остальные
14 строк помечены только `llvmpipe`; это software renderer, который не позволяет
установить Hashcat-устройство, поэтому скорости не приписаны CPU или GPU.
Таблицы профильных
агрегатов также перенесены в самостоятельные Markdown-карточки внутри папок GPU;
CSV-выгрузки больше не используются.

Это более детальные PTS-измерения, но не консольный `hashcat -b` stdout. Поле
`Processor` описывает хост; профиль имеет тип **Graphics**, поэтому CPU в этой
выгрузке не считается протестированным CPU Hashcat. Композитный label `RTX 5090
Laptop GPU + Intel` сохранён как system-level результат, а не скорость одной
карты. Строка `Radeon 880M / 890M` привязана к Radeon 890M только там, где PTS
указывает Ryzen AI 9 HX 370; сопоставление подтверждается спецификацией AMD и
помечено в карточке. `llvmpipe` не приписан ни CPU, ни GPU.

Нечёткие PTS labels вроде `Gigabyte AMD Radeon 32GB`, `Intel 2GB`,
`AMD Radeon RX 470/480/570/570X/580/580X/590`, `Intel BMG G31` и `Intel BMG G21`
оставлены в собственных alias-карточках/папках без выдуманного SKU. `AMD Radeon
64GB` и `AMD Strix Halo [Radeon 8050S 8060S]` привязаны к 8060S по записанному
Ryzen AI MAX+ 395; RPL-S и Lunar Lake aliases сопоставлены по host CPU и
помечены. Board-partner labels, которые надёжно сводятся к существующей модели,
сохранены дословно в строке результата, но не считаются новыми устройствами.

Новые или более конкретные PTS-прогоны, отсутствующие локально как raw stdout:

| Устройство / точная PTS-строка | Результат | Hashcat | Что подтверждается |
|---|---|---:|---|
| AMD Radeon RX 9060 XT 16GB | [2607118-NE-20260711925](https://openbenchmarking.org/result/2607118-NE-20260711925) | 7.1.2 | 12 режимов; MD5 25.523 GH/s, SHA1 12.0233 GH/s, SHA-256 5.15777 GH/s, SHA-512 1.33383 GH/s; отдельная PTS-карточка находится в папке этой модели |
| Gigabyte AMD Radeon RX 5700 8GB | [2604244-NE-NORMAL87152](https://openbenchmarking.org/result/2604244-NE-NORMAL87152) | 7.1.2 | 12 режимов; точное board-partner имя и повторы сохранены в PTS-карточке этой модели |
| NVIDIA GeForce RTX 5090 Laptop GPU + Intel 24GB | [2607028-NE-WINDOWS1195](https://openbenchmarking.org/result/2607028-NE-WINDOWS1195) | 7.1.2 | 12 режимов, но PTS указывает комбинированную graphics-строку; скорость нельзя уверенно отделить от Intel device |
| MSI NVIDIA GeForce RTX 4070 Laptop GPU 8GB | [2604161-NE-HASHTESTT88](https://openbenchmarking.org/result/2604161-NE-HASHTESTT88) | 7.1.2 | SHA-512 (mode 1700) 1.71937 GH/s; PTS JSON содержит три повтора, raw stdout не приложен |
| AMD Radeon PRO W7600/W7700/W7900; Intel Arc Pro B50; RTX PRO Blackwell series; AMD AI PRO R9700 | [2605138-PTS-NVIDIART24](https://openbenchmarking.org/result/2605138-PTS-NVIDIART24), [2605219-PTS-RTXPRO1304](https://openbenchmarking.org/result/2605219-PTS-RTXPRO1304) | 7.1.2 | Многосистемные PTS comparisons; точные строки устройств и повторы находятся в PTS-карточках моделей |
| Intel Arc Pro B70 | [2604083-NE-INTELARCP47](https://openbenchmarking.org/result/2604083-NE-INTELARCP47), [2605125-PTS-SCALING616](https://openbenchmarking.org/result/2605125-PTS-SCALING616) | 7.1.2 | 92 строки PTS JSON: сравнение с Arc A770/B580/Pro B50 и масштабирование 1×–4×; отдельная частичная карточка в [`GPU/Intel Arc Pro B70/`](GPU/Intel%20Arc%20Pro%20B70/) |
| AMD Radeon AI PRO R9700 | [2608162](https://openbenchmarking.org/result/2608162-NE-HASHCATSH47), [2608164](https://openbenchmarking.org/result/2608164-NE-HASHCATSH76), [2608169 7-Zip](https://openbenchmarking.org/result/2608169-NE-HASHCAT7Z12), [2608169 Kerberos](https://openbenchmarking.org/result/2608169-NE-HASHCATKE77) | 7.1.2 | `system/hashcat` profile: 4 отдельных режима; PTS JSON repeats, без raw stdout |
| ASUS NVIDIA GeForce RTX 3090 24GB | [2609012-NE-LOCALRIGV86](https://openbenchmarking.org/result/2609012-NE-LOCALRIGV86) | 7.1.2 | `system/hashcat` profile: 8 успешных режимов; CPU-хост в этом GPU-профиле не считается CPU-тестом |

### Агрегаты OpenBenchmarking без выделенного stdout

Одна страница MD5-агрегатов содержит следующие новые GPU-кандидаты:

| GPU | Средний MD5 | Число результатов |
|---|---:|---:|
| AMD Radeon RX 7900 GRE | 51.301 GH/s | 7 |
| AMD Radeon RX 7800 XT | 40.731 GH/s | 8 |
| AMD Radeon RX 7700 XT | 39.708 GH/s | 6 |
| AMD Radeon RX 7600 XT | 23.898 GH/s | 7 |
| AMD Radeon RX 7600 | 22.031 GH/s | 6 |
| AMD Radeon Vega 8 | 2.575 GH/s | 3 |
| AMD Radeon PRO W7600 | 21.318 GH/s | 3 |
| AMD Radeon PRO W7500 | 13.436 GH/s | 3 |
| NVIDIA RTX A1000 | 12.974 GH/s | 7 |
| NVIDIA RTX A400 | 5.201 GH/s | 3 |
| NVIDIA T400 | 4.187 GH/s | 3 |
| NVIDIA TU117GL (product alias not resolved) | 4.283 GH/s | 6 |

Также есть сводки для AMD Radeon 8060S (Hashcat 7.0 MD5 31.494 GH/s и SHA-256
5.404 GH/s, по 4 результата), Radeon PRO W7700 (MD5 30.5 GH/s, 3 результата),
Intel Arc A750, RTX 4000 Ada и других устройств. Страницы: [MD5](https://openbenchmarking.org/performance/test/pts/hashcat/8b64c180eac0ce4c97f0d73d774dbb6161bedb5f), [Hashcat 7.0 MD5](https://openbenchmarking.org/performance/test/pts/hashcat/7b7b45c3848e0a5482fb82f220518d5233961430).
RTX A1000/A400/T400/TU117GL и Radeon PRO W7500/W7600 значения взяты с [профиля Hashcat 6.2.4 MD5](https://openbenchmarking.org/performance/test/pts/hashcat/8b64c180eac0ce4c97f0d73d774dbb6161bedb5f); результаты SHA-512 для тех же строк есть на [профиле 6.2.4 SHA-512](https://openbenchmarking.org/performance/test/pts/hashcat/5ed72b49492c93ebaea7b21a1a301f6ab7c80661). `TU117GL` оставлен как неразрешённое имя устройства и не склеивается с T400/A400 без подтверждения модели.

## PHCS GPU comparison

В [PHCS-gh/Hashcat-benchmark](https://github.com/PHCS-gh/Hashcat-benchmark/)
есть общая таблица MD5; полный файл опубликован не для каждой строки.
Проверенные здесь устройства, которых нет под отдельным именем в локальном
каталоге raw-прогонов:

| Модель | Публичная сводная цифра | Статус |
|--------|------------------------:|--------|
| AMD Radeon RX 470 4GB | MD5 10.7 GH/s | Только строка comparison table |
| AMD Radeon RX 560 XT 8GB | MD5 8219.9 MH/s | Только строка comparison table |
| AMD Radeon RX 7800 XT 16GB | MD5 42.1 GH/s; Hashcat 6.2.6, `-O`, OpenCL AMD-APP 3617.0 | Comparison row, отдельный raw-файл не опубликован |
| NVIDIA GeForce RTX 3050 Ti Laptop 4GB | MD5 16.8 GH/s | Только строка comparison table |
| NVIDIA RTX PRO 6000 Blackwell Server Edition | MD5 200.9 GH/s | Только строка comparison table |

RX 580 2048SP имеет отдельный опубликованный raw-файл и уже занесена в [`GPU/`](GPU).

Все 99 строк PHCS (96 GPU-строк собраны в 93 карточки с учётом вариантов
памяти/дубликатов и 3 CPU) разложены в отдельные `PHCS comparison summary.md`
внутри папок устройств. В карточках сохранены
варианты памяти, опубликованная MD5-скорость, hashcat/driver/runtime при их
наличии и прямая ссылка на README. 13 опубликованных raw-файлов дополнительно
связаны из карточек; где локальная raw-карточка существует, она остаётся
отдельным документом. Строки без raw остаются comparison-only и не входят в
основной ranking как сопоставимый полный `hashcat -b`.

## GPU: опубликованная таблица Tesla P4 (partial, не raw stdout)

В [README проекта justinhimself/hashcat-nvopencl](https://hub.docker.com/r/justinhimself/hashcat-nvopencl)
есть измерения **NVIDIA Tesla P4** на Hashcat v6.2.6 для 25 режимов в двух
runtime (OpenCL 3.0 и CUDA 12.9.40). Источник описывает дефолтные настройки
оптимизации и приводит результаты по отдельным режимам, но не прикладывает
консольный stdout или повторы. Поэтому в [карточке P4](GPU/NVIDIA%20Tesla%20P4)
сохранена таблица как **partial published values**, не как raw benchmark.

Примеры из таблицы: MD5 15.3392/15.1675 GH/s, NTLM 23.9864/26.1730 GH/s,
SHA2-256 1.8636/1.9161 GH/s, SHA2-512 561.7/647.1 MH/s. Оба значения в паре —
разные runtime одного Tesla P4, их нельзя складывать. Все 25 пар сохранены в
локальной карточке.

## OpenBenchmarking / Phoronix Hashcat

[Профиль Hashcat](https://openbenchmarking.org/test/pts/hashcat) собирает публичные
загрузки результатов по версиям и режимам. Это graphics test; информация о CPU
в system-results может описывать хост, а не устройство, которому принадлежит
измеренная скорость. Не переносить такие показатели в CPU-коллекцию без
подтверждённого CPU device/result.

В просмотренных агрегатах обнаружены отсутствующие в GPU-каталоге модели:

- Radeon RX 7600, RX 7600 XT, RX 7700 XT, RX 7800 XT, RX 7900 GRE;
- Radeon RX 9070 GRE, RX 9070;
- Radeon Pro W7500, W7600, W7700, W7900;
- Radeon Vega 8, Radeon 8060S, Radeon AI PRO R9700.

Примеры публикаций: [Hashcat 6.2.4 SHA-512](https://openbenchmarking.org/performance/test/pts/hashcat/5ed72b49492c93ebaea7b21a1a301f6ab7c80661)
и [Hashcat 7.1.2 MD5](https://openbenchmarking.org/performance/test/pts/hashcat/2f1e49c858bdaf551168a2c36422c3bcd6dbf083).
Отображаемые средние/число результатов являются агрегатами, не исходными
логами одного устройства.

### Новые модели из среза Hashcat 7.1.2 (данные по 1 октября 2026)

Проверка актуального профиля Hashcat 7.1.2 на OpenBenchmarking выявила ещё
несколько GPU, которых пока нет отдельными папками `GPU/`. Это **агрегаты
отдельных публичных загрузок**, а не raw stdout; количество означает число
совместимых публичных результатов на странице выбранного режима.

| GPU | MD5, среднее (число результатов) | SHA-256, среднее (число результатов) | SHA-512, среднее (число результатов) |
|---|---:|---:|---:|
| AMD Radeon AI PRO R9700 | 47.35172 GH/s (5) | — | — |
| AMD Radeon RX 9070 GRE | 35.33807 GH/s (3) | 7.0055 GH/s (3) | 1.7948 GH/s (3) |
| NVIDIA RTX A1000 | 12.949 GH/s (4) | 1.823 GH/s (5) | 615.2 MH/s (3) |
| NVIDIA RTX PRO 6000 Blackwell Workstation Edition | — | 32.54382 GH/s (7) | 10.70873 GH/s (7) |
| NVIDIA RTX PRO 6000 Blackwell Max-Q Workstation Edition | 177.915 GH/s (4) | 23.56658 GH/s (7) | 7.58809 GH/s (7) |
| NVIDIA RTX PRO 5000 Blackwell | — | 16.71968 GH/s (6) | 5.74844 GH/s (6) |
| NVIDIA RTX PRO 4500 Blackwell | — | 12.66898 GH/s (8) | 4.27514 GH/s (8) |
| NVIDIA RTX PRO 4000 Blackwell | — | 9.50255 GH/s (6) | 3.13557 GH/s (6) |
| NVIDIA RTX PRO 2000 Blackwell | — | 4.77931 GH/s (5) | 1.60714 GH/s (5) |

Источники режимов: [Hashcat 7.1.2 MD5](https://openbenchmarking.org/performance/test/pts/hashcat/2f1e49c858bdaf551168a2c36422c3bcd6dbf083),
[SHA-256](https://openbenchmarking.org/performance/test/pts/hashcat/bb70ab4002871eaf41c4c257184d478de05cb604)
и [SHA-512](https://openbenchmarking.org/performance/test/pts/hashcat/ec680f525d7a44fb1c765bf8f3508874a039743e).
Для RTX A1000 по тем же срезам опубликованы 4 MD5, 5 SHA-256 и 3 SHA-512 результата; точные значения приведены в строке таблицы выше.
AMD 8060S и Intel B70 тоже есть в актуальных PTS-результатах, но уже перечислены
выше в этом файле. Системный CPU в этих GPU-профилях не считается тестированным
CPU: страница профиля обозначает данный набор как graphics test.

**Неоднозначное имя:** `RX 7900 XT/7900 XTX/7900M` встречается в [публичном
результате](https://openbenchmarking.org/result/2404244-NE-HASHCATTE65), но alias
не позволяет уверенно приписать скорость именно RX 7900M.

**Неоднозначный V100 32GB:** [таблица HPC NTNU](https://www.hpc.ntnu.no/idun/documentation/running-jobs/)
публикует Hashcat MD5 для «V100» (50.663 GH/s), но одновременно указывает, что
их V100-парк включает варианты 16 GB и 32 GB, не связывая этот замер с конкретной
памятью. Поэтому это не подтверждение именно Tesla V100 32GB; точная модель
остаётся открытым пробелом в [`COVERAGE.md`](COVERAGE.md).

### Карточки PTS по моделям GPU

Профильные агрегаты и индивидуальные PTS-результаты перенесены в отдельные
Markdown-файлы внутри папок GPU. В каждом агрегатном файле сохранены точное имя
устройства PTS, версия Hashcat, режим/метрика, среднее значение H/s, число
публичных результатов, разброс (если опубликован) и ссылка на профиль. В
индивидуальных файлах сохранены PTS-повторы, когда они есть. Исходный stdout
Hashcat PTS не предоставляет; эти карточки помечены как aggregate/partial и не
выдаются за RAW. Неразрешённые device aliases остаются в карточках с точным
именем PTS, а не приписываются произвольной retail-модели.

## CPU: официальный Hashcat Argon2 report, не `hashcat -b`

В [release notes Hashcat v7.0.0](https://github.com/hashcat/hashcat/blob/master/docs/releases_notes_v7.0.0.md)
приведены тесты CPU для двух дополнительных моделей:

| CPU | NTLM mode 1000 | Mode 34000 (Argon2id) | Mode 70000 (Assimilation Bridge Argon2id) | Python Bridge SHA-256, 28 threads | Тип результата |
|-----|--------------:|----------------------:|-----------------------------------------:|---------------------------------:|----------------|
| Intel Core i7-14700K | — | 96 H/s | 110 H/s | 16 → 611 kH/s (before → v8.0.0) | Официальные обработанные отчёты Hashcat |
| AMD Ryzen 9 9900X | >10 GH/s | 92 H/s | 109 H/s | — | Официальные обработанные отчёты Hashcat |

Hashcat описывает связанные с отчётом тесты как выполненные собственной
утилитой `benchmark_deep.pl` через одиночные cracking-сессии (`-O -a 3`), а не
через `hashcat -b`. Для двух моделей теперь заведены отдельные частичные карточки:
[Core i7-14700K](<CPU/Intel/Core i7/Intel Core i7-14700K/Intel Core i7-14700K — Hashcat v7.0.0 official Argon2 report partial.md>) и [его Python Bridge результат v8.0.0](<CPU/Intel/Core i7/Intel Core i7-14700K/Intel Core i7-14700K — Hashcat v8.0.0 Python Bridge SHA-256 partial.md>), а также
[Ryzen 9 9900X](<CPU/AMD/Ryzen 9/AMD Ryzen 9 9900X/AMD Ryzen 9 9900X — Hashcat v7.0.0 official Argon2 report partial.md>).
Они учитываются в CPU-каталоге как обработанный официальный отчёт, но не включены
в сравнительную таблицу стандартных `hashcat -b` режимов.

## CPU: PHCS comparison rows (summary only)

В [PHCS Hashcat comparison](https://github.com/PHCS-gh/Hashcat-benchmark/)
опубликованы три CPU-строки без локального индивидуального stdout:

| CPU | Hashcat version | Published value | Classification |
|---|---|---:|---|
| AMD EPYC 9754 | 6.2.6 | MD5 28.0 GH/s | PHCS comparison row; no local raw log |
| AMD Ryzen Threadripper 3990X | 7.1.2 | MD5 8922.5 MH/s | PHCS comparison row; no local raw log |
| Intel Xeon E3-1270 v5 | 7.1.2 | MD5 550.6 MH/s | PHCS comparison row; no local raw log |

Полные per-device карточки с ограничениями лежат в `CPU/`; эти данные не
выдаются за raw и не смешиваются с основным ranking.

Полные per-device карточки с ограничениями лежат в `CPU/`; эти данные не
выдаются за raw и не смешиваются с основным ranking.

## CPU: community WPA22000 comparison (unverified summary)

В публичном [Gist GermanAizek](https://gist.github.com/GermanAizek/c3b54e8c41def7cda33efc70913580b2)
содержится сравнительная таблица mode 22000 по CPU. Все 228 строк разобраны в
227 per-device `.md`-карточек (повтор Core M-5Y10c с тем же значением
дедуплицирован).
Таблица не сопровождается исходными логами, описанием процедуры или единообразно
указанными версиями Hashcat, поэтому значения — leads для поиска, а не
подтверждённые raw-бенчмарки. Полный индекс скоростей и ссылок — в [`CPU.md`](CPU.md);
каждая карточка указывает неизвестные параметры и отсутствие stdout.

