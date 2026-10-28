# 🗂️ Полный реестр мобильных GPU, 2010–2025

Максимально полный справочник **ноутбучных / мобильных / встраиваемых** GPU за
последние ~15 лет. Это **не** трекер найденных бенчмарков (для этого есть
[`MOBILE.md`](MOBILE.md) и [`COVERAGE.md`](COVERAGE.md)) — это **исходный список
целей**, по которому дальше будет идти поиск публичных выводов `hashcat -b`.

Названия приведены в **официальном виде производителя** (как их печатает
драйвер / как они значатся в TechPowerUp GPU Database и Notebookcheck) —
именно по этим строкам потом ищутся бенчмарки.

**Охват:** NVIDIA (Fermi → Blackwell + Tegra/Jetson) · AMD (TeraScale → RDNA 3.5
+ APU iGPU + Radeon Pro mobile) · Intel (Sandy Bridge iGPU → Arc Xe2).
**Apple Silicon здесь намеренно не дублируется** — см. раздел «Apple Silicon» в
[`COVERAGE.md`](COVERAGE.md).

### Легенда статуса
- ✅ — benchmark **уже есть** в коллекции (папка в корне репо)
- ⚠️ — найден частичный запуск/результат, полного benchmark пока нет
- ⬜ — **имеет смысл искать**: карта достаточно новая/мощная, современный
  hashcat её поддерживает, публичный прогон правдоподобен
- 🔒 — **бенчмарк маловероятен**: нет поддержки в актуальном hashcat/драйвере
  (CUDA CC < 5.0, OpenCL < 1.2), либо карта слишком слабая/нишевая, чтобы
  кто-то выкладывал прогон

### Легенда API / поддержки hashcat
| Метка | Что значит |
|---|---|
| `CUDA CC x.x` | вычислительная способность NVIDIA. **CC ≥ 5.0 (Maxwell)** — работает на современных CUDA 12.x. CC 2.x (Fermi) выпал из CUDA 9, CC 3.x (Kepler) — из CUDA 12. Для них нужен архивный драйвер + hashcat ≤ 6.x на OpenCL |
| `OpenCL` | универсальный бэкенд. hashcat требует **OpenCL 1.2+**. AMD TeraScale/старый GCN и Intel Gen7 практически не заводятся на актуальных сборках |
| `HIP` | ROCm-бэкенд AMD, только RDNA/GCN5 и новее, Linux |
| `Metal` | бэкенд hashcat 6.2.6+ для macOS (Apple + AMD Pro в маках) |
| `Level Zero / OpenCL NEO` | Intel Arc / Xe, современный стек |

---

# 🟩 NVIDIA

## GeForce — Fermi Mobile

### 400M (2010) · CUDA CC 2.1 · OpenCL 1.1 · 🔒 весь ряд
> Fermi выпал из CUDA начиная с 9.0, OpenCL остался на 1.1 — актуальный hashcat не стартует.

- 🔒 GeForce 405M · 🔒 GeForce 410M · 🔒 GeForce GT 415M · 🔒 GeForce GT 420M
- 🔒 GeForce GT 425M · 🔒 GeForce GT 435M · 🔒 GeForce GT 445M
- 🔒 GeForce GTX 460M · 🔒 GeForce GTX 470M · 🔒 GeForce GTX 480M · 🔒 GeForce GTX 485M

### 500M (2011) · CUDA CC 2.1 · OpenCL 1.1 · 🔒 весь ряд
- 🔒 GeForce 510M · 🔒 GeForce GT 520M · 🔒 GeForce GT 520MX · 🔒 GeForce GT 525M
- 🔒 GeForce GT 530M · 🔒 GeForce GT 540M · 🔒 GeForce GT 550M · 🔒 GeForce GT 555M
- 🔒 GeForce GTX 560M · 🔒 GeForce GTX 570M · 🔒 GeForce GTX 580M

## GeForce — Kepler Mobile

### 600M (2012) · CUDA CC 3.0 (часть — ребренды Fermi CC 2.1) · 🔒 весь ряд
> Kepler удалён из CUDA 12; hashcat 6.x на OpenCL теоретически заводится со старым драйвером,
> но публичных прогонов практически не существует.

