
## ☕ Coffee Data Analysis & Dashboard

### 📘 Introduction

This project comprehensively analyses coffee sales and distribution data using Microsoft Excel. It includes an interactive and visually appealing dashboard with key insights derived from formulas like
`XLOOKUP`, `IFS`, and `DATEDIF`. The dashboard leverages pivot charts, slicers, and formatted tables for dynamic data exploration and reporting.

---

### 📂 Table of Contents

* [Introduction](#-introduction)
* [Installation](#-installation)
* [Usage](#-usage)
* [Features](#-features)
* [Excel Dashboard Details](#-excel-dashboard-details)
* [Formulas Used](#-formulas-used)
* [Pivot Table & Chart](#-pivot-table--chart)
* [Slicers](#-slicers)
* [Graphs and Formatting](#-graphs-and-formatting)
* [Examples](#-examples)
* [Troubleshooting](#-troubleshooting)
* [Contributors](#-contributors)
* [License](#-license)

---

### 💾 Installation

1. Clone or download this repository.
2. Open the `coffeeOrdersData.xlsx` file in Microsoft Excel (preferably Excel 365 or Excel 2019 and later for full formula support).

---

### 🚀 Usage

Use the dashboard to:

* Analyse total sales, average prices, and regional trends.
* Filter data by product type, region, or date.
* Compare year-over-year growth.
* View performance metrics by coffee blend or supplier.

---

### ✨ Features

* Dynamic dashboard with real-time filtering.
* Calculations using advanced Excel formulas.
* Automatically updates based on the data source.
* Insightful visuals including trend lines, bar graphs, and pie charts.

---

### 📊 Excel Dashboard Details

The dashboard consists of:

* **Summary KPIs**: Total Sales, Total Quantity, Average Price.
* **Time Analysis**: Monthly and yearly sales comparison.
* **Category Breakdown**: Coffee types, blends, and supplier analysis.
* **Regional Analysis**: Sales by region/city/country.

---

### 🧠 Formulas Used

#### 1. `XLOOKUP`

Used to fetch details like region or supplier name based on product ID:

```excel
=XLOOKUP([@ProductID], ProductTable[ID], ProductTable[Supplier])
```

#### 2. `IFS`

Used for multi-conditional classification of performance:

```excel
=IFS([@Sales]>=100000, "High", [@Sales]>=50000, "Medium", TRUE, "Low")
```

#### 3. `DATEDIF`

Used to calculate the difference between the order date and the delivery date:

```excel
=DATEDIF([@OrderDate], [@DeliveryDate], "d")
```

---

### 📈 Pivot Table & Chart

* Created a pivot table for **Monthly Sales by Region**.
* Inserted a **Pivot Chart** (column and line combination) for visualisation.
* The pivot table dynamically updates with new data entries.

---

### 🎛️ Slicers

* Inserted slicers for:

  * **Region**
  * **Product Category**
  * **Year**
* These slicers allow users to filter pivot charts and tables with a click.

---

### 🎨 Graphs and Formatting

* Applied conditional formatting to highlight top-performing regions.
* Used data bars and colour scales for quick comparison.
* Added:

  * Bar chart for the top 5 blends
  * Pie chart for sales share by region
  * Line graph for monthly trends

---

### 🧪 Examples

**Example Use Cases:**

* Filter by *Espresso* type to see how it performs across cities.
* Use the slicer to analyze *2024* sales only.
* Observe delivery delays using the `DATEDIF` calculation across suppliers.

---

### 🛠️ Troubleshooting

| Issue                  | Solution                                        |
| ---------------------- | ----------------------------------------------- |
| Formulas not working   | Ensure Excel version supports dynamic arrays    |
| Slicers not responding | Ensure they are correctly linked to the pivot table |
| Charts not updating    | Refresh the pivot table via Data > Refresh All  |

---

### 👥 Contributors

* **Inderbir Singh** – Data Analyst & Excel Specialist


