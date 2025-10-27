# 📚 References & Notes – Week 5 (Oct 18 – 27)

## 🧾 Datasets & Technical Docs
- **NOAA ESRL/PSL – NARR Dailies (Pressure Levels)**  
  https://downloads.psl.noaa.gov/Datasets/NARR/Dailies/pressure/  
  Variables used: `hgt`, `uwnd`, `vwnd` (500 hPa & 850 hPa)
- **Xarray Documentation** – multi-file lazy loading, coordinate operations  
  https://docs.xarray.dev/
- **Cartopy & Matplotlib** – projection, quiver, contour plotting  
  https://scitools.org.uk/cartopy/
- **SciPy – t-tests** for composite significance  
  https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.ttest_ind.html
- For **Mexico City dataset** please refer to *Week 2* references.

---

## 🧠 Concept Notes
- **Geopotential Height (HGT):** elevation of a pressure surface; higher HGT → warmer, expanded air column → high pressure.  
- **HGT′ (Anomaly):** deviation from smoothed daily climatology → reveals ridges (positive) and troughs (negative).  
- **500 hPa Level:** mid-troposphere ≈ 5.5 km — shows regional subsidence and synoptic flow.  
- **850 hPa Level:** lower troposphere ≈ 1.5 km — indicates low-level ventilation affecting pollutant dispersion.  
- **Stippling (p < 0.05):** areas where anomalies differ significantly from climatological mean.  
- **P90 selection:** days above the 90th percentile of pollutant concentration per month.

---

## 🔍 Related Literature
- **Silva-Quiroz et al. (2019)** – blocking highs (MAM) trigger O₃ contingencies.  
- **Díaz-Esteban et al. (2022)** – 30-year synoptic WPs; O₃ → spring, PM₂․₅ → winter; La Niña ↑ polluted patterns.
- ERA5 & NARR methodology papers for vertical wind and geopotential computations.

---

## 💬 Remarks
- Verified that NARR data exist beyond 2014 despite conflicting documentation.  
- Execution via `xarray.open_mfdataset` was memory-intensive — optimized with chunking and subsetting.  
- 850 hPa composites provided clearer low-level wind patterns than 500 hPa.  
- Execution times remain high; potential improvement: pre-download & cache NetCDF subsets locally.

---
