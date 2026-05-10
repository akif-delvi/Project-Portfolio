# 🛒 German E-Commerce Customer Behavior Analysis

> A data-driven exploratory analysis project focused on understanding customer purchasing patterns, return behavior, regional trends, and seasonal activity in the German e-commerce market.

## 📌 Project Overview

This project explores customer behavior in the German e-commerce industry using a dataset of more than 100,000 transactions. The analysis focuses on identifying shopping patterns, return trends, regional performance, pricing behavior, and seasonal activity through exploratory data analysis and visualization.

The goal of this project was not only to analyze the data technically, but also to extract business insights that could help improve customer experience, inventory planning, and operational decision-making.

The analysis focuses on understanding how demographics, geography, pricing, product categories, and time-based factors influence customer purchasing and return patterns in the German e-commerce market.

---

# 📊 Business Problem

E-commerce companies face several operational challenges:

* High product return rates
* Inefficient inventory allocation
* Poor demand forecasting
* Regional performance imbalance
* Seasonal order fluctuations
* Customer retention and segmentation difficulties

This project aims to solve these problems using data-driven insights and exploratory analytics.

---

# 🎯 Objectives

The project was designed to:

* Analyze customer demographics and purchasing behavior
* Identify return-rate drivers
* Discover high-performing products and regions
* Study pricing patterns and customer sensitivity
* Analyze seasonal and weekly order cycles
* Explore delivery performance trends
* Prepare the dataset for future machine learning applications

---

# 📂 Dataset Information

The dataset contains approximately **100,000 rows** of German e-commerce transactional data with multiple business-related attributes.

### Key Features Include:

| Feature Category     | Description                                   |
| -------------------- | --------------------------------------------- |
| Customer Information | Age, title, registration date                 |
| Geographic Data      | German states and regional activity           |
| Product Details      | Item ID, size, category, price                |
| Transaction Data     | Orders, deliveries, returns                   |
| Time Features        | Order dates, monthly trends, weekday patterns |

---

# 🛠️ Technologies & Libraries Used

| Tool / Library   | Purpose                          |
| ---------------- | -------------------------------- |
| Python           | Core programming language        |
| Pandas           | Data cleaning and manipulation   |
| NumPy            | Numerical operations             |
| Matplotlib       | Data visualization               |
| Seaborn          | Statistical visualization        |
| Jupyter Notebook | Interactive analysis environment |

---

# 🧹 Data Cleaning & Preprocessing

Several preprocessing techniques were applied before analysis:

* Handling missing and null values
* Removing duplicate records
* Converting date columns into datetime format
* Detecting abnormal registration spikes
* Filtering unrealistic outliers
* Cleaning size and pricing inconsistencies
* Creating new temporal features (month, weekday, year)

---

# 📈 Exploratory Data Analysis (EDA)

The project includes detailed exploratory analysis across multiple dimensions.

---

# 🔍 Key Insights & Findings

## 1️⃣ Customer Demographics Analysis

### Observations

* Majority of customers belong to the **35–55 age group**.
* Younger users (18–25) show lower engagement levels.
* Several age outliers suggest either:

  * data-quality inconsistencies
  * or participation from older demographics.

### Business Insights

* Middle-aged customers form the primary revenue-driving segment.
* Younger audiences may require:

  * improved onboarding
  * targeted marketing
  * or product personalization.

---

## 2️⃣ Geographic Distribution Analysis

### Observations

Top-performing states:

1. North Rhine-Westphalia
2. Bavaria
3. Lower Saxony
4. Baden-Württemberg

Low-engagement regions include:

* Bremen
* Saarland
* Mecklenburg-Vorpommern

### Business Insights

* Customer activity strongly mirrors German population density.
* Underperforming states provide expansion opportunities.
* Region-specific logistics and marketing campaigns can improve penetration.

---

## 3️⃣ Customer Registration Trend Analysis

### Major Finding

A significant anomaly was discovered:

