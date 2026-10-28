# NVIDIA GeForce RTX 4060 Laptop GPU

- **Вендор / Vendor:** NVIDIA
- **Видеокарта / GPU:** GeForce RTX 4060 Laptop GPU
- **Версия hashcat / Version:** в статье не указана (автор использует пакет Debian в WSL 2)
- **Источник / Source:** [ATTACKD — How to Use NVIDIA Graphics Cards in WSL 2](https://attackd.com/blog/how-to-use-nvidia-graphics-cards-in-wsl-2/)
- **Параметры / Options:** `hashcat -b -m 1000`
- **Примечание / Note:** частичный benchmark только для NTLM; в той же системе Hashcat суммирует GPU с CPU, поэтому для таблицы взята строго строка `Speed.#1` (GPU), а не `Speed.#*`.

## Результат / Result

| Mode | Алгоритм | RTX 4060 Laptop GPU |
|-----:|----------|--------------------:|
| 1000 | NTLM | 32.7656 GH/s |

## Исходные строки / Raw excerpt

```text
hashcat -b -m 1000
* Device #1: NVIDIA GeForce RTX 4060 Laptop GPU
* Device #2: Intel Core i9 CPU
Speed.#1.........: 32765.6 MH/s
Speed.#2.........:  1939.0 MH/s
Speed.#*.........: 34704.6 MH/s
```

Отдельный форумный пост приводит ещё один однорежимный результат для этой модели: mode 22000 — 461.1 kH/s, без версии Hashcat и полного stdout: [Hashcat Forum, RTX 2060 vs 4060 laptop](https://hashcat.net/forum/thread-11704-post-59603.html).
