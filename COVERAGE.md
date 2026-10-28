# 📋 Реестр видеокарт — покрытие бенчмарками

Трекер того, какие GPU **уже есть** в коллекции (✅) и какие ещё предстоит
найти (⬜). Отмечаем только карты, для которых реально может существовать
публичный вывод `hashcat -b`. Ищем **постепенно, по батчам**.

**Текущее покрытие: 293 папки GPU с карточками** (539 Markdown-карточек; полный указатель — [`GPU.md`](GPU.md)).
Легенда: ✅ есть локальная raw-карточка · ⬜ ищем · ⚠️ частичный/неоднозначный либо только parsed PTS результат (без локального raw stdout) · 🔒 вряд ли существует публичный бенчмарк

Батчи в нижней части файла — исторические заметки; актуальные статусы выше отражают
текущее содержимое `GPU/` и более поздние результаты поиска.

---

## NVIDIA GeForce — Desktop

### Kepler (GTX 600/700)
- ⬜ GTX 650 / 650 Ti · ⚠️ GTX 660 (partial forum log) · ⚠️ GTX 660 Ti (legacy mode 7700) · ⬜ GTX 670 · ⬜ GTX 680 · ⚠️ GTX 690 (mixed rig)
- ⚠️ GTX 750 (legacy forum output) / ⬜ GTX 750 Ti · ⚠️ GTX 760 (legacy partial) · ⚠️ GTX 770 (legacy + forum run) · ⬜ GTX 780 · ⚠️ GTX 780 Ti (NTLM partial)
- ⬜ GTX TITAN · ⬜ TITAN Black · ⬜ TITAN Z

### Maxwell (GTX 900)
- ✅ GTX 950 · ✅ GTX 960 · ✅ GTX 970 · ✅ GTX 980 · ✅ GTX 980 Ti · ✅ GTX TITAN X

### Pascal (GTX 10)
- ✅ GT 1030 · ✅ GTX 1050 · ✅ GTX 1050 Ti · ✅ GTX 1060 3GB · ✅ GTX 1060 6GB
- ✅ GTX 1070 · ✅ GTX 1070 Ti · ✅ GTX 1080 · ✅ GTX 1080 Ti
- ⬜ TITAN X (Pascal) · ✅ TITAN Xp

### Turing (GTX 16)
- ⬜ GTX 1630 · ✅ GTX 1650 · ✅ GTX 1650 SUPER · ✅ GTX 1660 · ✅ GTX 1660 SUPER · ✅ GTX 1660 Ti

### Turing (RTX 20)
- ✅ RTX 2060 · ✅ RTX 2060 SUPER · ✅ RTX 2070 · ✅ RTX 2070 SUPER
- ✅ RTX 2080 · ✅ RTX 2080 SUPER · ✅ RTX 2080 Ti · ✅ TITAN RTX

### Ampere (RTX 30)
- ✅ RTX 3050 (6GB) · ✅ RTX 3060 · ✅ RTX 3060 Ti · ✅ RTX 3070 · ✅ RTX 3070 Ti
- ✅ RTX 3080 · ⬜ RTX 3080 12GB · ✅ RTX 3080 Ti · ✅ RTX 3090 · ✅ RTX 3090 Ti

### Ada Lovelace (RTX 40)
- ✅ RTX 4060 · ✅ RTX 4060 Ti · ✅ RTX 4070 · ✅ RTX 4070 SUPER
- ✅ RTX 4070 Ti · ✅ RTX 4070 Ti SUPER · ✅ RTX 4080 · ✅ RTX 4080 SUPER · ✅ RTX 4090 · ⚠️ RTX 4090 D (один режим)

### Blackwell (RTX 50)
- ⬜ RTX 5050 · ⬜ RTX 5060 · ✅ RTX 5060 Ti · ✅ RTX 5070 · ✅ RTX 5070 Ti · ✅ RTX 5080 · ✅ RTX 5090

## NVIDIA GeForce — Laptop
> Полный реестр мобильных GPU вынесен в [`MOBILE.md`](MOBILE.md).

- ✅ RTX 3070 Laptop · ✅ RTX 3060 Laptop · ✅ RTX 3080 Laptop
- ✅ RTX 4050 Laptop · ⚠️ RTX 4060 Laptop (частично) · ⚠️ RTX 4070 Laptop (PTS SHA-512 only) · ⬜ RTX 4080 / 4090 Laptop
- ✅ RTX 2060 Mobile · ⬜ RTX 2070/2080 Mobile · ✅ GTX 1060 Max-Q

