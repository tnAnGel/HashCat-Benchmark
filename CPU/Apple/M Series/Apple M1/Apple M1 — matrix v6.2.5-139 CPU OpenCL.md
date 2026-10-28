# Apple M1 — Hashcat CPU OpenCL benchmark

- **CPU device:** `Apple M1`; `hashcat -I` explicitly reports `Type: CPU` for Backend Device #1. The same report lists a separate Apple M1 GPU as Device #2.
- **Hashcat:** v6.2.5-139-ge2eacb4dd+ (x86_64 build under Rosetta 2).
- **Backend:** Apple OpenCL 1.2; command `./hashcat -b --benchmark-all -D1,2`. CPU and GPU were both enabled; the values below are only `Speed.#1` (CPU), not the combined `Speed.#*`.
- **Evidence:** raw benchmark output and `hashcat -I` device-type output in [matrix's GitHub Gist](https://gist.github.com/matrix/ae6b64a6e44392355a5467d129fd8bee); [raw file](https://gist.githubusercontent.com/matrix/ae6b64a6e44392355a5467d129fd8bee/raw/).
- **Classification:** per-device raw stdout excerpt; concurrent GPU device was active, so this is not a CPU-isolated run.

| Hash mode | Algorithm | CPU speed (`Speed.#1`) |
|---:|---|---:|
| 0 | MD5 | 186.6 MH/s |
| 100 | SHA1 | 140.7 MH/s |
| 900 | MD4 | 394.6 MH/s |
| 1000 | NTLM | 391.4 MH/s |
| 1400 | SHA2-256 | 61.5455 MH/s |
| 22000 | WPA-PBKDF2-PMKID+EAPOL | 6,802 H/s |

The full gist contains the complete `--benchmark-all` output. Only the CPU-device column is transcribed here.
