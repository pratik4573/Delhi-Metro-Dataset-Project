# 🚇 Delhi Metro Data Analysis using Python

### 📊 Project Overview
This project analyzes Delhi Metro passenger trip data to uncover insights about ridership patterns, fare distribution, and route performance.  
The goal is to clean, process, and visualize the data to help understand travel behavior and optimize operational decisions.

---

## 🧠 Objectives
- Perform **data cleaning and preprocessing** on raw metro data  
- Conduct **Exploratory Data Analysis (EDA)** using visualization  
- Identify **top-performing routes and stations**  
- Calculate **key KPIs** such as total fare, passenger count, and revenue trends  

---

## 🧹 Data Cleaning & Preparation
| Problem Area | Action Taken |
|---------------|--------------|
| **Missing Values** | Filled missing `Ticket_Type` values logically (based on remarks or frequency) |
| **Inconsistent Formatting** | Cleaned text using `.str.strip()` and `.str.title()` |
| **Date Parsing** | Converted `Date` column to datetime using `pd.to_datetime()` |
| **Outliers** | Detected using boxplots/z-score and handled using capping |
| **Data Types** | Converted numeric columns to correct types using `astype(float)` |
| **Remarks Standardization** | Standardized casing and replaced missing remarks with `"normal"` |
| **Duplicates** | Removed duplicate trips using `df.duplicated()` |
| **Invalid Records** | Validated `Fare ≈ Cost_per_passenger * Passengers` |

---

## 📈 Exploratory Data Analysis (EDA)
Key analysis and visualizations:
- 🔹 **Top 5 Most Frequent Routes**
- 🔹 **Top 5 Starting and Destination Stations**
- 🔹 **Fare vs Distance Analysis**
- 🔹 **Average Fare by Ticket Type**
- 🔹 **Ridership Trends by Remark (e.g., weekend, festival)**

All visualizations were created using `Matplotlib` and `Seaborn`.

---

## 💰 KPI Metrics
| Metric | Description |
|--------|--------------|
| **Total Fare** | Sum of all fares collected |
| **Total Passengers** | Sum of all passengers across trips |
| **Average Fare per Trip** | Mean fare across all trips |
| **Top Revenue Route** | Route generating maximum total fare |

---

## 🧾 Key Insights
- **Tourist cards** had higher average fares compared to regular tokens.  
- Some routes showed **exceptionally high passenger volume**, indicating high-demand corridors.  
- **Weekend and festival days** experienced spikes in ridership.  
- Outlier detection helped identify **data entry anomalies** in fare amounts.

---

## 🧰 Tools & Technologies Used
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn  
- **Environment:** Jupyter Notebook  
- **Version Control:** Git & GitHub  

---

## 📂 Folder Structure
