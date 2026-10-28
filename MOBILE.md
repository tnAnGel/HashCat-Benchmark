# 💻 Реестр мобильных (laptop / mobile) GPU — покрытие бенчмарками

Трекер того, какие **мобильные** GPU **уже есть** в коллекции (✅) и какие ещё
предстоит найти (⬜). Отмечаем только карты, для которых реально может
существовать публичный вывод `hashcat -b`. Apple Silicon вынесен отдельно
(см. COVERAGE.md) и здесь не дублируется.

Легенда: ✅ есть полный/достаточный исходный прогон · ⚠️ есть только частичный/legacy фрагмент · ⬜ ищем · 🔒 вряд ли существует публичный бенчмарк

---

## NVIDIA GeForce RTX — Laptop

### Blackwell (RTX 50 Laptop)
- ⬜ RTX 5050 Laptop · ⬜ RTX 5060 Laptop · ⬜ RTX 5070 Laptop
- ⬜ RTX 5070 Ti Laptop · ⬜ RTX 5080 Laptop · ⬜ RTX 5090 Laptop

### Ada Lovelace (RTX 40 Laptop)
- ✅ RTX 4050 Laptop · ⚠️ RTX 4060 Laptop (только NTLM + отдельный WPA mode) · ⬜ RTX 4070 Laptop
- ⬜ RTX 4080 Laptop · ⬜ RTX 4090 Laptop

### Ampere (RTX 30 Laptop)
- ✅ RTX 3050 Laptop · ⚠️ RTX 3050 Ti Laptop · ✅ RTX 3060 Laptop
- ✅ RTX 3070 Laptop · ⬜ RTX 3070 Ti Laptop · ✅ RTX 3080 Laptop · ⬜ RTX 3080 Ti Laptop

### Turing (RTX 20 Mobile + Max-Q)
- ⬜ RTX 2050 Mobile · ✅ RTX 2060 Mobile / Max-Q · ⚠️ RTX 2070 Super Max-Q (3 режима)
- ⬜ RTX 2080 Mobile / Max-Q

## NVIDIA GeForce GTX — Mobile

### Turing (GTX 16 Mobile)
- ⬜ GTX 1650 Mobile · ✅ GTX 1650 Ti (mobile-only) · ⬜ GTX 1660 Ti Mobile

### Pascal (GTX 10 Mobile)
- ✅ GTX 1050 Laptop · ⚠️ GTX 1050 Ti Laptop · ⬜ GTX 1050 3GB Laptop
- ✅ GTX 1060 Mobile (Max-Q) · ⬜ GTX 1060 Laptop
- ⬜ GTX 1070 Laptop · ⚠️ GTX 1070 Max-Q · ⬜ GTX 1080 Laptop / Max-Q

Подтверждённые записи: [GTX 1050 Laptop](<GPU/NVIDIA GeForce GTX 1050/NVIDIA GeForce GTX 1050 — kennwhite v5.1.0 [Laptop GTX 1050].md>) и [GTX 1060 Max-Q](<GPU/NVIDIA GeForce GTX 1060 with Max-Q Design/NVIDIA GeForce GTX 1060 with Max-Q Design — kevtheskin (hashcat forum).md>). Для GTX 1050 Ti Laptop есть частичный benchmark; для GTX 1070 Max-Q — только runtime-скорость LUKS. Отдельные варианты 1050 3GB, 1060 Laptop, 1070 Laptop и 1080 Laptop/Max-Q пока не подтверждены источниками hashcat. Подробности лежат в папках соответствующих моделей под `GPU/`.

Новые архивные находки для старых мобильных Kepler GPU: [GT 650M](<GPU/NVIDIA GeForce GT 650M/NVIDIA GeForce GT 650M — Hashcat Forum v3.10 partial.md>) — одна пригодная WPA/WPA2-строка в прерванном выводе; [GTX 660M](<GPU/NVIDIA GeForce GTX 660M/NVIDIA GeForce GTX 660M — Hashcat Forum oclHashcat v2.01 partial.md>) — много режимов, CPU пропущен, лог оборван на аварии; [GTX 765M](<GPU/NVIDIA GeForce GTX 765M/NVIDIA GeForce GTX 765M — Hashcat Forum cudaHashcat-lite v0.15 partial.md>) — частичный benchmark с лимитом времени; [GTX 780M](<GPU/NVIDIA GeForce GTX 780M/NVIDIA GeForce GTX 780M — Hashcat Forum partial.md>) — старый multi-mode вывод без указанной версии.