## NVIDIA Workstation (Quadro / RTX A / RTX Ada)
- ✅ Quadro RTX 4000 · ⚠️ Quadro P5000 (PKZIP modes only) · ✅ RTX 5000 · ✅ RTX 6000 · ⬜ RTX 8000
- ✅ RTX A2000 · ✅ RTX A4000 · ⚠️ RTX A4500 (PTS only) · ✅ RTX A5000 · ✅ RTX A6000 · ⚠️ Quadro RTX 5000 Max-Q (PTS only) · ⚠️ Quadro P2000 desktop (PTS only; Mobile SKU is separate)
- ⚠️ RTX A1000 / RTX A400 / T400 / MX230 (PTS aggregates only; see [`PUBLIC-AGGREGATES.md`](PUBLIC-AGGREGATES.md))
- ⚠️ RTX 2000 Ada (PTS only) · ⚠️ RTX 4000 Ada (PTS only) · ⬜ RTX 5000 Ada · ✅ RTX 6000 Ada Generation
- ⚠️ RTX 2000 Ada Laptop (PTS only)
- ⚠️ RTX PRO 6000 Blackwell Workstation (2× raw partial + PTS) / ⚠️ Max-Q · ⚠️ RTX PRO 5000 / 4500 / 4000 / 2000 Blackwell (PTS aggregates)

## NVIDIA Data-center / Compute
- ⬜ Tesla K40 · ⚠️ GRID K520 (legacy partial) · ✅ Tesla K80 · ✅ Tesla M40 · ✅ Tesla M60 · ⚠️ Tesla M6 (PTS only) · ✅ Tesla P40 · ⚠️ Tesla P4 (published partial table) · ✅ Tesla P100 · ✅ GB10 (DGX Spark)
- ✅ Tesla T4 · ✅ Tesla V100 SXM2 16GB · ⬜ V100 32GB · ✅ V100 PCIe
- ✅ A100 PCIe 40GB · ✅ A100 80GB · ✅ A100 SXM4 40GB · ✅ A10 · ⬜ A16 · ⬜ A30 · ✅ A40 · ✅ A800 80GB
- ✅ H100 PCIe · ✅ H100 SXM · ✅ H200 · ✅ L4 · ✅ L40 · ✅ L40S
- ⬜ B100 · ✅ B200 · ✅ GH200 · ⬜ GB200

## NVIDIA Mining (CMP / P-series)
- ✅ P102-100 · ✅ P104-100 · ✅ P106-100
- ⬜ CMP 30HX · ⬜ CMP 40HX · ✅ CMP 50HX · ✅ CMP 70HX · ✅ CMP 90HX · ✅ CMP 170HX

---

## AMD Radeon — Desktop

### GCN (HD 7000 / R9 / Fury)
- ⚠️ HD 7970 (legacy partial, oclHashcat v1.01) · ⚠️ HD 6990 (legacy mode 7700, dual GPU) · ✅ R9 280X (legacy oclHashcat beta1) · ✅ R9 290 · ✅ R9 290X (legacy v1.21) · ⚠️ R9 390X (legacy selected modes)
- ⚠️ R9 270X (legacy partial) · ⬜ R9 Fury · ⬜ R9 Fury X · ⬜ R9 Nano · ⬜ R9 380 / 380X

### Polaris (RX 400 / 500)
- ✅ RX 460 · ⚠️ RX 470 (comparison table only) · ✅ RX 480 · ⬜ RX 550 · ⬜ RX 560 · ⚠️ RX 570 Series (one SHA1 mode, 3-device alias; exact SKU unresolved) · ✅ RX 580 · ✅ RX 580 2048SP (distinct SKU) · ✅ RX 590
- ⚠️ RX 560 XT (comparison table only)

### Vega
- ✅ RX Vega 56 · ✅ RX Vega 64 · ✅ Vega 64 Liquid · ✅ Radeon VII · ⚠️ Radeon Vega 8 (PTS aggregate only)
- ⚠️ Radeon RX Vega 10 · ⚠️ Radeon RX Vega 11 (partial modes)

### RDNA (RX 5000)
- ⚠️ RX 5500 XT (forum log; mode 0 warns about memory) · ✅ RX 5600 XT · ⬜ RX 5700 · ✅ RX 5700 XT

### RDNA 2 (RX 6000)
- ✅ RX 6400 · ⬜ RX 6500 XT · ✅ RX 6600 · ✅ RX 6600 XT · ✅ RX 6650 XT
- ✅ RX 6700 XT · ⬜ RX 6750 XT · ✅ RX 6800 · ✅ RX 6800 XT · ✅ RX 6900 XT · ✅ RX 6950 XT

