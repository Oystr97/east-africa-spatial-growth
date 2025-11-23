## East Africa Demographic Shifts: Spatial Analysis (2015-2025)

![Population Change Map](notebook/images/population_change_2015_2025.png)

### 🌍 Project Overview
This project leverages geospatial data to analyze population growth patterns across **Uganda, Rwanda, Burundi, and Tanzania**. By classifying demographic shifts into Decline, Neutral, Growth, and High Growth categories, this analysis aids in identifying urbanization hotspots and resource allocation needs.

### 📊 Key Geographic Insights
Based on the spatial analysis output (Map 2):
*   **High-Density Growth:** Intense population pressure ("High Growth") is concentrated in the **Lake Victoria basin**, particularly impacting **Rwanda, Burundi, and Southern Uganda**.
*   **Urbanization Corridors:** Tanzania exhibits a more dispersed growth pattern, with distinct clusters likely correlating with major urban centers and transit corridors.
*   **Population Decline:** Specific pockets of population decline (Green) were identified, potentially indicating migration out of protected areas or rural-to-urban shifts in the Southern Highlands of Tanzania.

### 🛠️ Tech Stack & Methods
*   **Tools:** Python (Geopandas, Rasterio, Matplotlib), QGIS (for final cartography).
*   **Data Source:** WorldPop / National Census Projections.
*   **Methodology:**
    1.  Raster calculation to determine pixel-wise population change.
    2.  Reclassification of growth rates into categorical tiers.
    3.  Cartographic layout with scale bar (EPSG:xxxx) and North orientation.

### 🚀 How to Run the Analysis
1.  Clone the repository:
    ```bash
    git clone https://github.com/Oystr97/East-African-demographic-shifts-in-population-size-distribution-and-growth-patterns.git
    ```
2.  Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3.  Run the Jupyter Notebook:
    ```bash
    jupyter notebook notebooks/analysis.ipynb
    ```
### 📊 Data Sources
The datasets used in this project were downloaded from the following sources:
- **ICPAC Geoportal** (African Administrative Boundaries)
  - [https://geoportal.icpac.net/](https://geoportal.icpac.net/)
- **WorldPop** (Global Demographic Data)
  - [https://www.worldpop.org/](https://www.worldpop.org/)
- **Nature Scientific Data** (Urban form and functions data)
  - [https://doi.org/10.1038/s41597-020-00605-z](https://doi.org/10.1038/s41597-020-00605-z)
- **United Nations Population Division** (World Population Prospects 2022)
  - [https://population.un.org/wpp/](https://population.un.org/wpp/)
- **The World Bank Open Knowledge Repository** (Africa's Cities)
  - [https://openknowledge.worldbank.org/](https://openknowledge.worldbank.org/)
