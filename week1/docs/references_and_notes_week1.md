# 📚 References & Notes – Week 1 (Sept 4–11)

## Hong Kong

### Papers
- **Luo, M., Hou, X., Gu, Y., Lau, N., & Yim, S. H. (2017). Trans-boundary air pollution in a city under various atmospheric conditions. The Science of the Total Environment, 618, 132–141. https://doi.org/10.1016/j.scitotenv.2017.11.001**  
  *Trans-boundary air pollution in a city under various atmospheric conditions* - https://www.sciencedirect.com/science/article/pii/S0048969717330590?via%3Dihub
    - Transboundary air pollution (TAP) is the major contributor to PM10, PM2.5, SO₂, and NO₂ in Hong Kong (2002–2013).
    - Seasonal pattern: winter concentrations higher than summer, especially for PM10 and PM2.5.
    - Roadside peaks at 8–9 am and 6–8 pm highlight strong local traffic emissions.
    - Marine vessels and power plants are key local SO₂ and NO₂ sources alongside TAP.
    - Approaching tropical cyclones increase TAP by 17–46% due to stronger northerly winds and reduced precipitation.

- **Zeng, S., Chu, J., Cheung, H. M., Baek, K., Kim, H., & Son, J. (2025). Seasonal Variations in PM2.5 levels in Hong Kong Induced by Eastern and Western Tropical Cyclones. Atmospheric Environment, 121497. https://doi.org/10.1016/j.atmosenv.2025.121497**:
  *Seasonal variations in PM2.5 levels in Hong Kong induced by tropical cyclones* - https://www.sciencedirect.com/science/article/pii/S1352231025004728?via%3Dihub
    - Eastern TCs increase summer (JJA) PM2.5 in Hong Kong by ~94%, while western TCs reduce it by ~38%.
    - In autumn (SON), impacts weaken to +30% (east) and −10% (west), due to high background PM2.5 and weaker subsidence.
    - East TCs bring northerly winds, subsidence, and surface warming that trap pollutants and enhance fine aerosols.
    - West TCs introduce moist southerly winds and rainfall, improving ventilation and pollutant removal.
    - Aerosol optical data show east TCs favor larger fine-mode particles, while west TCs favor ultrafine aerosols.

