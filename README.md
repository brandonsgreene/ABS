# ABS

# 🧱 ABS @BBL H2D – Printing Profile & History

**Author:** Brandon Greene  
**Printer:** Bambu Lab H2D  
**Material:** ABS  
**Profile Version:** Standard V1  
**Purpose:** Documenting the complete process, tuning history, and performance results of ABS printing within the enclosed Bambu H2D system.

---

## ⚙️ Overview

This repository tracks the configuration, experiments, and iterative improvements made while developing a consistent, high-quality ABS printing profile for the **Bambu Lab H2D**.

The goal is reliability under real-world conditions — consistent adhesion, dimensional accuracy, minimal warping, and predictable mechanical strength.

The project captures not just slicer settings, but reasoning, environment, and field feedback from actual prints.

---

## 🧾 Current Stable Profile

**File:** `ABS_Standard_V1.txt`  
**Profile Type:** General-purpose ABS  
**Key Results:**
- Excellent layer adhesion at 245 °C / 100 °C / 65 °C chamber
- Smooth sidewalls with controlled overhang cooling
- Supports release cleanly after full cooling
- Nozzle swaps and AMS spool transitions stable mid-print
- Chamber maintains 9–11% RH consistently

**Recommended Use:**  
Functional parts, jigs, mechanical housings, and stress-bearing prototypes.

---

## 🔍 Version History

### **V1 – Standard (Current)**
- Tuned for stability and repeatability.
- Layer height: 0.20 mm.
- Nozzle: 245 °C.
- Bed: 100 °C.
- Chamber: 65 °C.
- Initial layer speed reduced to 20 mm/s.
- Overhang slowdowns enabled.
- Refined support gap: 0.25 mm.
- Rib walls and fillet edges enabled for stress diffusion.
- Flush into infill + supports for material efficiency.

**Result:**  
Strong mechanical adhesion, crisp top surfaces, zero warping on 3-hour prints. Best balance between print quality and throughput.

---

### **Planned V2 – High Precision (In Development)**
Goals:
- Layer height: 0.16 mm.
- Top/bottom density increase for smoother skin.
- Arc fitting & X/Y compensation tuned for tolerances under ±0.1 mm.
- Reduced nozzle temp (240 °C) for finer detail.
- Z-hop adjustment during travel for small-part cooling stability.

---

## 🧪 Environment & Hardware Notes

| Parameter | Target | Notes |
|------------|---------|------|
| AMS Humidity | 8–12% RH | If RH drops below 7%, static can increase feed drag. |
| Chamber Temp | 65 °C | Keep lid closed for consistency. |
| Air Conditioner | Heating mode only | No active cooling during ABS jobs. |
| Filament Type | Bambu ABS / Polymaker ABS | Both tested successfully. |
| Bed Type | Textured PEI | Apply Magigoo or ABS slurry for large parts. |

---

## 🧠 Lessons Learned

- **First-Layer Speed:** Slower (≤ 20 mm/s) ensures consistent adhesion without elephant footing.  
- **Chamber Stability:** Cracking and layer separation start around 55 °C or below; keep ambient steady.  
- **Humidity Management:** AMS readings below 10% improve extrusion smoothness and reduce bubbling.  
- **Overhang Slowdown:** Critical for complex geometries; small perimeter control prevents drag lines.  
- **Cooling Discipline:** Avoid external fans — chamber convection is sufficient after layer 5.  
- **Support Interface:** Concentric interface + 0.25 mm gap gives best removal quality.

---

## 🧰 Files in This Repo