- 🔒 GeForce 610M · 🔒 GeForce GT 620M · 🔒 GeForce GT 625M · 🔒 GeForce GT 630M
- 🔒 GeForce GT 635M · 🔒 GeForce GT 640M · 🔒 GeForce GT 640M LE · 🔒 GeForce GT 645M
- ⚠️ GeForce GT 650M (legacy forum partial) · ⚠️ GeForce GTX 660M (oclHashcat v2.01 partial) · 🔒 GeForce GTX 670M · 🔒 GeForce GTX 670MX
- 🔒 GeForce GTX 675M · 🔒 GeForce GTX 675MX · 🔒 GeForce GTX 680M · 🔒 GeForce GTX 680MX

### 700M (2013) · CUDA CC 3.0/3.5 · 🔒 весь ряд
- 🔒 GeForce 710M · 🔒 GeForce GT 720M · 🔒 GeForce GT 730M · 🔒 GeForce GT 735M
- 🔒 GeForce GT 740M · 🔒 GeForce GT 745M · 🔒 GeForce GT 750M · 🔒 GeForce GT 755M
- 🔒 GeForce GTX 760M · ⚠️ GeForce GTX 765M (legacy partial) · 🔒 GeForce GTX 770M · ⚠️ GeForce GTX 780M (legacy partial)

## GeForce — Maxwell Mobile

### 800M (2014) · смешанное поколение: GM107 (CC 5.0) + ребренды Kepler
- 🔒 GeForce GT 820M *(Fermi/Kepler ребренд)* · 🔒 GeForce 830M · 🔒 GeForce 840M
- 🔒 GeForce GTX 845M · ⬜ GeForce GTX 850M *(CC 5.0)* · ⬜ GeForce GTX 860M *(есть версии GM107 CC 5.0 и GK104 CC 3.0)*
- 🔒 GeForce GTX 870M *(Kepler GK104)* · 🔒 GeForce GTX 880M *(Kepler GK104)*

### 900M (2015) · CUDA CC 5.0/5.2 · OpenCL 1.2 · ⬜ поддерживается современным hashcat
- 🔒 GeForce 920M · 🔒 GeForce 920MX · 🔒 GeForce 930M · 🔒 GeForce 930MX
- 🔒 GeForce 940M · ⬜ GeForce 940MX · 🔒 GeForce 945M
- ⬜ GeForce GTX 950M · ✅ GeForce GTX 960M · ⬜ GeForce GTX 965M
- ✅ GeForce GTX 970M · ⬜ GeForce GTX 980M
- ⬜ GeForce GTX 980 (Notebook) *(десктопный GM204 в ноутбуке, без суффикса M)*

## GeForce — Pascal Mobile

### GTX 10 Mobile (2016–2017) · CUDA CC 6.1 · OpenCL 1.2 · полная поддержка
> С Pascal мобильные карты перестали получать суффикс «M» — драйвер печатает то же имя,
> что и у десктопа (кроме вариантов Max-Q).

- ✅ GeForce GTX 1050 (Laptop) · ⚠️ GeForce GTX 1050 Ti (Laptop) · ⬜ GeForce GTX 1050 3GB Laptop
- ✅ GeForce GTX 1060 with Max-Q Design · ⬜ GeForce GTX 1060 (Laptop)
- ⬜ GeForce GTX 1070 (Laptop) · ⚠️ GeForce GTX 1070 with Max-Q Design
- ⬜ GeForce GTX 1080 (Laptop) · ⬜ GeForce GTX 1080 with Max-Q Design

### MX-серия (2017–2022) · энергоэффективные дискретки для ультрабуков
| Модель | Год | Чип / архитектура | API | Статус |
|---|---|---|---|---|
| GeForce MX110 | 2017 | GM108, Maxwell | CUDA 5.0 | 🔒 |
| GeForce MX130 | 2017 | GM108, Maxwell | CUDA 5.0 | 🔒 |
| GeForce MX150 | 2017 | GP108, Pascal | CUDA 6.1 | ⬜ |
| GeForce MX230 | 2019 | GP108, Pascal | CUDA 6.1 | ⚠️ PTS-only |
| GeForce MX250 | 2019 | GP108, Pascal | CUDA 6.1 | ⬜ |
| GeForce MX330 | 2020 | GP108, Pascal | CUDA 6.1 | 🔒 |
| GeForce MX350 | 2020 | GP107, Pascal | CUDA 6.1 | ⬜ |
| GeForce MX450 | 2020 | TU117, Turing | CUDA 7.5 | ⬜ |
| GeForce MX550 | 2022 | TU117, Turing | CUDA 7.5 | ⬜ |
| GeForce MX570 / MX570 A | 2022 | GA107, Ampere | CUDA 8.6 | ⬜ |