### Links (HK)
- [Personalized consult - EPD HK](https://cd.epic.epd.gov.hk/EPICDI/air/station/?lang=en) – hk_air_cb_tm_202401.csv: PM2.5, PM10, NO₂, O₃ (Causeway Bay/Tap Mun), January 2024
- [AQHI](https://www.aqhi.gov.hk/en/past-data/past-aqhi.html) – hk_aqhi_202401.csv: Past AQHI, January 2024

---

## Mexico City

### Papers
- **González, I. G., Nepamuceno, D. M. C., Cruz, D. G., & Vergara, E. A. (2020). Correlación entre diferentes contaminantes atmosféricos de la Ciudad de México y el Área Metropolitana. CIENCIA Ergo Sum, 27(3), e95. https://doi.org/10.30878/ces.v27n3a5**:
  *Correlation between different air pollutants in Mexico City and the Metropolitan Area*  - https://www.ssoar.info/ssoar/handle/document/71212
    - Data from RAMA (2017) used for gases (SO₂, CO, NO, NO₂, O₃, NOx) and particles (PM2.5, PM10, PMcoarse).
    - Strong intra-station correlations: NO₂–NOx, NO–NOx, CO–NO, CO–NOx.
    - Particulate correlations: PM2.5–PM10 and PMcoarse–PM10 highly dependent.
    - Ozone showed strong correlation across different stations.
    - Highlights co-variation patterns useful to understand pollutant interactions.

- **Cruz-Huerta, C., Martínez-Trinidad, T., Correa-Díaz, A., Gómez-Guerrero, A., Vargas-Hernández, J. J., Villanueva-Díaz, J., & Beramendi-Orosco, L. E. (2023). Modelado espacial y temporal de contaminantes atmosféricos en la Zona Metropolitana de la Ciudad de México. Revista Chapingo Serie Ciencias Forestales Y Del Ambiente (En Línea)/Revista Chapingo Serie Ciencias Forestales Y Del Ambiente, 30(1), 1–18. https://doi.org/10.5154/r.rchscfa.2023.02.010**:
  *Spatial and temporal modeling of air pollution in Mexico City Metropolitan Area* - https://www.scielo.cl/scielo.php?pid=S0718-07642025000400021&script=sci_arttext
    - Analyzed NOx, CO, O₃ (1986–2021), PM10 (2000–2021), PM2.5 (2003–2021) across 44 Automatic Air Monitoring Network (RAMA) stations.
    - Seasonal peaks: NOx/CO in winter, O₃ in April–May, PM in dry season.
    - All pollutants showed long-term declines, most pronounced for NOx (−1.28 ppb/yr).
    - High correlations among NOx, CO, PM10, PM2.5; weaker for O₃ with PM.
    - Support Vector Machine outperformed Kriging, Random Forest, and Neural Network in spatial modeling.

- **Arganis, M., & Preciado, M. (2025). Análisis de frecuencias de los índices IMECA máximos horarios anuales del noroeste de la Ciudad de México. InformacióN TecnolóGica, 36(4), 21–30. https://doi.org/10.4067/s0718-07642025000400021**:
  *Frequency analysis of annual maximum hourly IMECA indices in northwest Mexico City* - https://www.scielo.cl/scielo.php?pid=S0718-07642025000400021&script=sci_arttext
    - Analyzed annual maximum IMECA indices (1992–2022) for O₃, CO, NO₂, SO₂, PM10 in NW Mexico City.
    - PM10 series homogeneous and random; SO₂ non-homogeneous but probabilistic (Gumbel).
    - O₃, CO, NO₂ non-homogeneous and dependent → require deterministic models.
    - Pettit test detected significant change points between 2004–2006 (linked to policy shifts).
    - Emphasizes statistical tools for predictive modeling and policy evaluation.

### Links (MC)
- [Consulta personalizada (estación/contaminante)](https://www.aire.cdmx.gob.mx/default.php?opc=%27aqBhnmQ=%27) – mc_CAM_MER_PED_202401.csv, hourly, Jan 2024
- [Índice de Aire y Salud](http://datosabiertos.aire.cdmx.gob.mx:8080/Opendata/ias/IAS_2024.csv)/(https://www.aire.cdmx.gob.mx/default.php?opc=%27aKBhnmI=%27&opcion=ZmU=) - mc_IAS_2024.csv: hourly, 2024
- [Consulta visual](https://www.aire.cdmx.gob.mx/default.php?opc=%27aqBhnmOkZA==%27)

---

## General Context
- Hong Kong: PM2.5 and TCs → clear seasonal modulation.
- Mexico City: Air & Health Index (ex-IMECA), correlations between pollutants, spatial/temporal modeling.
- Comparability: AQHI (Hong Kong) vs Air & Health Index (Mexico City).
- Week 1: Download raw datasets → cleanup + basic graphics.

---

## Notes on datasets:

### Hong Kong pollutants (hk_air_cb_tm_202401.csv)
- On VS Code (hk_pollutants_clean.csv):
  - Skipped first 11 rows
  - Converted 'DATE' to datetime with dayfirst=True.
  - Renamed columns.
  - Converted columns to float64, coercing errors.
  - The 'Hour' column remained as is (object).
  - Filled NaN of pollutants with daily average.
  - Applied rolled windows.
  - Exported clean CSV for future notebooks.

### Hong Kong AQHI (hk_aqhi_202401.csv)
- Manual cleaning due to some errors on VS Code (hk_aqhi_202401 - copia.csv): filled empty dates, removed rows with "Daily Max", converted to datetime, removed asterisks, filled NaN with daily mean, kept only the columns of interest, removed first 7 rows.
- On VS Code (hk_aqhi_clean.csv): converted some columns to float on VS Code, exported clean CSV for future notebooks.

### Mexico City pollutants (mc_CAM_MER_PED_202401.csv)
- Manual cleaning due to some errors on VS Code (mc_CAM_MER_PED_202401 - copia): concatenated 3 blocks of data per station, renamed columns, trimmed spaces in DATE column.
- On VS Code (mc_pollutants_clean.csv): dropped last row, converted DATE column to datetime, filled NaN of contaminants with daily average, applied rolled windows, exported clean CSV for future notebooks.

### Mexico City Air and Health Index (mc_IAS_2024.csv)
- On VS Code (mc_ias_clean):
  - Skipped first 9 rows.
  - Renamed columns.
  - Used ordinal mapping (1–5) of IAS categories for comparability with AQHI; future work could integrate numeric ICA data per pollutant/region.
  - Area of opportunity: Homogenize Mexican indices to make them directly comparable with those of Hong Kong.
  - Converted column DATE to datetime.
  - Exported clean CSV for future notebooks.

---

## Presentation made on Canva (see4994_week1.pdf)
- Output tables and plots obtained from week notebook (notebook_week1.ipynb).

### Links to presentation images:
- https://www.scmp.com/news/hong-kong/health-environment/article/3280562/hong-kong-air-pollution-reaches-serious-levels-parts-city-amid-weak-winds
- https://politica.expansion.mx/cdmx/2024/05/16/contingencia-ambiental-jueves-16-de-mayo-2024#uuid0000018f-86da-deea-afbf-9fda6ea80000
- https://www.britannica.com/place/Hong-Kong
- https://www.researchgate.net/figure/Map-of-the-16-local-governments-of-Mexico-City-Created-by-the-first-author-from-public_fig1_378783261
