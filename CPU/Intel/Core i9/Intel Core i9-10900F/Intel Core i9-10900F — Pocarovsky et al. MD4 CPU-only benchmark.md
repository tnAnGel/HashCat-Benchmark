# Intel Core i9-10900F — MD4 CPU-only benchmark

- **Processor:** Intel Core i9-10900F.
- **Hashcat mode:** benchmark mode, MD4 (mode 900).
- **Reported speed:** 3,147.5 MH/s.
- **Backend / isolation:** the paper's CPU-measurement section explicitly says GPUs were disabled and describes the result as the CPU benchmark. It does not publish a backend banner or Hashcat version in the text; retained as a published CPU-only aggregate, not raw stdout.
- **Tuning reported:** Accel 1024, Loops 1024, Thr 1, Vec 8.
- **Source:** Pocarovsky et al., “Computational Efficiency of Brute-Force Attacks on Hashing Algorithms,” *Software Engineering: Emerging Trends and Practices in System Development*, LNNS 1558 (2026), pp. 402–413, [DOI: 10.1007/978-3-032-00236-5_30](https://doi.org/10.1007/978-3-032-00236-5_30); [public full text](https://www.researchgate.net/publication/396553540_Computational_Efficiency_of_Brute-Force_Attacks_on_Hashing_Algorithms).

The paper separately reports 3,023.3 MH/s for the CPU in a CPU+GPU run; that mixed result is intentionally not substituted for the CPU-only figure above.