### Quadro Pascal Mobile (2016–2018) · CUDA CC 6.1
- 🔒 Quadro P500 · 🔒 Quadro P520 · 🔒 Quadro P600 · 🔒 Quadro P620
- ⬜ Quadro P1000 · ✅ Quadro P2000 (Mobile) · ⬜ Quadro P3000 · ⬜ Quadro P4000 (Mobile)
- ⬜ Quadro P5000 (Mobile) · ⬜ Quadro P3200 · ⬜ Quadro P4200 · ⬜ Quadro P5200

## GeForce — Turing Mobile (2019–2020) · CUDA CC 7.5 · OpenCL 3.0 · полная поддержка

### GTX 16 Mobile
- ⬜ GeForce GTX 1650 (Laptop) · ⬜ GeForce GTX 1650 with Max-Q Design
- ✅ GeForce GTX 1650 Ti *(модель только мобильная)* · ⬜ GeForce GTX 1650 Ti with Max-Q Design
- ⬜ GeForce GTX 1660 Ti (Laptop) · ⬜ GeForce GTX 1660 Ti with Max-Q Design

### RTX 20 Mobile / Max-Q
- ✅ GeForce RTX 2060 Mobile · ⬜ GeForce RTX 2060 with Max-Q Design
- ⬜ GeForce RTX 2070 Mobile · ⬜ GeForce RTX 2070 with Max-Q Design
- ⬜ GeForce RTX 2070 SUPER Mobile · ⚠️ GeForce RTX 2070 SUPER with Max-Q Design
- ⬜ GeForce RTX 2080 Mobile · ⬜ GeForce RTX 2080 with Max-Q Design
- ⬜ GeForce RTX 2080 SUPER Mobile · ⬜ GeForce RTX 2080 SUPER with Max-Q Design
- ⬜ GeForce RTX 2050 Laptop GPU *(2022; вопреки названию — чип GA107, **Ampere** CC 8.6)*

### Quadro / T-серия Turing Mobile
- ⬜ Quadro RTX 3000 (Mobile) · ⬜ Quadro RTX 3000 with Max-Q Design
- ⬜ Quadro RTX 4000 (Mobile) · ⬜ Quadro RTX 5000 (Mobile)
- 🔒 Quadro T500 · 🔒 Quadro T550 · 🔒 Quadro T600 (Mobile)
- ⬜ Quadro T1000 (Mobile) · ⬜ Quadro T1200 Laptop GPU · ⬜ Quadro T2000 (Mobile)

## GeForce — Ampere Laptop (2021–2022) · CUDA CC 8.6 · OpenCL 3.0

- ⬜ GeForce RTX 3050 Laptop GPU · ⚠️ [GeForce RTX 3050 Ti Laptop GPU](<GPU/NVIDIA GeForce RTX 3050 Ti Laptop GPU>) · ⬜ GeForce RTX 3050 6GB Laptop GPU
- ✅ GeForce RTX 3060 Laptop GPU · ✅ GeForce RTX 3070 Laptop GPU · ⬜ GeForce RTX 3070 Ti Laptop GPU
- ✅ GeForce RTX 3080 Laptop GPU · ⬜ GeForce RTX 3080 Ti Laptop GPU

### RTX A — Ampere workstation laptop
- 🔒 RTX A500 Laptop GPU · ⬜ RTX A1000 Laptop GPU · ⬜ RTX A2000 Laptop GPU
- ⬜ RTX A3000 Laptop GPU · ⬜ RTX A4000 Laptop GPU · ⬜ RTX A5000 Laptop GPU
- ⬜ RTX A4500 Laptop GPU · ⬜ RTX A5500 Laptop GPU

## GeForce — Ada Lovelace Laptop (2023–2024) · CUDA CC 8.9 · OpenCL 3.0

