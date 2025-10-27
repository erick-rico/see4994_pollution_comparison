# 🎯 Research Question – Week 5

## Main Question
**How do large-scale synoptic patterns influence extreme air-pollution days in Mexico City?**

---

### Sub-questions
1. Do high-pollution days (P90) correspond to specific mid-tropospheric (500 hPa) circulation anomalies?  
2. Are weak low-level winds (850 hPa) consistently associated with pollutant accumulation events?  
3. How coherent are these synoptic patterns across months and pollutants (PM₂.₅, PM₁₀, O₃, NO₂, SO₂)?  
4. Can the composite approach capture statistically significant anomalies (p < 0.05) indicating recurring meteorological setups?

---

### Approach Summary
- Identify monthly P90 pollution days → “event days”.  
- Use NARR fields (`hgt`, `uwnd`, `vwnd`) at 500 hPa & 850 hPa to build composites of:
  - Mean HGT (contours)  
  - HGT anomalies (HGT′, shading)  
  - Mean wind vectors (U,V)  
  - Stippling for p < 0.05
- Compare results across pollutants and levels.

---

### Expected Outcome
To reveal **synoptic coherence** — i.e., a consistent ridge or stagnation pattern appearing whenever Mexico City experiences high pollution, suggesting that local air quality extremes are embedded in broader atmospheric dynamics.

---

### Future Directions
- Refine spatial resolution (zoom into MCMA).  
- Extend to comparative study with Hong Kong (similar urban basin, different monsoon regime).  
- Automate composite generation for different pressure levels and seasons.

---
