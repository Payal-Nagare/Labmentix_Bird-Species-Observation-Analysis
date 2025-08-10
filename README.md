# Bird Species Observation Analysis

## Project Overview
This project analyzes bird species observations across forest and grassland ecosystems using Python.  
The dataset contains detailed records of bird sightings, environmental conditions, observer details, and species information.

The workflow includes data cleaning, preprocessing, exploratory data analysis (EDA), and generating insights about biodiversity trends, observation patterns, environmental correlations, and species conservation status.

---

## Objectives
- Merge and clean multi-sheet Excel datasets for forests and grasslands.
- Explore seasonal, temporal, and spatial trends in bird sightings.
- Identify biodiversity hotspots and dominant species.
- Analyze bird activity patterns, weather impact, and disturbance effects.
- Detect observer bias and evaluate conservation priorities.

---

## Dataset
Two Excel datasets:
- Bird_Monitoring_Data_FOREST.XLSX (multiple sheets)
- Bird_Monitoring_Data_GRASSLAND.XLSX (multiple sheets)

**Key columns:**
- `Scientific_Name`, `Common_Name`, `Location_Type`
- `Date`, `Start_Time`, `End_Time`
- `Temperature`, `Humidity`, `Sky`, `Wind`
- `ID_Method` (observation method), `Sex`
- `PIF_Watchlist_Status`, `Regional_Stewardship_Status`
- `Distance`, `Observer`, `Visit`

---

## Tools & Libraries
- Python 3
- pandas — Data manipulation
- numpy — Numerical operations
- matplotlib & seaborn — Visualization
- mysql.connector — (Optional) MySQL integration

---

## Analysis Performed
1. Data Loading & Merging  
   - Combine all sheets for each ecosystem.  
   - Merge forest and grassland datasets.  

2. Data Cleaning & Preprocessing  
   - Handle missing values.  
   - Convert dates/times to proper formats.  
   - Fill gaps with logical defaults.  

3. Seasonal Trends  
   - Map months to seasons.  
   - Count bird sightings per season/year.  

4. Observation Time Patterns  
   - Group sightings into time windows.  
   - Identify peak activity periods.  

5. Location Hotspots  
   - Top species per `Location_Type`.  
   - Most active `Plot_Name`s.  

6. Biodiversity Metrics  
   - Unique species counts by habitat.  

7. Activity Patterns  
   - Most common behaviors (e.g., singing).  

8. Sex Ratio Analysis  
   - Male-to-female observation counts per species.  

9. Weather Correlation  
   - Relationship between temperature, humidity, and bird counts.  

10. Disturbance Effects  
    - How disturbances affect sightings.  

11. Flyover Trends  
    - Patterns in `Flyover_Observed`.  

12. Observer Bias  
    - Which observers record the most sightings.  

13. Visit Patterns  
    - Impact of repeated visits on sightings and diversity.  

14. Conservation Watch  
    - Species flagged in watchlists or stewardship programs.

---

## Example Insights
- Peak activity occurs in early mornings (5 AM – 9 AM).  
- Spring and summer see the highest bird counts.  
- Certain plots consistently record higher biodiversity.  
- Humidity and wind conditions influence sightings.  
- Some observers report disproportionately more species — indicating possible bias.  
- Species on PIF watchlists align with high stewardship priority.  

---

## Project Structure
```
├── Bird_Monitoring_Data_FOREST.XLSX
├── Bird_Monitoring_Data_GRASSLAND.XLSX
├── Birds_forest.xlsx
├── Birds_Grassland.xlsx
├── Merged Data.csv
├── Visit.csv
├── bird_species_analysis.py   # Main Python script
└── README.md

## Possible Extensions
- Build interactive dashboards with Power BI or Streamlit.  
- Integrate geographic mapping for species distribution.  
- Connect to MySQL for scalable storage and querying.  
- Apply machine learning models for species prediction.

---

## Skills Demonstrated
- Data Cleaning & Transformation  
- Exploratory Data Analysis (EDA)  
- Statistical Summaries  
- Data Visualization  
- Environmental Data Interpretation  
- Database Integration