- ✅ GeForce RTX 4050 Laptop GPU · ⚠️ GeForce RTX 4060 Laptop GPU (частично) · ⚠️ GeForce RTX 4070 Laptop GPU (PTS SHA-512 result only; see [`PUBLIC-AGGREGATES.md`](PUBLIC-AGGREGATES.md))
- ⬜ GeForce RTX 4080 Laptop GPU · ⬜ GeForce RTX 4090 Laptop GPU

### RTX Ada Generation Laptop (workstation)
- 🔒 RTX 500 Ada Generation Laptop GPU · ⬜ RTX 1000 Ada Generation Laptop GPU
- ⬜ RTX 2000 Ada Generation Laptop GPU · ⬜ RTX 3000 Ada Generation Laptop GPU
- ⬜ RTX 3500 Ada Generation Laptop GPU · ⬜ RTX 4000 Ada Generation Laptop GPU
- ⬜ RTX 5000 Ada Generation Laptop GPU

## GeForce — Blackwell Laptop (2025) · CUDA CC 12.0 · OpenCL 3.0

- ⬜ GeForce RTX 5050 Laptop GPU · ⬜ GeForce RTX 5060 Laptop GPU
- ⬜ GeForce RTX 5070 Laptop GPU · ⬜ GeForce RTX 5070 Ti Laptop GPU
- ⬜ GeForce RTX 5080 Laptop GPU · ⬜ GeForce RTX 5090 Laptop GPU

### RTX PRO Blackwell Generation Laptop (workstation, 2025)
- 🔒 RTX PRO 500 Blackwell Generation Laptop GPU · ⬜ RTX PRO 1000 Blackwell Generation Laptop GPU
- ⬜ RTX PRO 2000 Blackwell Generation Laptop GPU · ⬜ RTX PRO 3000 Blackwell Generation Laptop GPU
- ⬜ RTX PRO 4000 Blackwell Generation Laptop GPU · ⬜ RTX PRO 5000 Blackwell Generation Laptop GPU

## Tegra / Jetson — встраиваемые (2014–2025)

> Формально не ноутбучные, но это мобильный класс SoC. hashcat собирается под
> aarch64 + CUDA (JetPack), прогоны редки, но существуют.

| Платформа | GPU | Год | API | Статус |
|---|---|---|---|---|
| Jetson TK1 | Tegra K1 (Kepler, CC 3.2) | 2014 | CUDA | 🔒 |
| Jetson TX1 / Nano | Tegra X1 (Maxwell, CC 5.3) | 2015 / 2019 | CUDA | ✅ (Jetson Nano) |
| Jetson TX2 | Tegra X2 «Parker» (Pascal, CC 6.2) | 2017 | CUDA | ⬜ |
| Jetson AGX Xavier | Volta GPU (CC 7.2) | 2018 | CUDA | ⬜ |
| Jetson Xavier NX | Volta GPU (CC 7.2) | 2020 | CUDA | ⬜ |
| Jetson AGX Orin | Ampere GPU (CC 8.7) | 2022 | CUDA | ⬜ |
| Jetson Orin NX / Orin Nano | Ampere GPU (CC 8.7) | 2023 | CUDA | ⬜ |
| Jetson AGX Thor | Blackwell GPU | 2025 | CUDA | ⬜ |
| Nintendo Switch / Switch 2 | Tegra X1 / T239 | 2017 / 2025 | CUDA / — | ✅ Switch (Linux 4 Tegra, v6.2.6 raw); Switch 2 не проверен |

---

# 🟥 AMD

## Mobility Radeon — TeraScale (2010–2013) · 🔒 весь ряд
> TeraScale 2/3 — OpenCL 1.2 только на легаси-драйверах Catalyst; актуальный
> hashcat (6.x) их не запускает. Раздел для полноты картины.

### Mobility Radeon HD 5000M (2010, TeraScale 2)
- 🔒 HD 5145 · 🔒 HD 5165 · 🔒 HD 5430 · 🔒 HD 5450 · 🔒 HD 5470 · 🔒 HD 5490
- 🔒 HD 5650 · 🔒 HD 5730 · 🔒 HD 5750 · 🔒 HD 5770 · 🔒 HD 5850 · 🔒 HD 5870

