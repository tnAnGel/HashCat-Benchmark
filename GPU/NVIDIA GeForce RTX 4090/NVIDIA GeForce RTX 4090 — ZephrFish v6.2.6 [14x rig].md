# NVIDIA GeForce RTX 4090 (14x rig) — hashcat v6.2.6 (raw benchmark)

- **Тип свидетельства:** полный raw stdout benchmark mode из GitHub Gist.
- **Конфигурация:** 14 × RTX 4090; `Speed.#1–#14` — отдельные карты, `Speed.#*` — сумма стенда. В таблице указаны GPU #1 и стендовая сумма, не выдаваемая за скорость одной карты.
- **Hashcat / runtime:** v6.2.6, CUDA 12.3; optimized kernel; конфигурация cloud rig.
- **Источник:** [Gist — исходная публикация](https://gist.github.com/ZephrFish/b849331aafa015ddd7786ca20ce718d7) · [полный raw stdout](https://gist.githubusercontent.com/ZephrFish/b849331aafa015ddd7786ca20ce718d7/raw/e3d896c9c1ed1f346c1fa1f44d31c563acd84b0b/14_RTX_4090_v6.2.6.Benchmark.txt).
- **Отличие от имеющихся данных:** отдельный 14-карточный raw run; локальный OnlineHashCrack benchmark — другой 8× rig, а single-card файлы являются отдельными прогонами.

| Mode | Алгоритм | GPU #1 | 14× суммарно `Speed.#*` |
|---:|---|---:|---:|
| 0 | MD5 | 142.0 GH/s | 2,009.0 GH/s |
| 100 | SHA1 | 47,286.0 MH/s | 667.1 GH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 2,371.0 kH/s | 34,003.2 kH/s |
| 1000 | NTLM | 242.0 GH/s | 3,419.2 GH/s |

Полный лог содержит результаты по всем доступным режимам и всем 14 устройствам. У каждой карты свой `Speed.#N`; не делить агрегат равномерно для получения точной скорости отдельного экземпляра.
