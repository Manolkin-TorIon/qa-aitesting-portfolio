# ROCm Tuning Notes – Kernel Parameter Experiments

**Date:** 2025‑09‑21  
**System:** Ryzen 5 5600X | RX 7900 GRE | 64GB Corsair Vengeance @ 3200MHz

---

## Experiment: Wavefront Size Adjustment
- **Parameter:** `HSA_ENABLE_SDMA=0`  
- **Purpose:** Disable SDMA to reduce latency in AI workloads.  
- **Result:**  
  - Latency reduced by ~4% in batch inference tests.  
  - Slight increase in CPU load (~2%).  
- **Notes:** Stable under sustained load; recommend pairing with `ROCR_VISIBLE_DEVICES` for targeted GPU allocation.

---

## Next Steps
- Test with mixed precision workloads.  
- Compare against default in ROCm 6.0+.