### Radeon HD 6000M (2011, TeraScale 2)
- 🔒 HD 6230M · 🔒 HD 6250M · 🔒 HD 6290M · 🔒 HD 6310M · 🔒 HD 6330M
- 🔒 HD 6370M · 🔒 HD 6470M · 🔒 HD 6490M · 🔒 HD 6550M · 🔒 HD 6570M
- 🔒 HD 6630M · 🔒 HD 6650M · 🔒 HD 6730M · 🔒 HD 6750M · 🔒 HD 6770M
- 🔒 HD 6850M · 🔒 HD 6870M · 🔒 HD 6970M · 🔒 HD 6990M

### Radeon HD 7000M (2012, TeraScale 2/3 + первые GCN)
- 🔒 HD 7350M · 🔒 HD 7430M · 🔒 HD 7450M · 🔒 HD 7470M · 🔒 HD 7550M
- 🔒 HD 7570M · 🔒 HD 7590M · 🔒 HD 7610M · 🔒 HD 7650M · 🔒 HD 7670M
- 🔒 HD 7690M / 7690M XT · 🔒 HD 7730M · 🔒 HD 7750M · 🔒 HD 7770M
- 🔒 HD 7850M · 🔒 HD 7870M · 🔒 HD 7970M *(GCN 1.0 «Wimbledon»)*

### Radeon HD 8000M (2013, GCN 1.0 + ребренды)
- 🔒 HD 8530M · 🔒 HD 8550M · 🔒 HD 8570M · 🔒 HD 8590M · 🔒 HD 8650M
- 🔒 HD 8670M · 🔒 HD 8690M · 🔒 HD 8730M · 🔒 HD 8750M · 🔒 HD 8770M
- 🔒 HD 8790M · 🔒 HD 8850M · 🔒 HD 8870M · 🔒 HD 8970M

## Radeon R-серия Mobile (GCN, 2014–2017) · OpenCL 1.2/2.0 · 🔒 в основном
> GCN 1.0–1.2 выпали из ROCm и из современного amdgpu-pro. На старых сборках
> hashcat (≤ 5.x) заводились, но публичных мобильных прогонов почти нет.

### R200M (2014)
- 🔒 R5 M230 · 🔒 R5 M240 · 🔒 R5 M255 · 🔒 R7 M260 / M260X · 🔒 R7 M265
- 🔒 R7 M270 · 🔒 R7 M275 · 🔒 R9 M265X · 🔒 R9 M270X · 🔒 R9 M275X
- 🔒 R9 M280X · 🔒 R9 M290X · 🔒 R9 M295X *(iMac 5K / MSI)*

### R300M (2015)
- 🔒 R5 M315 · 🔒 R5 M320 · 🔒 R5 M330 · 🔒 R5 M335 · 🔒 R7 M340 · 🔒 R7 M350
- 🔒 R7 M360 · 🔒 R7 M365X · 🔒 R7 M370 · 🔒 R9 M375 / M375X · 🔒 R9 M380
- 🔒 R9 M385 / M385X · 🔒 R9 M390 / M390X · 🔒 R9 M395 / M395X

### R400M / Radeon 500 Mobile (2016–2017, Polaris)
- 🔒 R5 M420 · 🔒 R5 M430 · 🔒 R7 M440 · 🔒 R7 M445 · 🔒 R7 M460 · 🔒 R7 M465
- 🔒 R9 M470 / M470X · 🔒 R9 M485X
- 🔒 Radeon 520 · 🔒 Radeon 530 · 🔒 Radeon 535 · 🔒 Radeon 540 / 540X
- 🔒 Radeon 550 / 550X · ⬜ Radeon 560 / 560X · ⬜ Radeon 570X · ⬜ Radeon 580X
- ⬜ Radeon 610 / 620 / 625 *(ребренды, 2019)* · 🔒 Radeon 630 · 🔒 Radeon 640

## Polaris / Vega Mobile (2016–2019) · OpenCL 2.0 · ⬜ реалистично
- ⬜ Radeon RX 460 (Laptop) · ⬜ Radeon RX 470M · ⬜ Radeon RX 480M *(редкие OEM-варианты)*
- ⬜ Radeon RX 540 / 540X (Mobile) · ⬜ Radeon RX 550 / 550X (Mobile)
- ⬜ Radeon RX 560 / 560X (Mobile) · ⬜ Radeon RX 570 (Mobile) · ⬜ Radeon RX 580 (Mobile)
- ⬜ Radeon RX 640 (Mobile)
- ⬜ Radeon RX Vega M GL *(Kaby Lake-G, Intel NUC / Dell XPS 15 2-in-1)*
- ⬜ Radeon RX Vega M GH *(Kaby Lake-G, Hades Canyon)*
- ⬜ Radeon Pro Vega 16 · ⬜ Radeon Pro Vega 20 *(MacBook Pro 15″ 2018–2019, Metal/OpenCL)*

