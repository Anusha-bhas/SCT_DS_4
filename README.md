# Accident Data Analysis: Patterns and Hotspots 🚨

This repository contains a Jupyter Notebook (`skillcraft-4.ipynb`) for **Exploratory Data Analysis (EDA)** on a road accident dataset. The analysis aims to identify **patterns in accident frequency** and **geographical hotspots** to inform safety interventions.

## ⚠️ Data Requirement

* **Input File:** This notebook requires a file named `Accident.csv` (or similar, as indicated by the code structure) containing accident data, including columns for:
    * **Start\_Time** (or similar timestamp)
    * **Latitude** and **Longitude**
    * **Weather\_Condition**
    * **Road\_Condition**

## ⚙️ Analysis and Feature Engineering

The initial data preparation included:

* **Time Conversion:** Converting the `Start_Time` column to a datetime object.
* **Time Features:** Extracting the **Hour** and **Day\_of\_Week** from the timestamp for time-series analysis.
* **Data Cleaning:** Standardizing the case of categorical columns (`Weather_Condition` and `Road_Condition`) for consistent counting.

## 📊 Key Visualizations (Intended Output)

The analysis generates three primary bar charts to understand contributing factors, and one interactive map for spatial analysis.

### 1. Temporal & Environmental Patterns

| Analysis | Description | Intended Output File |
| :--- | :--- | :--- |
| **Accident Frequency by Hour** | Shows when accidents are most likely to occur throughout the day (e.g., rush hour peaks). | `accident_frequency_by_hour.png`  |
| **Accident Frequency by Weather** | Visualizes which weather conditions are most frequently associated with accidents. | `accident_frequency_by_weather.png`  |
| **Accident Frequency by Road** | Identifies the most common road surface conditions (e.g., Dry, Wet) during accidents. | `accident_frequency_by_road.png`  |

### 2. Geographical Hotspots

* **Interactive Map:** An interactive **HeatMap** is generated using the `folium` library to visualize the density of accidents. Denser areas on the map indicate high-risk accident hotspots.
* **Intended Output File:** `accident_hotspots_map.html` ```

Would you like to try to resolve the `FileNotFoundError` or explore a different notebook's contents?