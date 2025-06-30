# ⚡ Electric Vehicle Specifications Power BI Dashboard (2025 Dataset)

## 📌 Project Title:  
**Analyzing Electric Vehicle Performance, Efficiency & Technical Specifications Using Power BI**

---

## 🧩 Project Objective

This Power BI dashboard project is designed to explore and visualize key attributes of Electric Vehicles (EVs) using the **Electric Vehicle Specifications 2025** dataset. The objective is to perform **in-depth analysis and storytelling** through visuals to answer ten open-ended analytical questions related to EV battery performance, efficiency, speed, torque, and more.

---

## 📂 Dataset Overview

- **Source**: [Kaggle - Electric Vehicle Specifications 2025](https://www.kaggle.com/datasets/urvishahir/electric-vehicle-specifications-dataset-2025)
- **Format**: CSV
- **Fields Included**:
  - Manufacturer / Brand
  - Battery Capacity (kWh)
  - Electric Range (km)
  - Acceleration (0–100 km/h)
  - Top Speed (km/h)
  - Total Torque (Nm)
  - Energy Consumption (Wh/km)
  - Battery Type
  - Number of Battery Cells
  - Motor Type
  - and more...

---

## 🧰 Tools & Technologies Used

| Tool/Technology | Purpose |
|-----------------|---------|
| **Power BI Desktop** | Visualization, analysis, dashboarding |
| **DAX** | Calculated fields and KPIs |
| **Python** | Cleaning, EDA, Integration |

---

## 🔍 Analytical Questions and Solutions

Below are the ten key questions addressed in the dashboard, along with the **approach**, **visuals**, and **insights** used to answer each.

---

### 1️⃣ Which manufacturers are offering the best balance of battery capacity and electric range?

- **Approach**:
  - Scatter Plot (X-axis: Battery Capacity, Y-axis: Electric Range)
  - Color-coded by Manufacturer

- **Visual**:
  - Custom scatter plot with data labels
  - Tooltip to show model name, range, and battery size

- **Insight**:
  - Brands like **Hyundai**, **Tesla**, and **BMW** stand out for offering longer ranges without disproportionately large batteries.
  - Ideal zone (high range, moderate battery) was highlighted in the scatter plot to identify optimal balance.

---

### 2️⃣ Does a higher battery capacity always result in a longer electric range?

- **Approach**:
  - Correlation analysis using a Scatter Chart + Trendline
  - R-squared value shown using a calculated field to express correlation strength

- **Visual**:
  - Scatter plot with linear regression line
  - Slicers for brand and battery type for deeper filtering

- **Insight**:
  - Positive correlation exists, but with exceptions.
  - Efficiency plays a role: some models have high capacity but underwhelming range due to poor energy consumption (Wh/km).

---

### 3️⃣ Which brands offer the fastest acceleration (0–100 km/h), and how does that relate to their torque values?

- **Approach**:
  - Bar Chart showing acceleration times sorted ascending (faster at top)
  - Overlay or tooltip showing Torque values

- **Visual**:
  - Combined Bar + Scatter (dual axis where needed)
  - Matrix view to compare multiple specs side-by-side

- **Insight**:
  - Brands like **Rimac**, **Lucid**, and **Tesla** dominate in acceleration.
  - Generally, higher torque correlates with better acceleration—but not always (weight & drivetrain also affect performance).

---

### 4️⃣ Comparison dashboard showing energy efficiency (Wh/km) across manufacturers

- **Approach**:
  - Average Wh/km by manufacturer using Bar Chart
  - Filters: Country, Brand, Battery Type

- **Visual**:
  - Column Chart for energy consumption
  - Conditional formatting to highlight most efficient

- **Insight**:
  - **Hyundai**, **Mini**, and **Renault** showed best Wh/km efficiency.
  - Larger vehicles (e.g., SUVs from Mercedes, Audi) consumed more Wh/km.

---

### 5️⃣ Analyze the relationship between total torque and top speed

- **Approach**:
  - Scatter Chart: X-axis = Torque, Y-axis = Top Speed
  - Trendline added to show correlation

- **Visual**:
  - Interactive Scatter Chart
  - Play Axis to see evolution per manufacturer

- **Insight**:
  - No strong linear correlation observed.
  - Some high-torque vehicles are limited in top speed due to safety/efficiency constraints.

---

### 6️⃣ Most common battery types and their average performance on key metrics

- **Approach**:
  - Group by Battery Type
  - Calculate averages: Range, Acceleration, Efficiency

- **Visual**:
  - Multi-row cards or Bar Charts
  - Category slicer for battery type

- **Insight**:
  - **Lithium-ion** is most dominant.
  - **Solid-state** batteries showed high efficiency but limited data points.

---

### 7️⃣ Which vehicle models deliver the best range with the least battery capacity (i.e., most efficient)?

- **Approach**:
  - Created a new calculated column: `Range per kWh = Electric Range / Battery Capacity`
  - Sorted models by this metric

- **Visual**:
  - Top 10 Most Efficient EVs – Bar Chart
  - Data Table with filters (manufacturer, type)

- **Insight**:
  - Models from **Hyundai Ioniq** and **BMW i3** stood out with high range/kWh values.
  - Efficiency is model-dependent, not just brand-dependent.

---

### 8️⃣ Are there any outliers in features like torque or acceleration?

- **Approach**:
  - Box plots and Scatter plots with tooltip outlier tags
  - Manual annotations for outliers

- **Visual**:
  - Scatter Plots with labeled outliers
  - Cards showing extreme values

- **Insight**:
  - Example Outliers:
    - **Rimac Nevera**: Extremely fast acceleration
    - **Mercedes EQS SUV**: Exceptionally high torque
    - **Tesla Roadster**: Very high top speed compared to peers

---

### 9️⃣ Which manufacturers have the highest number of battery cells and how does it relate to performance?

- **Approach**:
  - Bar chart of Battery Cells by Manufacturer
  - Side-by-side visuals comparing average top speed, range

- **Visual**:
  - Clustered column chart + KPI cards
  - Filter for battery cell count brackets

- **Insight**:
  - Brands like **Tesla** and **Lucid Motors** use higher cell counts.
  - No direct 1:1 correlation, but higher cell count often supported longer range.

---

### 🔟 Create a customer comparison dashboard (acceleration, range, top speed)

- **Approach**:
  - Designed user-friendly, filter-driven dashboard
  - Key specs (Acceleration, Range, Top Speed) shown side-by-side

- **Visual**:
  - Multi-filter interface:
    - Brand
    - Battery Type
    - Efficiency
  - Table with slicers and conditional highlights

- **Insight**:
  - Helps end-users shortlist vehicles by their preferences.
  - Effective for performance vs. efficiency trade-off analysis.

---

## ✨ Features of the Power BI Dashboard

- ✔️ Interactive filters and slicers (brand, battery type, motor type, etc.)
- ✔️ Custom DAX measures (e.g., Range/kWh)
- ✔️ Drill-through pages for detailed vehicle-level inspection
- ✔️ Conditional formatting to highlight best/worst performers
- ✔️ Tooltip-based exploration of specs
- ✔️ Outlier detection & annotation

---

## 📌 How to Use

1. Download the `.pbix` file from this repo.
2. Open in **Power BI Desktop**.
3. Explore dashboards using filters/slicers.
4. Navigate between visual pages designed around each analytical question.

---

## 📬 Contact -
E-mail - vishalkapoor9803@gmail.com

Linkedin - https://www.linkedin.com/in/vishal--kapoor/
