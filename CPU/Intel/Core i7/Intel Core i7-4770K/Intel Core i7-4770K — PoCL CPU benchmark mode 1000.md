# Intel Core i7-4770K — CPU OpenCL benchmark (mode 1000)

- **CPU device:** Intel Core i7-4770K @ 3.50 GHz, explicitly identified as the CPU device in the source output.
- **Hashcat command:** `oclHashcat -b -m 1000 --opencl-device-types 1 --opencl-platforms 1` (native Intel OpenCL) and the same with `--opencl-platforms 2` (PoCL); device type 1 is CPU.
- **Hash mode:** 1000, NTLM.
- **Results:** Intel OpenCL 1,019.7 MH/s; PoCL 522.7 MH/s.
- **Source:** [PoCL issue #292 — CPU performance vs native Intel OpenCL runtime](https://github.com/pocl/pocl/issues/292).
- **Classification:** partial raw stdout excerpt. Hashcat/oclHashcat build version is not specified in the post; the two runtimes are separate CPU-only runs.

The source output names the processor on both runtimes and reports `Speed.Dev.#1` for the CPU. No system GPU performance is included in these figures.
