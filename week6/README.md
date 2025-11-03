# Week 6 – Synoptic Control of High-Pollution Days in Mexico City

**Course:** SEE4994 – Guided Research Project  
**Supervisor:** Dr. Jung-Eun Chu (City University of Hong Kong)  
**Student:** Erick Rico Esparza  
**Period:** Oct 29 – Nov 12, 2025  

---

## Overview

This week focused on identifying the **dominant upper-level circulation pattern** associated with **extreme air-pollution days in Mexico City (CDMX)**, using **500-hPa geopotential height composites** from NARR reanalysis (2012–2024).  
The work improves the Week 5 analysis by refining the code, applying daily climatological anomalies (H′), and linking results with literature from both **Mexico** and **Hong Kong**.

Due to time constraints, the additional 850 hPa analysis was not completed, but the 500 hPa composites provide robust insights into the **ridge–stagnation regime** controlling polluted episodes in the MCMA.

---

## Structure

📂 week6
┣ 📜 README.md
┣ 📜 notebook_week6.ipynb
┣ 📜 see4994_week6.pdf ← Final presentation (Week 6)
┗ 📂 docs
┣ 📜 references_and_notes_week6.md
┗ 📜 research_question_week6.md


---

## Data sources and processing

- **Pollutant data:**  
  Derived from the Week 5 cleaned dataset (`cdmx_citymean_daily_2012_2024.csv`), originally processed from *aire.cdmx.gob.mx* official records.  
  Daily means were computed by averaging all active stations; missing days were handled via pandas interpolation.

- **Meteorological data (NARR):**  
  Accessed via *NOAA PSL THREDDS* using lazy downloading to concatenate monthly NetCDFs.  
  Variables: `hgt`, `uwnd`, `vwnd` at 500 hPa (2012–2024).  
  Daily climatologies were built with a 31-day rolling mean to smooth seasonal cycles.

- **Code origin and adaptation:**  
  The improved composite method was inspired by a script shared by a PhD student from the  
  **Climate Extreme Laboratory (School of Energy and Environment, City University of Hong Kong)**, supervised by **Prof. Jung-Eun Chu**.  
  Her approach was adapted and rewritten to fit the Mexico City dataset, resulting in clearer anomaly maps and more accurate ridge detection.

---

## Main results and conclusions

- A **persistent mid-tropospheric ridge** dominates over central Mexico during high-pollution days.  
- The ridge is characterized by **positive geopotential height anomalies (H′ ≈ +4 – 6 m)** and **weak ENE flow (1 m s⁻¹)** over the MCMA.  
- This regime produces **subsidence and thermal stability**, trapping pollutants in the basin.  
- The pattern aligns with previous studies (Díaz-Esteban 2022; Silva-Quiroz 2019; Jáuregui 1992).  
- Comparative analysis shows that while CDMX episodes are **home-grown under ridging**, Hong Kong’s are **cyclone- and monsoon-modulated**.  
- These findings link the Valley of Mexico’s geography and upper-level dynamics to its recurring air-quality crises.

---

## Files and reproducibility

To ensure privacy and size limits:
- Raw CSVs and NetCDFs are **not included** in this repository.  
- All figures are available in the Week 6 presentation (`see4994_week6.pdf`); screenshots may be freely used with citation.  
- Anyone interested in the datasets may contact me directly.

---

## Acknowledgements

Special thanks to **Prof. Jung-Eun Chu** and the **Climate Extreme Laboratory** for methodological guidance, and to NOAA PSL and AIRE CDMX (Mexico) for providing open-access data.

---

© 2025 Erick Rico Esparza  
Master’s Programme in Environmental Engineering, Tampere University  
Exchange semester at City University of Hong Kong