* On **17 February 2015**, registrations exceeded **30,000 users**.
* This is likely caused by:

  * bulk customer import
  * database migration
  * or system-level event.

### After Cleaning

* Daily registrations stabilize between **0–50 users/day**.
* Summer months show stronger acquisition activity.
* November–December registrations decline noticeably.

### Business Insights

* Outlier removal is essential before forecasting.
* Seasonal acquisition strategies can improve customer growth.

---

## 4️⃣ Return Behavior Analysis

### Major Findings

* Overall return rate is approximately **51%**.
* Company accounts show the highest return rates (**~63%**).
* Individual customers (Mr/Mrs categories) remain near average.
* Users with missing title information return the least.

### Business Insights

High return rates indicate:

* sizing problems
* expectation mismatch
* insufficient product information.

### Recommended Solutions

* Better size charts
* AI-powered fit recommendation systems
* Enhanced product descriptions
* Improved product imagery

---

## 5️⃣ Price Sensitivity Analysis

### Observations

* Product prices show weak correlation with returns (**~0.14 correlation**).
* Most products are priced below **€100**.
* Expensive items (>€300) experience fewer returns.

### Business Insights

* Customers are not primarily returning products due to price.
* Fit, quality perception, and product expectations matter more.
* Premium purchases involve more deliberate buying behavior.

---

## 6️⃣ Product Performance Analysis

### Observations

* A small subset of products generates a large portion of sales.
* Bestselling items also contribute heavily to returns.
* Some SKUs repeatedly dominate transaction volume.

### Business Insights

* Inventory forecasting should prioritize high-volume SKUs.
* Bestselling products require enhanced quality and fit optimization.
* Return prediction systems should focus on high-frequency products.

---

## 7️⃣ Size Distribution Analysis

### Clothing Sizes

Most common clothing sizes:

* L
* XL
* M

### Footwear Sizes

Most common footwear sizes range between:

* 38–42

### Business Insights

* Inventory allocation should heavily prioritize mid-range sizes.
* Extreme sizes should be managed carefully to avoid overstocking.

---

## 8️⃣ Time-Series & Seasonal Analysis

### Weekly Trends

* Monday records the highest order volume.
* Weekends remain strong but slightly below weekday performance.

### Monthly Trends

* June–August show the highest transaction activity.
* Activity drops significantly after September.

### Business Insights

* Monday marketing campaigns may improve conversions.
* Summer periods are critical for sales planning and inventory management.

---

## 9️⃣ Delivery Performance Analysis

### Observations

* August 2016 recorded approximately **36,000 successful deliveries**.
* Delivery records after September become unreliable due to missing data.

### Business Insights

* Q4 logistics analysis cannot be trusted without complete delivery records.
* Missing delivery data must be addressed before operational forecasting.

---

# 📊 Statistical & Correlation Analysis

The project also includes:

* Correlation heatmaps
* Distribution analysis
* Return-rate relationships
* Price vs return comparisons
* Temporal trend analysis
* Frequency distribution studies

These analyses help identify hidden relationships and prepare the dataset for predictive modeling.

---

# 🤖 Future Machine Learning Scope

This project creates a strong foundation for advanced analytics and machine learning.

## Planned Extensions

### 1. Return Prediction Model

Build ML models to predict whether an item will be returned.

Possible algorithms:

* Logistic Regression
* Random Forest
* XGBoost
* LightGBM

---

### 2. Customer Segmentation

Perform clustering using:

* K-Means
* Hierarchical Clustering
* DBSCAN

To identify:

* high-value customers
* seasonal buyers
* frequent returners
* premium shoppers.

---

### 3. RFM Analysis

Analyze:

* Recency
* Frequency
* Monetary Value

To score customer lifetime value.

---

### 4. Recommendation Systems

Future enhancement may include:

* personalized product recommendation engines
* collaborative filtering
* content-based recommendation systems.

---

# 📁 Project Structure

