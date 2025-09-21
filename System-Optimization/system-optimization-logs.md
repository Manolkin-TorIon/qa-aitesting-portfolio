# System Optimization Logs

**Author:** Manolkin (Tor’Ion)  
**Role:** Systems Optimizer | QA Tester | Hardware Tuner  
**Date Range:** Ongoing (2024–2025)

---

## 🎯 Objective
To document BIOS tuning, ROCm/AMD GPU optimization, and system-level adjustments that improve performance, stability, and workflow efficiency.

---

## 🧩 Optimization Areas

### 1. **BIOS Tuning**
- Adjusted memory timings for stability under heavy GPU load.
- Enabled/disabled specific CPU features to optimize AI/ML workloads.
- Updated firmware to latest stable build after regression testing.

### 2. **ROCm/AMD GPU Optimization**
- Installed and configured ROCm for AI acceleration under WSL.
- Tuned kernel parameters for reduced latency in compute-heavy tasks.
- Benchmarked performance before and after driver updates.

### 3. **Thermal & Power Management**
- Adjusted fan curves for optimal cooling without excessive noise.
- Applied undervolting to reduce thermal throttling.
- Logged temperature deltas under sustained load.

---

## 📊 Key Outcomes
- Achieved **12–18% performance gain** in AI image generation benchmarks.
- Reduced thermal throttling events by **~40%**.
- Improved system stability during multi-hour stress tests.

---

## 🛠 Tools & Environments
- Windows 11 (Insider builds)
- WSL (Windows Subsystem for Linux)
- ROCm/AMD GPU stack
- BIOS/UEFI configuration tools
- Benchmarking utilities (e.g., Geekbench, Blender, custom AI workloads)

---

## 📂 Evidence
- [Benchmark Results – Before/After](./benchmark-results.md)
- [BIOS Settings Reference](./bios-settings-reference.md)
- [ROCm Configuration Notes](./rocm-config-notes.md)

---

## 🔍 Lessons Learned
- Incremental changes with proper logging prevent instability.
- ROCm performance can vary significantly between driver versions — always benchmark.
- Thermal management is as critical as raw clock speed for sustained performance.

---

*This log demonstrates applied technical skill in hardware and software optimization, with measurable, documented results.*
