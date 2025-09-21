# Bug Report Samples

**Author:** Manolkin (Tor’Ion)  
**Role:** QA Tester | Systems Optimizer | AI Image Engineer  
**Date Range:** Ongoing (2024–2025)

---

## 📢 Disclaimer
The following bug reports are **sample formats** created to demonstrate professional QA documentation style.  
They are not necessarily based on issues I have personally encountered or reproduced.  
Real bug reports will be added over time as they are discovered and verified.

---

## 🧩 Purpose
To demonstrate clear, reproducible, and developer‑ready bug reports across different domains — from game testing to AI workflows and system optimization.

---

## 📄 Sample 1 – Game Bug (Space Marine 2 PvP)

**Title:** Vanguard Class – Grapple Animation Lock After Interrupt  
**Environment:**  
- Game: Space Marine 2 (Closed PvP Test)  
- Platform: Windows 11 Home (Insider build)  
- GPU: AMD Radeon RX 7900 GRE  
- CPU: AMD Ryzen 5 5600X  
- Network: Wired, 1 Gbps  

**Steps to Reproduce:**
1. Equip Vanguard class with default melee loadout.  
2. Initiate grapple on enemy player.  
3. Have a third player interrupt grapple with ranged attack during animation wind‑up.  
4. Attempt to move or attack after animation break.

**Expected Result:**  
Player regains control immediately after grapple is interrupted.

**Actual Result:**  
Player remains locked in grapple animation pose for 3–5 seconds, unable to move or attack.

**Severity:** High (affects combat flow in competitive matches)  
**Attachments:** Video clip + frame‑time graph showing input lock duration.

## Sample 1b -
### Bug Report – Animation Lock on Vanguard Charge Cancel

**Title:** Vanguard charge cancel leaves player in locked animation state  
**Environment:** Space Marine 2 PvP – Closed Test Build (2025‑09‑15)  
**Steps to Reproduce:**
1. Equip Vanguard class.  
2. Initiate charge attack.  
3. Cancel charge mid‑animation by switching weapons.  
4. Attempt to perform melee or dodge immediately after cancel.

**Expected Result:** Player regains full control instantly after cancel.  
**Actual Result:** Player remains locked in partial charge animation for ~1.5 seconds, unable to act.  
**Frequency:** ~60% when cancel timing is within final 5 frames of charge wind‑up.  
**Impact:** High – leaves player vulnerable in competitive scenarios.  
**Notes:** Possibly related to animation state machine not resetting on cancel event.
---

## 📄 Sample 2 – AI Workflow Bug (Mythic Portrait Series)

**Title:** Harmonic Coil Sigil Rendering Inconsistent Across Iterations  
**Environment:**  
- AI Platform: [Model/Version]  
- Prompt: Mythic Portrait Series template with fixed seed  
- Parameters: 1024×1024, Guidance 7.5, Negative prompts active  

**Steps to Reproduce:**
1. Use provided prompt template with fixed seed.  
2. Generate 10 iterations, changing only lighting descriptor.  
3. Compare sigil rendering in each output.

**Expected Result:**  
Sigil shape and placement remain consistent across all iterations.

**Actual Result:**  
Sigil distorts or disappears entirely in ~30% of outputs.

**Severity:** Medium (affects visual consistency in published series)  
**Attachments:** Iteration gallery with annotations.

---

## 📄 Sample 3 – System Optimization Bug (ROCm on WSL2)

**Title:** ROCm Kernel Panic Under High Parallel Load  
**Environment:**  
- OS: Windows 11 Home (Insider build)  
- WSL2: Ubuntu 22.04  
- GPU: AMD Radeon RX 7900 GRE  
- ROCm Version: [Insert version]  

**Steps to Reproduce:**
1. Launch Stable Diffusion batch job (batch size 8).  
2. Run simultaneous Blender GPU render in WSL2.  
3. Monitor GPU utilization and kernel logs.

**Expected Result:**  
Both workloads complete without driver crash.

**Actual Result:**  
ROCm kernel panic after ~2 minutes, WSL session terminates.

**Severity:** Critical (causes data loss and requires system restart)  
**Attachments:** ROCm kernel log excerpt + GPU utilization chart.

---

## 🔍 Notes
- All reports follow a **clear, reproducible format**: Title → Environment → Steps → Expected vs Actual → Severity → Attachments.  
- Severity levels are assigned based on gameplay impact, workflow disruption, or system stability risk.  
- Attachments are referenced but stored separately in `/QA-Case-Studies/attachments/`.

---
