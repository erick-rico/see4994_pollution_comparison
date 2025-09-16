# Week 2 – Progress Report (Sept 12–17)

## 📌 Overview
Extended analysis of Hong Kong vs Mexico City air quality over a longer period (2012–2024). Focused on spatial patterns (urban vs rural/peripheral) and seasonal trends across five key pollutants. Prepared overview tables of monitoring stations and pollutants for both cities.  

## 📂 Contents
- `notebook_week2.ipynb` → full analysis (time series, distributions, spatial comparison, correlations, seasonal trends).  
- `see4994_week2.pdf` → slides for meeting.  
- `docs/` → references, sources, notes, week notebook & presentation.  
- **Note:** Raw/clean datasets and output plots are **not uploaded** due to size and preprocessing complexity. Data can be shared **upon request**.  

## 📊 Key Findings / Outputs
- **Temporal trends:** PM higher in Mexico City (especially winter/spring), O₃ higher in Hong Kong (autumn/spring).  
- **Distributions:** Mexico City shows broader and higher PM ranges; Hong Kong shows higher O₃ and NO₂.  
- **Spatial patterns:** Urban Mexico City → highest particulates; rural Hong Kong → highest ozone.  
- **Correlations:** PM₁₀ and PM₂.₅ strongly correlated; O₃ negatively correlated with NO₂ (particularly in HK).  
- **Seasonality:** PM and NO₂ peak in winter/spring; O₃ peaks in autumn (HK) and spring/summer (MC).  

## 🔜 Next Steps
- Integrate meteorological variables to explain critical episodes.  
- Develop a numerical version of Mexico City’s IAS and compare with Hong Kong AQHI.  
- Event-based analysis of extreme pollution episodes at specific stations.  

## 🧾 Useful Links (Data Sources & References)

### Hong Kong
- Data (pollutants): https://cd.epic.epd.gov.hk/EPICDI/air/parameter/  
- AQ objectives: https://www.epd.gov.hk/epd/english/environmentinhk/air/air_quality_objectives/air_quality_objectives.html  
- AQHI info: https://www.aqhi.gov.hk/en/what-is-aqhi/about-aqhi.html  
- AQHI past data: https://www.aqhi.gov.hk/en/past-data/past-aqhi.html  
- Station network (types/locations): https://www.aqhi.gov.hk/en/monitoring-network/air-quality-monitoring-stations.html  
- Altitude (tool): https://www.advancedconverter.com/es/herramientas-de-mapa/encontrar-altitud-desde-coordenadas  

### Mexico City
- Data (pollutants): https://www.aire.cdmx.gob.mx/default.php?opc=%27aqBhnmQ=%27  
- IAS index info: https://www.aire.cdmx.gob.mx/default.php?opc=%27ZaBhnmI=&dc=%27Zw==  
- IAS data (historical): https://www.aire.cdmx.gob.mx/default.php?opc=%27aKBhnmI=%27&opcion=ZmU=  
- Monitoring stations list: https://www.aire.cdmx.gob.mx/default.php?opc=%27ZaBhnmI=&dc=%27ZA==  
- Station map (official): https://www.aire.cdmx.gob.mx/default.php?opc=%27ZaBhnmM=%27  
- Repositorio CONACYT (stations, coords, altitudes): https://repositorio-salud.conacyt.mx/jspui/handle/1000/235  

## ❓ Research Question (living)
*How do pollutant characteristics and their spatial/seasonal patterns compare between Hong Kong and Mexico City (2012–2024), and what lessons can be drawn for air quality management in urban vs rural/peripheral contexts?*
