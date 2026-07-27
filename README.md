# urban-mobility-economy-relation-2024
Data analysis project exploring the relationship between urban mobility (traffic congestion) and economic productivity (GDP per capita) across major Latin American cities in 2024. Built with Python and Pandas to identify key opportunities for transport infrastructure investment.

# Urban Mobility and Economy 2024 🚗📊

## 📌 Project Overview
This data analysis project aims to empirically evaluate the relationship between **urban mobility** (congestion levels and travel times) and **economic productivity** (GDP per capita and unemployment) across 15 major Latin American cities in 2024. 

By processing and merging multiple data sources, this analysis seeks to answer a key business and public policy question: *Is there a direct correlation between traffic congestion and economic development, and in which cities is it a priority to invest in transport infrastructure?*[cite: 1]

## 🛠️ Technologies and Tools
* **Language:** Python 3[cite: 1]
* **Data Manipulation & Cleaning:** Pandas, NumPy[cite: 1]
* **Data Visualization:** Seaborn, Matplotlib[cite: 1]
* **Environment:** Jupyter Notebook

## 🗂️ Data Sources
The project ingests and integrates data from two primary sources (processing over 1 million records)[cite: 1]:
1. **TomTom Traffic Index:** Real-time and historical data on travel times, jams delay, and traffic indexes by city[cite: 1].
2. **OECD Cities Economy:** Macroeconomic indicators including GDP per capita, unemployment rates, pollution levels (PM2.5), and population size[cite: 1].

## ⚙️ Methodology
The analysis followed a professional Data Analytics workflow:
1. **Data Wrangling & Cleaning:** 
   - Nomenclature standardization (*snake_case*)[cite: 1].
   - Data type conversion (transforming monetary and percentage strings to floats, parsing datetime formats)[cite: 1].
   - Generation of absolute metrics (e.g., calculating total population)[cite: 1].
2. **Transformation & Modeling:**
   - Filtering historical records to isolate the study period (2024)[cite: 1].
   - Grouping multiple daily records to calculate annual average metrics per city[cite: 1].
   - Performing an *Inner Join* between traffic and economic datasets using key variables (`city`, `year`)[cite: 1].
3. **Exploratory Data Analysis (EDA):**
   - Identifying outliers and statistical distributions through visualizations (Boxplots, Histograms, and comparative bar charts)[cite: 1].

## 💡 Key Insights
* **Lack of direct correlation:** It was determined that GDP per capita alone does not explain congestion[cite: 1]. For instance, Montevideo has the highest GDP per capita in the sample ($26,176) while maintaining very low congestion levels, whereas Mexico City presents a high GDP (21,111) but suffers from the most severe congestion in the region[cite: 1].
* **Opposite patterns in similar economies:** Cities like São Paulo and Buenos Aires, which share comparable economic levels, show diametrically opposed congestion patterns[cite: 1].
* **The issue of underdevelopment and traffic:** Cities with relatively lower productivity (such as Bogotá and Lima) face critical congestion (average delays exceeding 1,000 minutes), suggesting that congestion here is driven by structural deficiencies in mobility management rather than economic activity volume[cite: 1].

## 🎯 Strategic Recommendations
Based on the data, the recommendations for investment in infrastructure and mass public transport are:
1. **High Priority Cities:** **Mexico City, São Paulo, Bogotá, and Lima**[cite: 1]. In these cities, reducing congestion would have a direct multiplier effect on their competitiveness and productivity[cite: 1].
2. **Case Studies:** Analyze **Montevideo's** mobility and urban planning model as a successful reference point applicable to the rest of the region[cite: 1].

## 🚀 How to Run This Project
1. Clone this repository:
   ```bash
   git clone [https://github.com/your-username/urban-mobility-economy-2024.git](https://github.com/your-username/urban-mobility-economy-2024.git)
2. Use colab:
   [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)]([URL_DEL_NOTEBOOK_EN_GITHUB](https://colab.research.google.com/drive/15I9NGY3_Xu742ZpQRCZCil60mITC4W6p?usp=sharing)
   
