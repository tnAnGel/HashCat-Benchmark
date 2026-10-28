# Intel Iris Xe Graphics (13th-gen Intel Core i7-1355U) — MD5 raw excerpt

- **GPU identification:** gist author identifies the GPU in their Lenovo ThinkPad T16 Gen 2 as Intel Iris Xe Graphics. The Hashcat device line reports the host CPU model (`13th Gen Intel Core i7-1355U`), not the Iris Xe marketing name; exact iGPU device ID/SKU is not present in the excerpt.
- **Hashcat:** v6.2.6-827-g46ce637d3.
- **Command:** `./hashcat -D 1 -b -m 0` — GPU device type selected, MD5 mode only.
- **Result:** mode 0 (MD5), `369.7 MH/s`.
- **Evidence type:** raw stdout excerpt for one explicitly requested mode, not a complete all-modes benchmark and not a PTS aggregate.
- **Source:** [AlbertVeli's public gist](https://gist.github.com/AlbertVeli/8bf70de44daec9d7169f71c6a4a56fbf).

## Raw stdout excerpt

```text
$ ./hashcat -D 1 -b -m 0
hashcat (v6.2.6-827-g46ce637d3) starting in benchmark mode
...
OpenCL API (OpenCL 1.2 Intel(R) FPGA SDK for OpenCL(TM), Version 20.3) - Platform #1 [Intel(R) Corporation]
===========================================================================================================
* Device #1: Intel(R) FPGA Emulation Device, skipped

OpenCL API (OpenCL 3.0 LINUX) - Platform #2 [Intel(R) Corporation]
==================================================================
* Device #2: 13th Gen Intel(R) Core(TM) i7-1355U, 15843/31751 MB (7937 MB allocatable), 12MCU

OpenCL API (OpenCL 2.0 pocl 1.8 Linux, None+Asserts, RELOC, LLVM 11.1.0, SLEEF, DISTRO, POCL_DEBUG) - Platform #3 [The pocl project]
=====================================================================================================================================
* Device #3: pthread-13th Gen Intel(R) Core(TM) i7-1355U, skipped

Benchmark relevant options:
===========================
* --backend-devices-virtual=1
* --opencl-device-types=1
* --optimized-kernel-enable

-------------------
* Hash-Mode 0 (MD5)
-------------------

Speed.#2.........: 369.7 MH/s (33.67ms) @ Accel:1024 Loops:1024 Thr:1 Vec:8
```

The source has an ellipsis (`...`) in the published output, so it is retained as an excerpt rather than presented as a complete stdout capture.
