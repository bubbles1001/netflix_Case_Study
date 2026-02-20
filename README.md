# Netflix Data Analysis

## Project Overview
This project conducts an exploratory data analysis (EDA) on Netflix content data to understand patterns in content availability, production trends, and platform composition. The analysis combines data cleaning, feature engineering, and visualization to derive insights that inform data-driven recommendations.

---

## Dataset Description
The dataset contains metadata related to titles available on Netflix, including:

- Title  
- Content type (Movie / TV Show)  
- Director and cast  
- Country of production  
- Date added to Netflix  
- Release year  
- Rating  
- Duration  
- Genre(s)  

The dataset contains missing values and multi-valued categorical fields, reflecting real-world data complexity.

---

## Scope of Analysis
The analysis includes:

- Data cleaning and preprocessing  
- Handling missing and inconsistent values  
- Feature extraction from date and text columns  
- Exploratory Data Analysis (EDA)  
- Trend, distribution, and comparative analysis  

The analysis findings are later used to derive actionable recommendations.

---

## Data Cleaning & Preprocessing
Key preprocessing steps include:

- Converting date fields to datetime format  
- Extracting year and month from the `date_added` column  
- Handling missing values in categorical fields such as director and country  
- Standardizing column data types  
- Processing multi-value fields such as genres and countries for analysis  

These steps ensured data consistency and analytical reliability.

---

## Exploratory Data Analysis (EDA)

### Content Distribution
- Comparison of Movies vs TV Shows on the platform  
- Growth in content additions over time  
- Distribution of content by release year  

### Geographic Analysis
- Country-wise content production patterns  
- Identification of regions with high content contribution  

### Genre & Rating Analysis
- Most prevalent genres on Netflix  
- Rating distribution across Movies and TV Shows  
- Duration patterns across different content types  

### Time-Based Trends
- Year-wise and month-wise trends in content addition  
- Lag analysis between content release year and Netflix availability  

All observations are supported using visualizations and summary statistics.

---

## Tools & Technologies
- Python  
- Pandas  
- NumPy  
- Matplotlib  
- Seaborn  
- Jupyter Notebook  

---

## Outcomes and Recommendations
Based on the analysis, the following insights and recommendations were derived:

- Netflix has a significantly larger share of Movies compared to TV Shows, suggesting an opportunity to expand long-running and episodic content.
- Content production is heavily concentrated in a few countries, indicating potential for diversification by investing in underrepresented regions.
- Certain genres consistently dominate the platform, while niche genres remain less explored and could be targeted for audience expansion.
- Recent years show a sharp increase in content additions, highlighting a shift toward aggressive content acquisition and production.
- A noticeable delay exists between the content release year and platform addition for some titles, suggesting optimization opportunities in licensing and acquisition timelines.

These recommendations are grounded in observed historical patterns and platform trends.

---

## Repository Structure