Дополнительный поиск по [PHCS-gh](https://github.com/PHCS-gh/Hashcat-benchmark) нашёл отдельные MD5-сравнения, но не полные выводы `hashcat -b`: RTX 3050 Ti Laptop — 16.8 GH/s (6.2.6), RTX 2070 SUPER Max-Q Laptop — 25.0 GH/s (6.2.5), RTX 3060 Laptop — 25.0 GH/s, RTX 3070 Laptop — 31.9 GH/s, RTX 4050 Laptop — 8.28 GH/s и RTX 4060 Laptop — 25.3 GH/s. Каждое значение перенесено в `PHCS comparison summary.md` папки соответствующей модели и помечено как summary-only; это не raw.

### Maxwell (GTX 900M)
- ⬜ GTX 950M · ✅ GTX 960M · ⬜ GTX 965M · ✅ GTX 970M · ⬜ GTX 980M
- ⬜ GTX 980 (Notebook) — [benchmark GTX 980](<GPU/NVIDIA GeForce GTX 980/NVIDIA GeForce GTX 980 — soxrok2212 v6.2.3.md>) найден, но источник не подтверждает ноутбучную конфигурацию; [обзор мобильной GTX 980](https://gamersnexus.net/hwreviews/2142-gt72-dominator-pro-gtx-980-notebook-benchmarked) не содержит hashcat-теста

Подтверждённые записи: [GTX 960M](<GPU/NVIDIA GeForce GTX 960M/NVIDIA GeForce GTX 960M — kennwhite v5.1.0.md>) и [GTX 970M](<GPU/NVIDIA GeForce GTX 970M/NVIDIA GeForce GTX 970M — public source.md>). Для GTX 950M, 965M и 980M найдены только обнаружение устройства/незавершённый запуск в hashcat и значения из стороннего Hashcat-ng; последние не считаются стандартным `hashcat -b`. См. [GTX 950M](<GPU/NVIDIA GeForce GTX 950M/NVIDIA GeForce GTX 950M — public source.md>), [GTX 965M](<GPU/NVIDIA GeForce GTX 965M/NVIDIA GeForce GTX 965M — public source.md>) и [GTX 980M](<GPU/NVIDIA GeForce GTX 980M/NVIDIA GeForce GTX 980M — public source.md>).

## NVIDIA Workstation Mobile (Quadro / RTX A / RTX Ada Laptop)

### RTX A (Ampere Laptop)
- ⬜ RTX A1000 Laptop · ✅ RTX A2000 Laptop · ⬜ RTX A3000 Laptop
- ⬜ RTX A4000 Laptop · ⬜ RTX A5000 Laptop · ⬜ RTX A5500 Laptop

### Quadro RTX (Turing Mobile)
- ⬜ Quadro RTX 3000 Mobile · ⬜ Quadro RTX 4000 Mobile · ⬜ Quadro RTX 5000 Mobile
- ✅ **Quadro T2000** (mobile-only, Turing) · ⬜ Quadro T1000 · ⬜ Quadro T500

### Quadro Pascal / Maxwell Mobile
- ✅ **Quadro M1200** (mobile-only, Maxwell) · ⬜ Quadro M2200 · ⬜ Quadro P1000 Mobile
- ✅ Quadro P2000 Mobile · ⬜ Quadro P3200/P4200/P5200

### RTX Ada (Ada Laptop)
- ⬜ RTX 2000 Ada Laptop · ⬜ RTX 3000 Ada Laptop · ⬜ RTX 3500 Ada Laptop · ⬜ RTX 5000 Ada Laptop

---

## AMD Radeon RX — Mobile

### RDNA 3 (RX 7000M / S)
- ⬜ RX 7900M · ⬜ RX 7800M · ⬜ RX 7700S · ⬜ RX 7600M XT · ⬜ RX 7600S

### RDNA 2 (RX 6000M)
- ⬜ RX 6850M XT · ✅ RX 6800M · ⬜ RX 6700M · ⬜ RX 6600M · ⬜ RX 6500M

### RDNA / прочие
- ⬜ RX 5600M · ⬜ RX 5500M · ⬜ Radeon RX Vega M (Kaby Lake-G)

### AMD мобильные iGPU (APU)
- ✅ **Radeon 760M** (RDNA 3, Phoenix; ThinkPad P14s Gen 5) — полный `-b -w 3` + отдельный WPA `-O`
- ⚠️ **Radeon 780M** — шесть опубликованных режимов, частичный прогон; см. [`GPU/AMD Radeon 780M Graphics/`](<GPU/AMD Radeon 780M Graphics>)
- ⬜ Radeon 880M / 890M (Strix Point) · ⬜ Vega 8 / Vega 11 mobile

---

## Intel — Mobile / iGPU

### Arc A (Alchemist Mobile, dGPU)
- ✅ Arc A770M (additional ZerNox raw partial, 9 modes) · ⬜ Arc A730M · ⬜ Arc A570M · ⬜ Arc A550M · ⬜ Arc A370M · ⬜ Arc A350M

### Arc iGPU (Lunar Lake / Meteor Lake)
- ⚠️ Arc 140V (есть запуск, self-test errors) · ⬜ Arc 130V · ⬜ Arc iGPU (Meteor Lake, Ultra 7 155H и т.п.)
- ⚠️ Iris Xe Raptor Lake-P (one MD5 mode, partial raw) · ⬜ Iris Xe Tiger Lake (other configs not yet matched)

---

---

## Встраиваемые / портативные (handheld / SBC / ARM)

Не «ноутбучные» в классическом смысле, но мобильные/встраиваемые GPU — по просьбе.
- ✅ **Valve Steam Deck** — AMD Custom GPU 0932 (Van Gogh RDNA2), Paradice, hashcat forum
- ✅ **NVIDIA Jetson Nano** — Tegra X1 (Maxwell), Chick3nman, v5.1.0-beta
- ✅ **Nintendo Switch (Linux 4 Tegra)** — NVIDIA Tegra X1, Chick3nman, v6.2.6 (`--benchmark-all`; отдельная raw-карточка в папке Tegra X1)
- ✅ **NVIDIA Jetson AGX Xavier** — lepido, hashcat forum tid 8355 (неполный вывод: 6 режимов, `nvpmodel -m 0` / 30 Вт)
- ✅ **NVIDIA Jetson Xavier NX** — brianhealey, gist (`--benchmark-all`, MODE_15W_6CORE)
- ✅ **NVIDIA Jetson AGX Orin** — Shatatel, gist
- ⬜ Jetson TX2 · ⬜ Jetson Orin Nano / NX
- 🔒 Snapdragon 865 — на форуме (tid 11571) есть вывод, но он получен на **CPU** (pthread/OpenCL), а не на GPU Adreno — не GPU-бенчмарк

---

## Уже в коллекции (мобильные / портативные)
- ✅ **NVIDIA GeForce GTX 1050 Laptop** — kennwhite, v5.1.0 (`--benchmark-all`)
- ⚠️ **NVIDIA GeForce GTX 1050 Ti Laptop** — HP Omen, v4.0.1 beta (частичный benchmark)
- ⚠️ **NVIDIA GeForce GTX 1070 with Max-Q Design** — Reddit, v5.1.0 (частичный LUKS runtime, 103 H/s)
- ✅ **NVIDIA GeForce RTX 4050 Laptop GPU** — agrodude, v6.2.6 (прогон с `-w 1`)
- ✅ **NVIDIA GeForce RTX 3070 Laptop GPU** — PHCS-gh, v6.2.3
- ✅ **NVIDIA GeForce RTX 3060 Laptop GPU** — neeythann, v6.2.5
- ✅ **NVIDIA GeForce RTX 2060 Mobile** — whitefight18, v6.2.6
- ✅ **NVIDIA GeForce GTX 1650 Ti** (mobile-only) — whitefight18 (уже была в коллекции ранее)
- ✅ **NVIDIA GeForce GTX 1060 with Max-Q Design** — kevtheskin, hashcat forum
- ✅ **AMD Radeon RX 6800M** — chaos.exe, hashcat forum
- ✅ **Valve Steam Deck (AMD Custom GPU 0932)** — Paradice, hashcat forum
- ✅ **NVIDIA Jetson Nano (Tegra X1)** — Chick3nman, v5.1.0-beta
- ✅ **Nintendo Switch / Tegra X1 (L4T Linux)** — Chick3nman, v6.2.6 (`hashcat -b -O -w 4 --benchmark-all`)
- ✅ **Intel Arc A770M** — ConanChiles, v6.2.6
- ✅ **NVIDIA GeForce RTX 3050 Laptop GPU** — HexRx, v6.2.6
- ⚠️ **NVIDIA GeForce RTX 3050 Ti Laptop GPU** — PHCS comparison, MD5 16.8 GH/s; без локального raw stdout ([карточка](<GPU/NVIDIA GeForce RTX 3050 Ti Laptop GPU>))
- ✅ **NVIDIA RTX A2000 Laptop GPU** — shoeper, v6.2.5 (Device #2 в прогоне — CPU через PoCL)
- ✅ **NVIDIA Quadro T2000** — 9pii9, v6.2.6
- ✅ **NVIDIA Quadro M1200** — crypt0rr, v6.2.6-123 (`--workload-profile=4`)
- ✅ **NVIDIA Jetson AGX Orin** — Shatatel, v6.2.5-676
- ✅ **NVIDIA Jetson Xavier NX** — brianhealey, v6.1.1-71 (`--benchmark-all`, 15 Вт)
- ✅ **NVIDIA Jetson AGX Xavier** — lepido, v5.1.0-1397 (неполный вывод, 30 Вт)
- ✅ **AMD Radeon 760M Graphics** (iGPU ноутбука) — LaptopPWR, v6.2.6 (полный `-b -w 3` + отдельный `-m 2500` с `-O`)
</content>
</invoke>

---

## Заметки по поиску (глубокий проход)

- Раздел форума **Hardware (forum-13)** просмотрен по 56 страницам листингов / 1107 тредам,
  но позднее найдены старые отдельные архивные публикации, пропущенные первоначальным поиском:
  GT 650M (tid 6157), GTX 660M (post 28623), GTX 765M (tid 2617) и GTX 780M (tid 3169). Помимо них подтверждены
  RTX 4050 Laptop (tid 13412), GTX 1060 Max-Q, Tegra X1 / Xavier (tid 8355),
  Radeon 760M (tids 12463, 12466). Треды 8221 (RTX 2070 Mobile), 8579 (RTX 2080 Max-Q), 10741 (3080 Laptop),
  11704 (RTX 2060 vs 4060 Laptop) — сравнение не содержит полного stdout, но автор явно
  указывает строку `Speed.#1` mode 22000 как результат RTX 4060 Laptop; сохранено как
  дополнительный частичный источник в папке GPU.
- Вложения форума (`attachment.php`) требуют логина и недоступны.
- Мобильных GPU **не найдено** ни в одном подлинном выводе по: RTX 50 Laptop (5050–5090),
  RTX 4070/4080/4090 Laptop, RTX 3050 Ti / 3070 Ti / 3080 / 3080 Ti Laptop,
  RTX 2050/2070/2080 Mobile, GTX 1650/1660 Ti/1050/1050 Ti/1070/1080 Mobile, GTX 900M,
  RTX A1000/A3000/A4000/A5000/A5500 Laptop, Quadro RTX 3000/4000/5000 **Mobile**
  (найденные Quadro RTX 4000/5000 в чужих прогонах — десктопные, суффикса Mobile/Max-Q нет),
  RTX 2000–5000 Ada Laptop, RX 7900M/7800M/7700S/7600M XT/7600S, RX 6850M XT/6700M/6600M/6500M,
  RX 5600M/5500M, Vega M, Arc A730M/A570M/A550M/A370M/A350M, Arc iGPU (Meteor/Lunar Lake), Iris Xe.