## Radeon Pro Mobile — Apple MacBook Pro и мобильные рабочие станции
> В маках доступен бэкенд **Metal** (hashcat 6.2.6+) и OpenCL — реалистичная цель.

- ⬜ Radeon Pro 450 / 455 / 460 *(MBP 2016, Polaris 11)*
- ⬜ Radeon Pro 555 / 555X · ⬜ Radeon Pro 560 / 560X *(MBP 2017–2019)*
- ⬜ Radeon Pro 570X / 575X / 580X *(iMac 2019, формально десктоп-моб. чип)*
- ⬜ Radeon Pro 5300M · ⚠️ Radeon Pro 5500M (mode 11600 partial raw) · ⬜ Radeon Pro 5600M *(MBP 16″ 2019–2020, RDNA)*
- 🔒 Radeon Pro WX 2100 / 3100 (Mobile) · 🔒 Radeon Pro WX 3200 · ⬜ Radeon Pro WX 4100 / 4130 / 4150
- ⬜ Radeon Pro WX 7100 (Mobile) · ⬜ Radeon Pro WX Vega M GL
- 🔒 Radeon Pro W6300M · ⬜ Radeon Pro W6400M · ⬜ Radeon Pro W6500M
- ⬜ Radeon Pro W6600M · ⬜ Radeon Pro W6800M · ⬜ Radeon Pro W7600M / W7800M *(наличие в рознице ограничено)*

## Radeon RX — RDNA Mobile (2019–2020) · OpenCL 2.0 / HIP (gfx1010–1012)
- ⬜ Radeon RX 5300M · ⬜ Radeon RX 5500M · ⬜ Radeon RX 5600M · ⬜ Radeon RX 5700M

## Radeon RX — RDNA 2 Mobile (2021–2022) · OpenCL / HIP (gfx1032–1034)
- 🔒 Radeon RX 6300M · 🔒 Radeon RX 6450M · ⬜ Radeon RX 6500M · ⬜ Radeon RX 6550M
- ⬜ Radeon RX 6550S · ⬜ Radeon RX 6600M · ⬜ Radeon RX 6600S · ⬜ Radeon RX 6650M
- ⬜ Radeon RX 6650M XT · ⬜ Radeon RX 6700M · ⬜ Radeon RX 6700S
- ✅ Radeon RX 6800M · ⬜ Radeon RX 6800S · ⬜ Radeon RX 6850M XT

## Radeon RX — RDNA 3 Mobile (2023–2024) · OpenCL / HIP (gfx1101–1102)
- ⬜ Radeon RX 7600M · ⬜ Radeon RX 7600M XT · ⬜ Radeon RX 7600S · ⬜ Radeon RX 7700S
- ⬜ Radeon RX 7800M · ⬜ Radeon RX 7900M

## AMD APU — встроенная графика (2018–2025)
> В ноутбуках это самый массовый «мобильный GPU». OpenCL/HIP работает,
> производительность низкая, но публичные прогоны встречаются.

