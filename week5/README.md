# 🌎 SEE4994 – Week 5 (Oct 18 – 27)
## Synoptic Patterns and Pollutant Events (2012–2024)

### 🎯 Objective
This week focused on linking **large-scale atmospheric circulation** with **pollution extremes over Mexico City (CDMX)**.  
Using **NARR reanalysis data** (NOAA – ESRL/PSL) and my cleaned pollutant dataset (Week 2), I analyzed how **geopotential height anomalies (HGT′)** and **wind patterns** behave during the most polluted days.

---

### 📦 Datasets Used
| Dataset | Description | Source |
|----------|--------------|---------|
| `cleaned_cdmx_air_2012-2024.csv` | Daily mean concentrations of NO₂, O₃, PM₁₀, PM₂.₅, SO₂ for CDMX (2012–2024) | Self-processed (Week 2) |
| NARR – Daily Pressure Levels | 500 hPa & 850 hPa geopotential height (hgt), zonal wind (uwnd), meridional wind (vwnd) | [NOAA PSL – NARR Dailies](https://downloads.psl.noaa.gov/Datasets/NARR/Dailies/pressure/) |

> ⚠️ Note: I did **not** download full NetCDF files (≈ 80 GB).  
> The workflow used **lazy access and subsetting via `xarray`**, retrieving only the needed variables, levels, and bounding box.

---

### 🧠 Process Overview
1. **Data availability check:** verified month-by-month URLs (2012–2024) to confirm NARR continuity — official documentation said data stopped at 2014, but all monthly files loaded successfully ✅.  
2. **Subset extraction:** limited the spatial domain to **Central Mexico / MCMA**, combining 13 years × 3 variables × 2 levels (≈ 4750 days per level).  
3. **Event selection:** used the top 10 % (P90) of pollutant concentrations per month to define “event days.”  
4. **Composites:** computed mean 500 hPa and 850 hPa geopotential height (HGT), its anomalies (HGT′), and mean wind vectors (U,V) for those events vs climatology.  
5. **Significance:** pixelwise *t-tests* (p < 0.05) marked with stippling.  
6. **Visualization:**  
   - Individual maps per pollutant  
   - 2×3 multipanel layout for 850 hPa  
   - Histograms showing pollutant distributions + P90 thresholds

---

### 🕒 Execution Notes
- Each composite run (2012–2024) took **a few hours** on a personal laptop (i5 CPU + 16 GB RAM).  
- Results are preliminary — several areas (e.g., vector scaling, colormap tuning, zoom level) will be refined in later weeks.

---

### 🖼️ Outputs
All figures and code are in the accompanying notebook:  
**`notebook_week5.ipynb`** and presentation **`see4994_week5.pdf`**

- 500 hPa composite maps (per pollutant)  
- 850 hPa composite maps + 2×3 panel layout  
- Histograms of pollutant distributions (with P90 lines)

> Figures are original outputs generated from my code.  
> Feel free to reuse them with proper credit (mention of author and week/project).  
> No need to request permission.

---

### 🗣️ Personal Note
This was my most technically demanding week so far — combining **xarray, dask, cartopy, and scipy** for the first time.  
Execution was slow and imperfect, but this exercise helped me deeply understand:
- How synoptic patterns connect to local pollution, and  
- How to work with reanalysis datasets efficiently.

This is **not my final work**, but a learning step toward a cleaner, automated pipeline for future comparisons (e.g., Mexico City ↔ Hong Kong).

---
