# SAPFlow360 — Enterprise Procurement & Inventory Intelligence Using Python

## 📌 Project Overview

**SAPFlow360** is a data analytics project designed to analyze enterprise procurement and inventory data using Python. The project explores purchase orders, suppliers, materials, and inventory records to identify purchasing patterns, supplier activity, and stock distribution.

The goal is to transform raw business data into meaningful insights that can support procurement analysis and inventory-related decision-making.

## 🎯 Project Objectives

- Analyze purchase order activity across companies and suppliers.
- Identify the most active suppliers by purchase order count.
- Examine monthly purchasing trends.
- Identify materials with the highest total purchase value.
- Explore relationships between purchase quantity, unit price, and purchase value.
- Analyze inventory distribution across plants.

## 🛠️ Tools & Technologies

- **Python** — Data analysis and visualization
- **Pandas** — Data cleaning, transformation, and aggregation
- **NumPy** — Numerical operations
- **Matplotlib** — Chart creation and dashboard layout
- **Seaborn** — Statistical and business data visualization
- **Jupyter Notebook** — Interactive analysis and documentation

## 📂 Dataset Overview

The project uses interconnected procurement and inventory datasets.

| Dataset | Purpose |
|---|---|
| `purchase_orders_cleaned.csv` | Purchase order headers, suppliers, dates, and company codes |
| `purchase_order_items_cleaned.csv` | Material quantities, unit prices, and purchase values |
| `vendors_cleaned.csv` | Supplier details |
| `material_names_cleaned.csv` | Material descriptions |
| `plants_cleaned.csv` | Plant information |
| `material_groups_cleaned.csv` | Material group information |
| `inventory_current.csv` | Inventory stock information |
| `inventory_material_plant.csv` | Material and plant-level inventory data |

*Only datasets required by the final analysis need to be included in the repository. Ensure you have permission to share the data publicly.*

## 📊 Key Analyses & Visualizations

### 1. Supplier Procurement Activity
Analyzes unique purchase order counts by supplier to identify suppliers with the highest purchasing activity.

### 2. Monthly Purchase Order Trends
Examines changes in purchase order activity over time and identifies months with higher purchasing volume.

### 3. Material Purchase Value Analysis
Ranks materials by total recorded purchase value to highlight materials contributing the most to procurement spending.

### 4. Procurement Metrics Correlation
Uses a correlation heatmap to explore relationships between:
- `menge` — Purchase quantity
- `netpr` — Net price
- `netwr` — Net purchase value

### 5. Inventory Distribution
Analyzes unrestricted-use stock (`labst`) across plants (`werks`) to compare recorded inventory quantities.

### 6. Company-Level Procurement Analysis
Compares purchase order activity across company codes (`bukrs`) to understand differences in procurement volume.

## 💡 Business Value

SAPFlow360 demonstrates how Python can be used to:

- Identify suppliers with high procurement activity.
- Understand purchasing patterns over time.
- Prioritize materials for further purchasing analysis.
- Explore quantity, price, and purchase-value relationships.
- Compare inventory levels across plants.
- Support data-driven procurement and inventory discussions.

These analyses describe patterns in the available data; they do not independently establish supplier quality, stockout risk, or procurement efficiency.

## 🚀 How to Run the Project

### 1. Clone the repository

```bash
git clone <your-github-repository-url>
cd SAPFlow360
```

### 2. Create a virtual environment

```bash
python -m venv .venv
```

### 3. Activate the environment

Windows Command Prompt:

```bash
.venv\Scripts\activate
```

### 4. Install dependencies

```bash
pip install -r requirements.txt
```

### 5. Launch Jupyter Notebook

```bash
jupyter notebook
```

Open `SAPFlow360_Analysis.ipynb` and run the notebook cells in order.

Ensure the required CSV files are in the expected locations before running the analysis.

## 📁 Project Structure

```text
SAPFlow360/
│
├── data/
│   ├── purchase_orders_cleaned.csv
│   ├── purchase_order_items_cleaned.csv
│   ├── vendors_cleaned.csv
│   ├── material_names_cleaned.csv
│   ├── plants_cleaned.csv
│   ├── material_groups_cleaned.csv
│   ├── inventory_current.csv
│   └── inventory_material_plant.csv
│
├── SAPFlow360_Analysis.ipynb
├── README.md
├── requirements.txt
└── .gitignore
```

*Adjust the folder structure in this README to match the actual locations of your files.*

## 👨‍💻 Skills Demonstrated

- Data cleaning and preprocessing
- Data merging and aggregation
- Exploratory data analysis (EDA)
- GroupBy operations and ranking
- Date-based analysis
- Correlation analysis
- Data visualization
- Business insight communication
- Python-based analytics workflow

## 🔮 Future Improvements

- Build an interactive procurement dashboard.
- Add material-group and plant-level comparisons.
- Investigate inventory shortages using suitable historical stock and demand data.
- Connect the analysis to a database.
- Add automated data-quality checks and repeatable reporting.

---

**Project:** SAPFlow360 — Enterprise Procurement & Inventory Intelligence Using Python  
**Category:** Data Analytics  
**Primary Tools:** Python, Pandas, NumPy, Matplotlib, Seaborn, Jupyter Notebook