| Поколение | Год | Модели iGPU | Архитектура | API | Статус |
|---|---|---|---|---|---|
| Raven Ridge / Picasso | 2018–19 | Radeon Vega 3 · Vega 6 · Vega 8 · Vega 10 · Vega 11 | GCN 5 (Vega) | OpenCL 2.0 | ⬜ Vega 8/11, 🔒 остальные |
| Renoir / Lucienne | 2020–21 | Radeon Graphics Vega 5 · Vega 6 · Vega 7 · Vega 8 | GCN 5 (Vega) | OpenCL 2.0 | ⬜ Vega 7/8 |
| Cezanne / Barcelo | 2021–22 | Radeon Graphics (Vega 6/7/8) | GCN 5 (Vega) | OpenCL 2.0 | ⬜ |
| Van Gogh | 2022 | AMD Custom GPU 0405 / 0932 *(Steam Deck)* | RDNA 2 | OpenCL / HIP | ✅ Steam Deck |
| Mendocino | 2022 | Radeon 610M | RDNA 2 | OpenCL | 🔒 |
| Rembrandt | 2022 | Radeon 660M · Radeon 680M | RDNA 2 | OpenCL / HIP | ⬜ |
| Phoenix / Hawk Point | 2023–24 | Radeon 740M · 760M · 780M | RDNA 3 | OpenCL / HIP | ⚠️ 760M full; 780M partial; 740M open |
| Phoenix 2 | 2024 | Radeon 740M · 780M (кастом) | RDNA 3 | OpenCL | 🔒 |
| Strix Point | 2024 | Radeon 840M · 860M · 880M · 890M | RDNA 3.5 | OpenCL / HIP | ⬜ |
| Krackan Point | 2025 | Radeon 820M · 840M · 860M | RDNA 3.5 | OpenCL | ⬜ |
| Strix Halo | 2025 | Radeon 8050S · 8060S | RDNA 3.5 | OpenCL / HIP | ⬜ |

---

# 🟦 Intel

## Встроенная графика (iGPU)

| Поколение / кодовое имя | Год | Модели | API | Статус |
|---|---|---|---|---|
| Sandy Bridge (Gen 6) | 2011 | HD Graphics 2000 · HD Graphics 3000 | нет OpenCL на GPU | 🔒 |
| Ivy Bridge (Gen 7) | 2012 | HD Graphics 2500 · HD Graphics 4000 | OpenCL 1.2 (легаси-драйвер) | 🔒 |
| Haswell (Gen 7.5) | 2013 | HD 4200 · HD 4400 · HD 4600 · HD 5000 · Iris Graphics 5100 · Iris Pro Graphics 5200 | OpenCL 1.2 | 🔒 |
| Broadwell (Gen 8) | 2015 | HD 5300 · HD 5500 · HD 5600 · HD 6000 · Iris Graphics 6100 · Iris Pro Graphics 6200 | OpenCL 2.0 | 🔒 |
| Skylake (Gen 9) | 2015–16 | HD 510 · HD 515 · HD 520 · HD 530 · Iris Graphics 540 · Iris Graphics 550 · Iris Pro Graphics 580 | OpenCL 2.1 | ⬜ (HD 520/530, Iris Pro 580) |
| Kaby Lake (Gen 9.5) | 2016–17 | HD 610 · HD 615 · HD 620 · HD 630 · Iris Plus Graphics 640 · Iris Plus Graphics 650 | OpenCL 2.1 | ⬜ |
| Coffee/Whiskey/Comet Lake | 2018–20 | UHD Graphics 610 · 617 · 620 · 630 | OpenCL 2.1 / 3.0 | ⬜ (UHD 620/630) |
| Ice Lake (Gen 11) | 2019 | UHD Graphics G1 · Iris Plus Graphics G4 · Iris Plus Graphics G7 | OpenCL 3.0 (NEO) | ⬜ |
| Tiger Lake (Xe-LP) | 2020 | UHD Graphics Xe 32EU · Iris Xe Graphics G7 80EU · Iris Xe Graphics G7 96EU | OpenCL 3.0 / Level Zero | ⬜ |
| Rocket/Alder/Raptor Lake (Xe-LP) | 2021–23 | Iris Xe Graphics (96EU) · UHD Graphics (32/48EU) | OpenCL 3.0 / Level Zero | ⚠️ Raptor Lake-P partial MD5 raw only |
| Meteor Lake (Xe-LPG) | 2023–24 | Intel Arc Graphics (8-Xe-Core / 7-Xe-Core / 4-Xe-Core) · Intel Graphics (4-Xe-Core) | OpenCL 3.0 / Level Zero | ⬜ |
| Lunar Lake (Xe2-LPG) | 2024 | Intel Arc Graphics 130V · Intel Arc Graphics 140V | OpenCL 3.0 / Level Zero | ⚠️ 140V (self-test errors) |
| Arrow Lake-H (Xe-LPG+) | 2025 | Intel Arc Graphics 130T · Intel Arc Graphics 140T | OpenCL 3.0 / Level Zero | ⬜ |
| Panther Lake (Xe3) | 2025–26 | Intel Arc Graphics (Xe3, до 12 Xe-ядер) | OpenCL / Level Zero | ⬜ |

