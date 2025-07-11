
##  Objective

The purpose of this lab is to apply data exploration, visualization, preprocessing, and statistical analysis techniques on the `Walmart_Sales` dataset using Python in a Jupyter Notebook. This exercise demonstrates practical skills in cleaning, analyzing, and drawing insights from real-world data.

---

##  Dataset Information

- **Name:** Walmart_Sales.csv  
- **Attributes:**
  - Store
  - Date
  - Weekly_Sales
  - Holiday_Flag
  - Temperature
  - Fuel_Price
  - CPI
  - Unemployment

---

##  Key Tasks Performed

###  Step 1: Data Collection
- Loaded dataset using Pandas.
- Parsed and cleaned corrupted dates.
- Displayed the first few rows for inspection.

###  Step 2: Data Visualization
- **Scatter Plot:** Visualized the relationship between Weekly Sales and Temperature.
- **Line Plot:** Displayed trends in Weekly Sales over time.
- **Insights:** Observed seasonal trends and temperature influence on sales.

###  Step 3: Data Preprocessing
- **Missing Values:** Identified and handled using mean and forward fill techniques.
- **Outlier Detection:** Used IQR method to find and remove outliers from Weekly Sales.
- **Data Reduction:** Applied sampling (30%) and removed less relevant columns like Fuel_Price.
- **Scaling:** Applied Min-Max Scaling to numeric variables.
- **Discretization:** Converted Temperature into categorical bins (Cold, Mild, Hot).

###  Step 4: Statistical Analysis
- Explored dataset using `.info()` and `.describe()`.
- Calculated central tendency: min, max, mean, median, mode.
- Calculated dispersion: range, IQR, variance, standard deviation.
- **Correlation Analysis:** Generated correlation matrix and heatmap for numeric attributes.

---

##  Key Insights

- Outliers were significantly impacting weekly sales data and were cleaned.
- There’s no strong linear correlation between Weekly Sales and CPI/Unemployment.
- Weekly sales show trends that may correlate with seasonal patterns.
- Data visualization helped identify patterns that are not obvious from raw numbers.

---

##  Challenges & Decisions

- Some date values were malformed and required parsing with `errors='coerce'`.
- Decision made to fill missing CPI and Unemployment with column mean.
- Outliers removed based on IQR to improve analysis quality.

---
