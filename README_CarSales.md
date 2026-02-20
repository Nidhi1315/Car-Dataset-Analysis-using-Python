# 🚗 Car Sales Data Analysis

An exploratory data analysis (EDA) project on a car sales dataset containing **50,000 records** across 5 major manufacturers. The project uncovers pricing trends, mileage patterns, and model-level comparisons through rich visualizations using Matplotlib and Seaborn.

---

## 📋 Table of Contents

- [Overview](#overview)
- [Dataset](#dataset)
- [Tech Stack](#tech-stack)
- [Project Workflow](#project-workflow)
- [Key Analyses](#key-analyses)
- [Visualizations](#visualizations)
- [How to Run](#how-to-run)

---

## 📌 Overview

This project performs in-depth exploratory analysis of second-hand car sales data. It examines how factors like manufacturer, car model, fuel type, engine size, mileage, and year of manufacture influence car pricing. The analysis includes groupby aggregations, merges, and multiple chart types to reveal patterns across brands and models.

---

## 📊 Dataset

- **File:** `car_sales_data.csv`
- **Total Records:** 50,000 rows × 7 columns

| Column | Description |
|---|---|
| Manufacturer | Car brand (Ford, VW, Toyota, BMW, Porsche) |
| Model | Specific car model (15 unique models) |
| Engine size | Engine displacement in litres (1.0 – 5.0) |
| Fuel type | Petrol, Diesel, or Hybrid |
| Year of manufacture | Year the car was made (1984 – 2022) |
| Mileage | Total miles driven (630 – 453,537) |
| Price | Selling price in GBP (£76 – £168,081) |

**Manufacturer Distribution:**

| Manufacturer | Count |
|---|---|
| Ford | 14,959 |
| VW | 14,913 |
| Toyota | 12,554 |
| BMW | 4,965 |
| Porsche | 2,609 |

---

## 🛠️ Tech Stack

- Python 3
- Pandas
- Matplotlib
- Seaborn
- Google Colab / Jupyter Notebook

---

## 🔄 Project Workflow

1. **Import Libraries** — Pandas, Matplotlib, Seaborn
2. **Load Dataset** — Upload and read `car_sales_data.csv`
3. **Explore Data** — View shape, columns, and sample rows
4. **Manufacturer Analysis** — Count of cars per brand using `value_counts()`
5. **Mileage Analysis** — Average mileage grouped by manufacturer and model
6. **Mileage Comparison** — Merge model-level vs. brand-level average mileage
7. **Price Analysis** — Distribution, box plots, violin plots, scatter plots by model and manufacturer
8. **Visualizations** — Multiple chart types to present findings clearly

---

## 🔍 Key Analyses

**Average Mileage by Manufacturer:**

| Manufacturer | Avg Mileage |
|---|---|
| VW | 113,462 |
| BMW | 112,838 |
| Ford | 112,526 |
| Porsche | 111,638 |
| Toyota | 111,361 |

**Average Mileage by Model (selected):**

| Model | Avg Mileage |
|---|---|
| VW Passat | 115,021 |
| Ford Focus | 114,062 |
| BMW M5 | 113,931 |
| Porsche 718 Cayman | 113,057 |
| Toyota Yaris | 110,036 |

---

## 📈 Visualizations

The notebook generates the following charts:

- **Bar Chart** — Average mileage per manufacturer (simple)
- **Grouped Bar Chart** — Mileage by manufacturer and model (model-level vs. brand-level)
- **Histogram** — Price distribution across all cars
- **Histogram** — Mileage distribution across all cars
- **Box Plot** — Price distribution by car model (log scale)
- **Violin Plot** — Price distribution by manufacturer
- **Scatter Plot** — Price vs. manufacturer
- **Scatter Plot** — Price vs. car model
- **Strip Plot** — Price spread per car model with jitter

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/car-sales-analysis.git
   cd car-sales-analysis
   ```

2. **Install dependencies**
   ```bash
   pip install pandas matplotlib seaborn
   ```

3. **Add the dataset**
   Place `car_sales_data.csv` in the project root directory.

4. **Run the notebook**
   Open `car_sales_data.ipynb` in Jupyter Notebook or Google Colab and run all cells.

   > **Note:** If running on Google Colab, the notebook uses `files.upload()` to upload `car_sales_data.csv` directly. On Jupyter, update the loading line to `pd.read_csv('car_sales_data.csv')`.

---

## 📁 Project Structure

```
car-sales-analysis/
│
├── car_sales_data.csv        # Dataset
├── car_sales_data.ipynb      # Main analysis notebook
└── README.md                 # Project documentation
```

---

## 🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you'd like to change.

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).
