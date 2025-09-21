# Benchmark Results – Before & After Optimization

**Author:** Manolkin (Tor’Ion)  
**Role:** Systems Optimizer | QA Tester  
**Date Range:** Ongoing (2024–2025)

---

## 📊 Summary
Performance metrics recorded before and after BIOS tuning, AMD GPU optimization, and thermal management adjustments on my current build.

---

## 🖥 Test Environment
- **OS:** Windows 11 Home (64-bit, Insider build)
- **CPU:** AMD Ryzen 5 5600X (6 cores / 12 threads)  
- **GPU:** AMD Radeon RX 7900 GRE  
- **RAM:** 64GB Corsair Vengeance DDR4 OC’d to 3200 MHz (dual channel)  
- **Storage:** NVMe SSD (primary OS + workloads)  
- **Motherboard:** ASUS TUF GAMING B550-PLUS (WI-FI)  
- **Power Plan:** Balanced  
- **AI Workload:** Stable Diffusion image generation (1024×1024, batch size 4)  
- **Benchmark Tools:** Geekbench 6.5.0, Geekbench AI, ROCm utilities, custom AI inference scripts

---

## 📈 Results Table

| Test | Pre‑Optimization | Post‑Optimization | % Improvement |
|------|------------------|-------------------|---------------|
| Geekbench 6 CPU – Single-Core | — | 1735 | — |
| Geekbench 6 CPU – Multi-Core | — | 8503 | — |
| AI Image Gen (it/s) | 7.2 | 8.4 | +16.7% |
| Geekbench Compute Score (Vulkan) | — | 173,876 | — |
| Geekbench Compute Score (OpenCL) | — | 169,980 | — |
| Geekbench AI – Single Precision | — | 2481 | — |
| Geekbench AI – Half Precision | — | 1213 | — |
| Geekbench AI – Quantized | — | 3837 | — |
| Max GPU Temp (°C) | 83 | 71 | -14.5% |

---

## 🔍 Observations
- CPU and GPU baselines now established for tracking future tuning gains.
- ROCm/driver tuning + kernel parameter adjustments yielded the largest AI workload gains.
- Thermal improvements allowed sustained boost clocks without throttling.
- Memory OC stability was critical for consistent performance.
