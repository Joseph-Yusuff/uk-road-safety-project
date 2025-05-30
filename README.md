# 🚦 UK Road Safety & Accident Prediction Project (2020)

## 📌 Objective
To support UK government agencies in improving road safety by:
- Mining STATS19 road accident data for key patterns.
- Modeling and forecasting accident occurrences using time series.
- Uncovering accident-prone locations using clustering.
- Extracting hidden associations using rule mining.
- Evaluating social influence using social network analysis.

## 📊 Tools Used
- **Python:** pandas, scikit-learn, statsmodels, networkx, folium
- **Power BI:** Interactive dashboards
- **Jupyter Notebook:** Exploratory and modeling notebooks
- **SQLite3:** For database storage
- **Geospatial Libraries:** geopandas, shapely

## 📁 Structure
| Folder | Description |
|--------|-------------|
| `data/` | Raw and processed STATS19 datasets |
| `notebooks/` | Jupyter notebooks for each analytical task |
| `dashboards/` | Power BI visuals |
| `figures/` | Static images used in documentation and markdown |

## 📌 Key Analyses
### Q1–Q4: Exploratory Patterns
- Hourly and daily accident trends
- Road user type distribution

### Q5: Clustering Hotspots
- Applied KMeans & DBSCAN on spatial coordinates
- Visualized clusters using scatter plots, KDE heatmaps, and Folium maps

### Q6: Weekly Forecasts
- SARIMA and Prophet models for accident counts in major cities

### Q7: Daily LSOA-level Forecasting
- Forecasts for Hull LSOAs with model evaluation (MAE, RMSE)

### Q8–Q10: Social Network Analysis
- Edge centrality, bridge detection
- Community detection: Girvan–Newman vs Louvain

## 📸 Dashboards (Power BI)
- Accident distribution by hour/day
- Motorcycle and pedestrian accidents by time and severity
- Integrated accident forecasts

> 📂 See `/dashboards/` for visuals in compressed PDF version of Power BI dashboard for portfolio sharing (full .pbix exceeds GitHub limit).

## 📌 Project Highlights
- 📈 **Forecasting accuracy evaluated with MAE, RMSE, Coverage**
- 🧠 **High-performance modeling with SARIMA tuning and `auto_arima`**
- 🗺️ **Geospatial clustering with KDE and Folium**
- 🌐 **Network community detection and centrality measures**
- 📊 **Professional-grade Power BI Dashboards**

## Run Locally
bash
# Create a virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt

# Launch the notebook
jupyter notebook