### RDNA 3 (RX 7000)
- ⚠️ RX 7600 (PTS aggregate) · ⚠️ RX 7600 XT (PTS aggregate) · ⚠️ RX 7700 XT (PTS aggregate) · ⚠️ RX 7800 XT (PTS + individual result)
- ⚠️ RX 7900 GRE (PTS aggregate) · ✅ RX 7900 XT · ✅ RX 7900 XTX

### RDNA 4 (RX 9000)
- ⚠️ RX 9060 XT (individual PTS results) · ⚠️ RX 9070 (individual PTS result) · ⚠️ RX 9070 GRE (PTS aggregate) · ✅ RX 9070 XT

## AMD Workstation / Instinct
- ⬜ Radeon Pro W6800 · ⚠️ Pro W5700X (4 raw modes) · ⚠️ FirePro D700 (legacy partial) · ⚠️ Pro W6800X Duo (partial Mac Pro log) · ⚠️ Radeon Pro 580X (partial) · ✅ Pro WX 3200 · ✅ Pro 5500M · ✅ Pro 560 (mode 14800 only) · ⚠️ Pro Vega II (partial Mac Pro log) · ⬜ Radeon Pro W7800 · ⚠️ Radeon Pro W7500 / W7600 / W7700 / W7900 (PTS aggregates, no raw) · ⚠️ Radeon AI PRO R9700 (4 individual PTS modes; no raw stdout)
- ⚠️ Instinct MI50 (4×, backend alias MI60/MI50) · ⬜ MI100 · ⬜ MI210 · ⚠️ MI250/MI250X (8×, mode 1000 only; model variant ambiguous) · ✅ MI300X (raw + published rates, non-raw) · ⬜ MI300A
- ✅ Radeon 8060S (one raw MD5 mode; PTS results separately in [`PUBLIC-AGGREGATES.md`](PUBLIC-AGGREGATES.md)) · ⚠️ Radeon 680M (NTLM-only forum line) · ⚠️ Radeon (TM) 520 · ⚠️ Radeon HD 8250 (partial)

---

## Intel Arc
- ⚠️ Arc A310 (Hashcat-ng mode 22000 summary; non-upstream) · ⚠️ Arc A380 (PTS + Hashcat-ng summary; non-upstream) · ⚠️ Arc A580 (PTS only) · ⚠️ Arc A750 (PTS only) · ✅ Arc A770 (raw `-b` v6.2.6 + WPA source)
- ✅ Arc A770M (two raw sources; one partial) · ⚠️ Arc B570 (PTS only) · ✅ Arc B580
- ⚠️ Arc Pro B50 (individual PTS parsed result; not raw stdout) · ⚠️ Arc Pro B70 (PTS only) · ⚠️ Iris Xe Graphics (Tiger Lake-LP GT2; individual partial raw MD5)
- ⚠️ UHD Graphics 770 (forum excerpts) · ✅ UHD Graphics 630 · ✅ HD Graphics 630 · ✅ HD Graphics 4600 · ✅ UHD Graphics 620 · ⚠️ HD Graphics 4000 · ⚠️ HD Graphics 4400 · ⚠️ Iris Pro (partial outputs)
- ⚠️ Iris Xe TGL GT2 (individual partial raw + PTS aggregate) · ⚠️ Iris Xe RPL-P (one MD5 mode, partial raw) · ⚠️ Iris Xe ADL GT2 (PTS aggregate only)

---

## Apple Silicon
- ✅ M1 · ✅ M1 Pro · ✅ M1 Max · ✅ M1 Ultra
- ✅ M2 · ✅ M2 Pro · ✅ M2 Max · ✅ M2 Ultra
- ✅ M3 · ✅ M3 Pro · ✅ M3 Max · ⬜ M3 Ultra
- ✅ M4 · ✅ M4 Pro · ✅ M4 Max · ✅ M5 · ⚠️ M5 Max (one WPA mode from proprietary Hashcat-ng fork; not upstream-comparable)

---

## Портативные / встраиваемые
- ✅ Valve Steam Deck (AMD Custom GPU 0932) · ✅ NVIDIA Jetson Nano (Tegra X1)
- ✅ Jetson AGX Xavier · ✅ Jetson Orin · 🔒 Snapdragon 865 (публичный вывод — CPU, не Adreno)

---

## План поиска (по батчам)

Идём от самых востребованных (по ним чаще всего есть публичные прогоны) к
редким. Каждый батч — отдельный заход поиска; найденное сразу оформляется в
папки и попадает в сводную таблицу README.

