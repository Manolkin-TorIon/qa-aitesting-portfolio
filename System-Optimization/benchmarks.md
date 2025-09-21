# Benchmark Log – Harmonic Coil Systems

**System:** Ryzen 5 5600X | RX 7900 GRE | 64GB DDR4 @ 3200MHz  
**Date:** 2025‑09‑21

---

## Test Suite: Mixed Workload (Gaming + ROCm AI Inference)
- **3DMark Time Spy:** 17,842 (GPU: 18,210 | CPU: 9,850)  
- **Unigine Superposition (4K Optimized):** 10,412  
- **ROCm AI Batch Inference:** 4.2% latency reduction vs. baseline after kernel tuning  
- **Thermals:** Peak GPU 72°C, CPU 74°C under sustained load

---

## Notes:
- Stable under 6‑hour mixed load test.  
- ROCm tuning parameters from `rocm-tuning-notes.md` applied.  
- BIOS profile: Balanced Performance OC (see `bios-configs.md`).
