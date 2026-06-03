
# Vrinda Store Data Analytics Project (Annual Sales Report 2022)

## Project Objective
The objective of this project is to analyze the 2022 sales data of Vrinda Store, an online retail business operating across multiple e-commerce channels in India. The goal is to deliver an interactive, data-driven performance report that provides clear insights into customer demographics, geographic sales distribution, and high-performing channels to drive strategic business growth in 2023.

---

## Technical Stack & Tools Used
*   **Tool:** Microsoft Excel
*   **Features:** Data Cleaning, Dynamic Formatting, Nested Functions (`IF`), Text Analytics (`TEXT`), Pivot Tables, Advanced Pivot Charts, Interactive Slicers, Dashboard Designing.

---

## Project Workflow & Implementation

### 1. Data Cleaning
Addressed anomalies, structural inconsistencies, and standardized values across a raw dataset of over 30,000 transactions:
*   **Standardization:** Cleaned the `Gender` column by map-reducing inconsistent labels (`M` to `Men`, `W` to `Women`).
*   **Data Correction:** Cleaned and standardized values within the `Size` column to ensure numerical uniformity.
*   **Validation:** Checked critical ID fields (`Order ID`, `Customer ID`) and financial variables for null values, blanks, or outliers to guarantee data integrity.

### 2. Data Processing & Engineering
Transformed and enriched raw columns to create structured parameters for data slicing:
*   **Age Segmentation:** Engineered an `Age Group` category using conditional logic:
    *   `Senior`: Age > 50
    *   `Adult`: 30 <= Age <= 50
    *   `Teenager`: Age < 30
*   **Temporal Extraction:** Utilized the `=TEXT(Date, "mmm")` function to extract distinct month codes (e.g., *Jan*, *Feb*, *Mar*) from the baseline delivery dates for macro-level time series charting.

### 3. Data Analysis & Pivot Architecture
Constructed dedicated Pivot Tables to process key business metrics:
*   **Sales vs. Orders:** Evaluated absolute financial turnover (Sum of Amount) alongside transactional density (Count of Orders) across months.
*   **Demographic Split:** Segmented shopping behaviors by `Gender` and `Age Group`.
*   **Geographic Metrics:** Isolated top-performing regional territories at the `State` level.
*   **Channel Performance:** Calculated percentage contribution metrics for multiple underlying distribution channels (Amazon, Flipkart, Myntra, etc.).

### 4. Interactive Dashboard Design
Built a consolidated, visually clean canvas highlighting:
*   **Dual-Axis Combo Chart:** Compares Sales and Order numbers on a synchronized timeline, revealing March as the peak performing month.
*   **Demographic & Status Distributions:** Custom pie and donut charts visualizing distribution shares across customer segments.
*   **Horizontal Bar Charts:** Ranking the Top 5 states driving revenue.
*   **Dynamic Cross-Filtering:** Configured interactive **Slicers** (Month, Channel, Category) with unified **Report Connections** to enable instant dashboard updates upon parameter selection.

---

## Data-Driven Insights & Strategic Summary

*   **Primary Customer Persona:** Adult women aged 30-49 contribute to approximately 35% of total sales volume.
*   **Platform Dominance:** Amazon, Flipkart, and Myntra generate roughly 80% of total annual revenue, with Amazon leading at 35%.
*   **Geographic Hubs:** Maharashtra, Karnataka, and Uttar Pradesh comprise the top 3 highest-revenue-generating states.

### Final Strategic Recommendation
To maximize sales growth in 2023, marketing spend should prioritize **targeted coupon campaigns and promotional offers for adult women (30-49) located in Maharashtra, Karnataka, and Uttar Pradesh**, deployed explicitly through **Amazon and Flipkart** interfaces.
