# Unofficial GTFS Feed: Metropolitano (Lima, Peru)
This repository contains the **gtfs lima** feed, a structurally valid but unofficial General Transit Feed Specification (GTFS) dataset for the Metropolitano bus rapid transit system in Lima.
### Disclaimer
This is **not an official resource**. This feed was independently generated for research and structural testing purposes. It is not affiliated with, endorsed by, or maintained by the Autoridad de Transporte Urbano (ATU) or any official transit agency.
### Data Sources and Methodology
The data used to build this feed was scraped and reverse-engineered from an independent, non-standardized informational website (metrolima.net). Because the source material was unstructured text rather than a native public dataset, several adaptations were made to force compliance with the GTFS standard:
* **Route & Stop Inventories:** Extracted manually from text descriptions and HTML lists detailing the regular (A, B, C, D) and express routes.
* **Geospatial Data:** Exact latitude and longitude coordinates for stations were not provided by the source and were approximated to satisfy basic validator requirements.
* **Timetables:** Minute-by-minute stop times (`stop_times.txt`) were synthesized using total travel times and general headway frequencies to ensure structural compliance, rather than representing exact real-world schedules[cite: 1, 6, 7].
For official data, service alerts, or direct inquiries, please consult the ATU directly at https://www.gob.pe/atu.