```bash
├── Dataset/                 # Raw dataset (not uploaded)
├── Notebooks/               # Jupyter notebooks
├── visuals/                 # EDA visualizations and charts
├── README.md                # Project documentation
└── requirements.txt         # Python dependencies
```

---

# 📷 Visualizations

## 🖼️ Daily Orders with 7-Day Rolling Mean

![Daily Orders](https://github.com/alfiya-ansari-175/Data-Science-Portfolio/blob/2c88df290599aead0ef3860a2771cc5e443fa28a/German%20E-Commerce%20Customer%20Behaviour%20Analysis/visuals/Insights-1.png)

---

## 🖼️ Item Size Distribution

![Size Distribution](https://github.com/alfiya-ansari-175/Data-Science-Portfolio/blob/2c88df290599aead0ef3860a2771cc5e443fa28a/German%20E-Commerce%20Customer%20Behaviour%20Analysis/visuals/Insights-4.jpg)

---

## 🖼️ Orders Per State

![Orders Per State](https://github.com/alfiya-ansari-175/Data-Science-Portfolio/blob/2c88df290599aead0ef3860a2771cc5e443fa28a/German%20E-Commerce%20Customer%20Behaviour%20Analysis/visuals/Insights-2.jpg)

---

## 🖼️ User Count by State

![Users By State](https://github.com/alfiya-ansari-175/Data-Science-Portfolio/blob/2c88df290599aead0ef3860a2771cc5e443fa28a/German%20E-Commerce%20Customer%20Behaviour%20Analysis/visuals/Insights-8.jpg)

---

## 🖼️ Average Item Price by User Title

![Average Price](https://github.com/alfiya-ansari-175/Data-Science-Portfolio/blob/2218946ac4c37bb88064c7cc936f840bf7bd2cc1/German%20E-Commerce%20Customer%20Behaviour%20Analysis/visuals/Insights-7.jpg)

---

## 🖼️ Monthly Registration Comparison (2015 vs 2016)

![Monthly Registrations](https://github.com/alfiya-ansari-175/Data-Science-Portfolio/blob/c95536df476cdd89a17a192c675b5f7bbd786bfc/German%20E-Commerce%20Customer%20Behaviour%20Analysis/visuals/Insights-9.jpg)

---

# 🚀 How to Run the Project

## 1️⃣ Clone the Repository

```bash
git clone https://github.com/your-username/german-ecommerce-customer-analysis.git
```

## 2️⃣ Install Dependencies

```bash
pip install -r requirements.txt
```

## 3️⃣ Run the Notebook

```bash
jupyter notebook
```

Open the notebook and run all cells.

---

# 💡 What I Learned From This Project

Working on this project helped me better understand how raw transactional data can reveal real business problems and customer behavior patterns. One of the most interesting findings was discovering how strongly returns impact e-commerce operations and how customer activity changes across regions and seasons.

This project also strengthened my skills in:

* Cleaning and preprocessing messy real-world datasets
* Detecting anomalies and outliers
* Building meaningful visualizations
* Extracting business-focused insights from data
* Working with time-series and behavioral patterns

---

# 📌 Project Highlights

✅ Large-scale real-world e-commerce dataset
✅ End-to-end exploratory data analysis
✅ Advanced business insights
✅ Time-series and trend analysis
✅ Return behavior analytics
✅ Customer and regional analysis
✅ Visualization-driven storytelling
✅ Machine learning readiness

---

# 📚 Skills Demonstrated

* Exploratory Data Analysis (EDA)
* Data Cleaning & Preprocessing
* Data Visualization
* Statistical Analysis
* Business Intelligence
* Customer Behavior Analytics
* Time-Series Analysis
* Feature Engineering
* Problem Solving
* Insight Communication

---

# 📄 License

This project is intended for educational and analytical purposes only.

---

# 👩‍💻 Author

**Alfiya Ansari**

If you found this project useful, feel free to ⭐ the repository.