## Intel Arc — дискретные мобильные (Alchemist, 2022) · OpenCL 3.0 / Level Zero
- ⬜ Intel Arc A310M *(редкий OEM)* · ⬜ Intel Arc A350M · ⬜ Intel Arc A370M
- ⬜ Intel Arc A530M · ⬜ Intel Arc A550M · ⬜ Intel Arc A570M
- ⬜ Intel Arc A730M · ✅ Intel Arc A770M (additional ZerNox partial raw, 9 modes)
- ⬜ Intel Arc Pro A30M · ⬜ Intel Arc Pro A40 / A50 *(мобильные workstation-варианты)*

---

# 🍎 Apple

Apple Silicon (M1 → M4 и далее) — **уже покрыт** отдельным разделом в
[`COVERAGE.md`](COVERAGE.md) (бэкенд **Metal**, hashcat 6.2.6+). Здесь не
дублируется, чтобы не расходились два списка.

Дискретные AMD в MacBook Pro/iMac учтены выше в разделе
[Radeon Pro Mobile](#radeon-pro-mobile--apple-macbook-pro-и-мобильные-рабочие-станции).

Дояблокремниевые Intel iGPU в маках (Iris Plus 640/650, Iris Pro 5200 и т. д.)
перечислены в таблице Intel.

---

# 📊 Итоговый счётчик

Счёт по количеству проставленных меток (строки таблиц Intel и AMD APU
объединяют по несколько родственных моделей — фактических SKU там больше).

| Вендор | Всего позиций | ✅ есть | ⬜ искать | 🔒 маловероятно |
|---|---|---|---|---|
| NVIDIA (GeForce + Quadro/RTX Pro + MX + Tegra/Jetson) | 183 | 7 | 94 | 82 |
| AMD (Radeon Mobility/RX + Radeon Pro + APU iGPU) | 178 | 2 | 62 | 114 |
| Intel (iGPU-поколения + Arc mobile) | 24 | 1 | 19 | 4 |
| **Итого** | **385** | **10** | **175** | **200** |

> ✅ в этом файле: GTX 1060 Max-Q · GTX 1650 Ti · RTX 2060 Mobile · RTX 3060 Laptop ·
> RTX 3070 Laptop · RTX 4050 Laptop · RX 6800M (+ Steam Deck и Jetson Nano в таблицах) ·
> Intel Arc A770M.

## Оценка: по чему реально имеет смысл искать

Формально ⬜ помечено 175 позиций, но реалистичность сильно неоднородна.
Приоритеты для будущего поиска:

1. **Высокая вероятность найти (~45 моделей)** — игровые ноутбучные dGPU
   2019–2025, по которым люди активно постят прогоны: RTX 20/30/40/50 Laptop
   (все ступени + Max-Q), GTX 1650/1660 Ti Mobile, RX 6600M–6850M XT,
   RX 7600M XT–7900M, Arc A370M/A730M.
2. **Средняя (~50)** — Pascal Mobile и Maxwell 900M (GTX 950M–980M, 1050–1080
   Laptop), workstation-мобильные (Quadro P/T/RTX, RTX A * Laptop,
   RTX Ada Laptop), MX150/MX250/MX350/MX450/MX550, RDNA1 RX 5500M/5600M,
   Radeon Pro 5500M/5600M в MacBook Pro.
3. **Низкая, но не нулевая (~60)** — Intel iGPU (HD 520 … Iris Xe … Arc 140V):
   технически всё работает, но прогоны выкладывают редко и они малоинтересны;
   AMD APU-графика (Vega 8/11, 680M/780M/890M); мобильные Polaris/Vega M.
4. **Практически нулевая (198 🔒)** — вся Fermi/Kepler мобильная линейка,
   TeraScale и GCN 1.x Mobility, Intel Gen 6–8, low-end MX/R5/Radeon 5xx.
   Их держим в реестре только ради полноты справочника.

**Практический вывод:** осмысленный «рабочий фронт» поиска — примерно
**95–110 моделей** (пункты 1–2). Остальное — либо архивная экзотика, либо
iGPU-мелочь, по которой публичных выводов `hashcat -b` почти не бывает.
