![Python](https://img.shields.io/badge/Python-3.10%2B-blue)
![pandas](https://img.shields.io/badge/pandas-%23150458.svg)
![numpy](https://img.shields.io/badge/numpy-%23013243.svg)
![matplotlib](https://img.shields.io/badge/matplotlib-%23ffffff.svg)
![seaborn](https://img.shields.io/badge/seaborn-%23007396.svg)
![plotly](https://img.shields.io/badge/plotly-%2300407A.svg)
![folium](https://img.shields.io/badge/folium-Geo-green)
![DBSCAN](https://img.shields.io/badge/sklearn-DBSCAN-orange)

<h2>📊 Crime Incidents Analysis 2024</h2>

A Data Processing & Exploratory Data Analysis (EDA) Project.  
This project focuses on analyzing crime incidents reported in 2024 using a real-world dataset containing geospatial, temporal, and categorical crime information.  
The goal is to clean, process, visualize, and derive insights about crime patterns using Python data analysis techniques.

---

<h3>📁 Dataset Overview</h3>

- Dataset: Crime_Incidents_in_2024.csv  
- Rows: ~25,000 incidents  

**🔍 Key Columns**

| Column                                 | Description                                               |
|----------------------------------------|-----------------------------------------------------------|
| `REPORT_DAT`                           | Date & timestamp of the incident                          |
| `SHIFT`                                | Duty shift (DAY, EVENING, MIDNIGHT)                       |
| `OFFENSE`                              | Type of crime (THEFT, MOTOR VEHICLE THEFT, ROBBERY, etc.) |
| `METHOD`                               | Crime method (GUN, KNIFE, OTHERS…)                        |
| `LATITUDE`, `LONGITUDE`                | Geospatial coordinates                                    |
| `BLOCK`, `BLOCK_GROUP`, `CENSUS_TRACT` | Location identifiers                                      |
| `START_DATE`, `END_DATE`               | Time window of the incident                               |

---

<h3>🧪 Notebook Included</h3>

**DataProcessing & EDA.ipynb**  
This notebook covers:

- **Data Cleaning:** handled missing coordinates, fixed datetime formats, standardized categories.  
- **Exploratory Analysis:** crime distribution across shifts, top offenses, temporal patterns, and clustering (DBSCAN).  
- **Geospatial Visualization:** mapped crime locations and highlighted high-density hotspots using Folium.  

---

<h3>📌 Key Insights from EDA</h3>

- Theft-related crimes (THEFT/OTHER, THEFT F/AUTO) dominate reported incidents.  
- Crime patterns vary significantly across shifts:  
  - **DAY:** more theft reports  
  - **EVENING:** more street-level crimes  
  - **MIDNIGHT:** lower volume but higher-risk categories  
- Geospatial analysis reveals clear hotspot clusters in specific urban zones.  

---

<h3>🗺️ Visualizations Included</h3>

- Crime distribution bar charts  
- Monthly trend line plots  
- Heatmaps of offense frequency  
- Interactive Folium crime map  
- DBSCAN cluster map  

---

[🌍 View Interactive Crime Cluster Map](https://akhilaulpara.github.io/Crime-Incidents-Analysis-2024/crime_clusters_map.html)

<img width="1920" height="1080" alt="Image" src="https://github.com/user-attachments/assets/7e12473a-1aba-4497-ada8-1bdb0d7b74f7" />
- GitHub does not run JavaScript or interactive HTML inside Jupyter notebooks, so Folium maps (which are rendered using HTML + JavaScript) cannot be displayed directly in the .ipynb preview.
- Because of this limitation, the interactive map does not appear even if the notebook is trusted.
- To ensure the map is still accessible, the Folium output is exported separately as an HTML file
- This standalone file preserves the full interactivity of the map and can be opened directly in a browser or viewed through GitHub Pages.
