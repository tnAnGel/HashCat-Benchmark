# AMD Ryzen 7 7700 — Hashcat CPU WPA2 dictionary results

- **Processor:** AMD Ryzen 7 7700 (Zen 4, 8 cores / 16 threads).
- **Workload:** Hashcat WPA2 dictionary-attack throughput, reported as passwords/s; this is an actual attack measurement, not Hashcat's synthetic `-b` rate.
- **CPU attribution:** the peer-reviewed study labels the experiment and result table “CPU Architecture Comparison” and lists this CPU as a tested CPU. GPU measurements are reported separately. The paper does not include raw Hashcat stdout or an OpenCL device banner, so this is a study-attributed aggregate, not a raw backend transcript.
- **Source:** Oleksii Chalyi, “Assessing Wi-Fi Security Protocols: A Study of Dictionary Attack Performance,” *Baltic Journal of Modern Computing* 13(3), 592–623 (2025), [DOI: 10.22364/bjmc.2025.13.3.03](https://doi.org/10.22364/bjmc.2025.13.3.03); [publisher PDF](https://www.bjmc.lu.lv/fileadmin/user_upload/lu_portal/projekti/bjmc/Contents/13_3_03_Chalyi.pdf).

| Published CPU test condition | Hashcat speed |
|---|---:|
| CPU fixed at 1.7 GHz | 28,040 pw/s |
| CPU fixed at 3.6 GHz | 60,109 pw/s |
| Default/unrestricted frequency, average | 110,900 pw/s |

The paper used a `rockyou.txt` dictionary attack against a WPA2 handshake and lists repeated runs for the CPU experiments. No Hashcat version is stated.
