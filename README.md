# Seasonal-Agricultural-Performance-Analysis
## 📌 Project Overview

Agricultural performance can vary significantly across seasons due to changes in environmental conditions, farming practices, resource availability, crop selection, and market conditions. However, raw agricultural data does not directly reveal how these factors influence productivity, profitability, resource efficiency, and agricultural risk.

This project performs **Exploratory Data Analysis (EDA) and data visualization** on an agricultural dataset to investigate seasonal differences in agricultural performance and identify meaningful patterns, trends, relationships, and variations within the available data.

The analysis focuses on **seasonal performance, crop productivity, profitability, resource efficiency, environmental conditions, farming practices, irrigation methods, and disease/pest risk**.

The overall objective is to transform raw agricultural data into meaningful insights that can support **data-driven farming, resource allocation, crop planning, and agricultural decision-making**.

---

## 🎯 Problem Statement

Agricultural activities are influenced by seasonal variations in environmental conditions, farming practices, resource availability, and market conditions. As a result, agricultural performance may differ from one season to another.

However, raw agricultural data does not clearly explain how agricultural performance changes across seasons or what patterns can be observed under different seasonal conditions.

The problem is to analyze the given agricultural dataset and investigate **seasonal differences in agricultural performance** by identifying meaningful:

- Patterns
- Trends
- Relationships
- Variations

within the available agricultural data.

---

## 🎯 Project Objectives

The main objectives of this analysis are:

1. Understand the structure and quality of the agricultural dataset.
2. Compare agricultural productivity across different seasons.
3. Identify the best-performing season based on yield and production.
4. Analyze crop performance across different seasons.
5. Compare profitability across seasons, crops, and states.
6. Examine water usage and water efficiency across crops and irrigation methods.
7. Analyze seasonal variations in environmental conditions such as rainfall, temperature, and soil moisture.
8. Investigate the relationship between environmental factors and agricultural yield.
9. Analyze farming practices such as irrigation, fertilizer, pesticide, nutrient usage, and seed quality.
10. Identify relationships between farming practices and agricultural yield.
11. Analyze disease and pest risk across seasons.
12. Identify the strongest relationships among numerical agricultural variables using correlation analysis.
13. Derive meaningful insights that can support agricultural planning and resource allocation.

---

## 📊 Dataset Overview

The dataset contains **4,000 farm-level agricultural records** covering different geographical locations, crops, and seasons.

### Dataset Coverage

- **Records:** 4,000
- **States:** 9
- **Districts:** 10
- **Crop Types:** 8
- **Seasons:** 3

### Major Variables

| Category | Variables |
|---|---|
| Farm Information | Farm Area |
| Geography | State, District |
| Crop & Season | Crop, Season |
| Environmental Conditions | Rainfall, Temperature, Humidity, Sunlight |
| Soil Characteristics | Soil pH, Soil Moisture |
| Nutrients | Nitrogen, Phosphorus, Potassium |
| Farming Inputs | Fertilizer, Pesticide, Seed Quality |
| Productivity | Yield, Production |
| Financial Factors | Market Price, Total Cost, Revenue, Profit |
| Water Management | Water Used, Water Efficiency |
| Agricultural Risk | Disease/Pest Risk |
| Farming Practices | Irrigation Method |

### Derived Metrics

The following calculated columns were created:

- **Profit Margin (%)** = `(Profit(INR) / Revenue(INR)) x 100`
- **Profit Per Hectare** = `Profit(INR) / Farm Area(Hectares)`
- **Revenue Per Hectare** = `Revenue(INR) / Farm Area(Hectares)`
- **Cost Per Hectare** = `Total Cost(INR) / Farm Area(Hectares)`
- **ROI (%)** = `(Profit(INR) / Total Cost(INR)) x 100`
- **Water Used Per Tonne** = `Water Used(m3) / Production(Tonnes)`

---

## 📌 Important Terminologies:
-**🌧️ Kharif Season:** The monsoon season, generally from June to October, when crops are mainly grown with seasonal rainfall.
-**❄️ Rabi Season:** The winter season, generally from October/November to March/April, suitable for crops grown in cooler and relatively dry conditions.
-**☀️ Zaid Season:** The short summer season, generally from March to June, when crops are cultivated between the Rabi and Kharif seasons.

---

## 🔍 Analysis Workflow

The analysis follows the workflow below:

| Step | Analysis Stage |
|---|---|
| 1 | 📥 Data Import |
| 2 | 🔎 Data Exploration & Quality Assessment |
| 3 | 🧹 Data Cleaning & Preprocessing |
| 4 | ⚙️ Feature Creation |
| 5 | 📊 Outlier Detection |
| 6 | 🌦️ Seasonal Performance Analysis |
| 7 | 🌱 Crop Performance Analysis |
| 8 | 🌍 Environmental Factor Analysis |
| 9 | 🚜 Farming Practice Analysis |
| 10 | 💰 Financial Performance Analysis |
| 11 | 📈 Correlation Analysis |
| 12 | 💡 Key Findings & Conclusion |

---

## 🏁 Overall Conclusion

The **Seasonal Agricultural Performance & Productivity Analysis** reveals significant differences in agricultural productivity, profitability, water efficiency, and risk across seasons, crops, and farming practices.

**Kharif emerges as the strongest overall-performing season**, delivering the highest average yield, total production, profit, ROI, and water efficiency. However, it also records the highest disease and pest risk.

At the crop level, **Sugarcane is the best-performing crop overall**, consistently achieving the highest yield, production, profit, and ROI across Kharif, Rabi, and Zaid seasons.

The analysis also highlights **Water Efficiency as the factor most strongly associated with Yield**, while most environmental variables and farming inputs show negligible direct linear relationships with yield.

Overall, the findings demonstrate that **crop selection, seasonal conditions, water management, and production efficiency** are important considerations for agricultural and financial performance.

---

## 🔑 Key Findings

### 🌦️ Seasonal Performance

- **Kharif was the best-performing season overall**, with the highest average yield, total production, profitability, ROI, and water efficiency.
- **Zaid showed the weakest financial performance**, with negative average profit, profit per hectare, profit margin, and ROI.
- Kharif also recorded the **highest disease and pest risk**, highlighting a potential trade-off between productivity and agricultural risk.

### 🌱 Crop Performance

- **Sugarcane was the top-performing crop**, consistently recording the highest yield and profit across Kharif, Rabi, and Zaid seasons.
- **Chilli also demonstrated strong profitability**, particularly in terms of profit margin.
- **Maize, Rice, and Wheat showed comparatively weaker or negative financial performance**.

### 💧 Water Efficiency & Irrigation

- **Water Efficiency had the strongest positive relationship with Yield (0.92)**, followed by **Production (0.89)**.
- **Drip irrigation achieved the highest average yield**.
- **Rainfed agriculture showed the highest water efficiency**.
- These findings highlight the importance of efficient water utilization for agricultural productivity.

### 🌍 Environmental Factors

- **Rainfall, temperature, soil moisture, humidity, and disease/pest risk showed negligible direct correlations with Yield** in this dataset.
- Although these environmental variables vary across seasons, their individual linear relationships with yield were weak.

### 🚜 Farming Inputs

- **Fertilizer, pesticide, seed quality, and individual NPK nutrient usage showed little to no direct linear relationship with Yield**.
- This suggests that input quantities alone do not explain yield variation within the analyzed dataset.

### 💰 Financial Performance

- **Kharif recorded the strongest overall financial performance**.
- **Sugarcane achieved the highest average profit per hectare and ROI**.
- **Chilli demonstrated strong profitability**, particularly in terms of profit margin.
- **Punjab recorded the highest average profit per hectare**, followed by Telangana, Maharashtra, and Karnataka.

### 📈 Correlation Analysis

The strongest relationships identified in the correlation analysis were:

| Relationship | Correlation |
|---|---:|
| Farm Area ↔ Total Cost | **0.96** |
| Yield ↔ Water Efficiency | **0.92** |
| Revenue ↔ Profit | **0.89** |
| Yield ↔ Production | **0.89** |
| Production ↔ Water Efficiency | **0.81** |

The correlation heatmap visually confirms these strong relationships among the key numerical variables.

---

## 💡 Overall Insight

Overall, the analysis suggests that **improving water efficiency, selecting high-performing crops such as Sugarcane, adopting effective irrigation practices, and considering seasonal profitability** can support better agricultural productivity and financial outcomes.

The findings provide a data-driven perspective that can support **crop planning, resource allocation, water management, seasonal decision-making, and agricultural performance evaluation**.

> **Note:** Correlation represents statistical association and does not imply causation. The findings describe relationships observed within the analyzed dataset.

---

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn
- **Development Environment:** Google Colab

---

## 👩‍💻 Author

Ritika Moolya  
Bachelor of Computer Applications (BCA)  
Interested in Data Analytics, Data Science, and Business Intelligence
