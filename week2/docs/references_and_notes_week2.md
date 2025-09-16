# 📚 References & Notes – Week 2 (Sept 12–17)

## Hong Kong

### Links (HK)
- [Personalized consult – EPD HK](https://cd.epic.epd.gov.hk/EPICDI/air/parameter/) – Pollutants: PM10, PM2.5, O₃, NO₂, SO₂;  
  **Stations (2012–2024):** CENTRAL/WESTERN, EASTERN, KWUN TONG, SHAM SHUI PO, SHATIN, TAI PO, TAP MUN, TSUEN WAN, TUNG CHUNG, YUEN LONG.  
  *Roadside stations excluded; selected stations based on lower proportion of missing values (NaNs) and more spatial coverage across the territory.*
- [AQ objectives – HK](https://www.epd.gov.hk/epd/english/environmentinhk/air/air_quality_objectives/air_quality_objectives.html) – air pollutant limits and objectives.
- [AQHI info](https://www.aqhi.gov.hk/en/what-is-aqhi/about-aqhi.html) – description of AQHI system.
- [Past AQHI](https://www.aqhi.gov.hk/en/past-data/past-aqhi.html) – historical AQHI data.
- [Station network](https://www.aqhi.gov.hk/en/monitoring-network/air-quality-monitoring-stations.html) – classification of stations (urban, new town, rural).
- [Altitude tool](https://www.advancedconverter.com/es/herramientas-de-mapa/encontrar-altitud-desde-coordenadas) – used for extracting altitudes of HK stations.

---

## Mexico City

### Links (MC)
- [Personalized consult – AIRE CDMX](https://www.aire.cdmx.gob.mx/default.php?opc=%27aqBhnmQ=%27) – Pollutants: PM10, PM2.5, O₃, NO₂, SO₂;  
  **Stations (2012–2024):** AJUSCO MEDIO, CAMARONES, HOSPITAL GENERAL DE MEXICO, MERCED, MIGUEL HIDALGO, PEDREGAL, SAN AGUSTIN, TLALNEPANTLA, UAM IZTAPALAPA, XALOSTOC.  
  *Stations selected because they consistently contained all 5 pollutants within the available period (2012–2024).*
- [IAS info](https://www.aire.cdmx.gob.mx/default.php?opc=%27ZaBhnmI=&dc=%27Zw==) – documentation of IAS categories and recommendations.
- [IAS data (historical)](https://www.aire.cdmx.gob.mx/default.php?opc=%27aKBhnmI=%27&opcion=ZmU=) – historical IAS data.
- [Monitoring stations list](https://www.aire.cdmx.gob.mx/default.php?opc=%27ZaBhnmI=&dc=%27ZA==) – official station catalog.
- [Station map (official)](https://www.aire.cdmx.gob.mx/default.php?opc=%27ZaBhnmM=%27) – interactive location map.
- [Repositorio CONACYT](https://repositorio-salud.conacyt.mx/jspui/handle/1000/235) – metadata for stations (coordinates, altitude).

---

## Notes on datasets

### Hong Kong pollutants
- Cleaning in VS Code:
  - Skipped first lines of raw files.
  - Dropped NaNs and ensured all pollutant columns converted to `int`.
  - Converted `DATE` column to datetime.
  - Concatenated two separate files to obtain the full 2012–2024 period.
  - Exported a combined dataset for analysis.

### Mexico City pollutants
- Excel cleaning:
  - Removed unnecessary columns and rows.
  - Renamed all pollutant/date columns; formatted DATE as short date.
  - Used cleaning tool to fix formatting of DATE column.
- VS Code cleaning: 
  - Dropped NaNs, converted pollutant columns to `int`, DATE to datetime, ensured no errors or NaT values.
  - Since portal only allows download per year for a max of 4 stations:
    - Repeated cleaning for each year and group of stations.
    - Concatenated yearly files per group of stations.
    - Exported group-of-stations-level datasets.
    - Finally concatenated all 10 selected stations (2012–2024) into one dataset ordered by DATE.

---

## Presentation (see4994_week2.pdf)
- Output tables and plots embedded directly from `notebook_week2.ipynb`.

### Links to presentation images:
- Google Maps (screenshots with custom markers for HK & MC stations): https://www.google.com/maps
