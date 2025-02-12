# Aviation Accident Analysis & Insights

## Overview
This repository contains a **comprehensive data analysis of aviation accidents and incidents**

## Key Objectives
-**Data Cleaning & Pocessing**
    - Identified and handled missing vales (**`NaN`** and string **'NaN'**)
    - Standardized categorical columns and resolved inconsistencies.
    - Eliminated duplicate records and validated key fields.
    - Ensured numerical fields (such as engine counts and injury reports) were corrected
    
- **Business-Driven Data Exploration**
  - **Aircraft Selection** → Identified the safest and most accident-prone aircraft models.
  - **Fleet Planning** → Analyzed incident trends to guide aircraft purchases.
  - **Route Safety Analysis** → Mapped accident frequency across different regions.
  - **Flight Phase Risk Assessment** → Determined when accidents are most likely to occur.
  - **Weather & Environmental Impact** → Evaluated the influence of weather conditions on accident likelihood.

##  Data Processing & Cleaning
The dataset was **cleaned and transformed** to remove inconsistencies and prepare for visualization & machine learning. Key data processing steps included:


### ** Handling Missing Values**
- **Converted string `"NaN"` values to actual `np.nan`** and handled missing categorical data.
- **Filled missing numerical data** with appropriate statistical methods (`mode()`, `0` for injuries).
- **Removed impossible values** (e.g., zero engine counts in aircraft).

### ** Standardizing Categorical Data**
- Converted categorical text fields to **uppercase** and **removed extra spaces**.
- Standardized **injury severity classifications** (e.g., `"Fatal(3)"` → `"Fatal"`).
- Categorized incidents into **Fatal, Serious, Minor, and Non-Injury classifications**.

### ** Validating Injury Reports**
- Ensured consistency between **injury severity labels and reported fatalities**.
- **Resolved inconsistencies** where `"Fatal"` incidents had `0` reported fatalities.

### ** Identifying High-Risk Flight Phases**
- Grouped data by **flight phase** (Takeoff, Cruise, Landing, etc.).
- Visualized accident frequency during **each phase of flight**.

##  Visualizations & Insights
This project includes multiple **data visualizations** to communicate insights clearly:

### ** Accident Frequency by Flight Phase**
- **Findings:** Most accidents occur during **Landing, Takeoff, and Approach**.
- **Impact:** Highlights the need for **improved pilot training** and **aircraft stability checks**.

### ** Route Risk Analysis**
- **Findings:** Certain regions experience **higher accident frequencies**.
- **Impact:** Helps companies optimize **safe flight routes**.

### ** Aircraft Model Safety**
- **Findings:** Some aircraft models show **higher accident-to-fatality ratios**.
- **Impact:** Can inform **fleet purchases** and **safety improvements**.

##  Tools & Technologies Used
- **Python (Pandas, NumPy, Matplotlib, Seaborn)**
- **Tableau (Data Visualization & Dashboards)**
- **Jupyter Notebook (Data Cleaning & Analysis)**
- **csv (For Exporting Final Clean Data)**