1. **Батч 1 — популярные десктопные ✅ ВЫПОЛНЕН.** Найдено 10:
   RTX 2070/2070 S/2080 S, RTX 3090 Ti, RTX 4070 Ti, RTX 5070, GTX 980/1050,
   RX 590/6950 XT. Не нашли (нет реального сырого вывода): RTX 3050, RTX 5060,
   RX 7900 XTX, 7800 XT, 7700 XT, 7600, 6900 XT, 6650 XT, 6750 XT, 5700, 5600 XT,
   570, Intel Arc A770/A750/A380. RX 6800 — есть только «реконструированный»
   вывод из комментария к гисту, не взят (нужен подлинный).
2. **Батч 2 — data-center:** V100 32GB, A100 80GB, A40/A30/A10, H200, L40/L40S,
   Tesla P40/M60.
3. **Батч 3 — Apple Silicon ✅ ВЫПОЛНЕН.** Найдено 12: M1/M1 Pro/M1 Max/M1 Ultra,
   M2/M2 Pro/M2 Max/M2 Ultra, M3/M3 Pro, M4 Pro/M4 Max. Не нашли: M3 Ultra, базовый M4.
4. **Батч 4 — workstation/DC/AMD ✅ ВЫПОЛНЕН.** Найдено 3: RTX A2000, L40S, RX 6600.
   Остальное (RX 7900 XTX, 6900 XT, 7800/7700 XT, 7600, Arc A770/A750/A380, RTX 3050/5060,
   A4500, V100 32GB, A100 80GB и др.) — публичного сырого вывода `hashcat -b` не нашлось
   (нет на GitHub, либо только на заблокированных hashcat.net/geeks3d). Ждём, пока кто-то выложит.
5. **Батч 6 — повторный заход + мобильные ✅ ВЫПОЛНЕН.** Найдено 18 (98 → 116).
   Ключевое: **hashcat.net/forum оказался доступен** — 403 отдаётся только на
   WebFetch, обычный `curl` с User-Agent получает 200 (`printthread.php?tid=N`,
   листинги `forum-13-page-N.html`). Недоступны только вложения (`attachment.php`
   требует логина).
   - Десктоп/DC/workstation (11): RX 7900 XTX, RX 9070 XT, RX 6900 XT, RX 6650 XT,
     RX 5600 XT, RX 460, RTX A6000, L40, A10, Tesla T4, TITAN Xp.
   - Мобильные/портативные (7): RTX 4050 Laptop, RTX 3060 Laptop, RTX 2060 Mobile,
     GTX 1060 Max-Q, RX 6800M, Steam Deck, Jetson Nano. Реестр — [`MOBILE.md`](MOBILE.md).
   - Не нашлось: RDNA3 середина (7900 GRE, 7800/7700 XT, 7600), RX 9070/9060 XT,
     вся десктопная Intel Arc, RTX 3050/5050/5060/3080 12GB, A4500/Ada,
     H200/A100 80GB/A40/A30, MI300X/MI250X, Radeon Pro W7900, Apple M3 Ultra и M4.
6. **Батч 7 — рой из 40 агентов (285 целей) ✅ ВЫПОЛНЕН (исторический снимок до миграции папок).** Найдено 23 (132 → 155).
   Data-center/workstation: **H200, GH200, A100 80GB, Tesla M40, Tesla V100 PCIe,
   Quadro RTX 4000/5000/6000**. Десктоп/мобильные: **RX 480, RTX 3050 6GB,
   RTX 3080 Laptop, GTX 950, GTX 960M, GTX 860M, GT 1030, 940M, Vega 64 Liquid,
   Pro 5500M, Pro WX 3200, R9 M395X**. Intel **Arc A770** — только режим 22000.
   Много прогонов неполные/старого формата hashcat 3.x–5.x (помечено ⚠️ в README и
   в шапках файлов). Дубликат RTX 3050: gist был про 6GB-версию, папка базовой 8GB
   удалена, оставлена RTX 3050 6GB.
   - Не нашлось (публичного сырого вывода нет): RDNA3 середина (7800/7700 XT, 7600,
     7900 GRE, 7900M/7700S), RDNA4 (9070/9060 XT), Instinct MI50/MI100/MI210/MI250/MI300A,
     Radeon Pro W7800/W7900, RTX A4500, RTX 2000–5000 Ada, Quadro RTX 8000,
     Tesla K40, V100 32GB, A30/A16, B100/GB200, Apple M3 Ultra,
     Intel Arc A750/A580/A380/A310/A730M/A370M и большинство ноутбучных RTX.
