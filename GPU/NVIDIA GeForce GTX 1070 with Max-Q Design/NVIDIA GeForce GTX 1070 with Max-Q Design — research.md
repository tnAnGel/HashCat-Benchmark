# NVIDIA GeForce GTX 1070 with Max-Q Design

- **Статус:** ⚠️ найден частичный запуск hashcat; benchmark-mode `-b` не найден
- **Источник:** [Reddit — Using Nvidia 1070 Max-Q with Hashcat](https://www.reddit.com/r/HowToHack/comments/ciywre/), MSI laptop, hashcat v5.1.0
- **Подтверждение устройства:** вывод hashcat показывает `GeForce GTX 1070 with Max-Q Design`, 8192 MB, 16 MCU.
- **Опубликованный режим:** LUKS (mode 14600), скорость во время атаки по словарю — 103 H/s.

Это реальный runtime-результат, но не benchmark `hashcat -b`; в `MOBILE.md` отмечен как частичный.
