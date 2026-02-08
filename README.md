#  Netflix Case Study: Analysis & Recommendation System

This project began as a foundational data analysis exercise. It gradually evolved into a layered analytics and machine learning case study as my learning journey in data science progressed—from data cleaning and exploratory analysis to recommendation system design using NLP techniques.

**Project Notebook:**  
[the project link ](https://colab.research.google.com/drive/1dlJZDX7UVk7DAeqwDob_y9BjcSWl5QBc)

---

##  Project Overview

This case study analyzes Netflix’s content dataset to extract business insights and design a hybrid recommendation system.  
The workflow mirrors a real-world analytics + ML pipeline, covering:

- Data cleaning and preprocessing  
- Exploratory Data Analysis (EDA)  
- SQL-style analytical reasoning  
- Recommendation system design under realistic constraints  

The project demonstrates the ability to:
- Understand raw business data  
- Ask meaningful analytical questions  
- Translate insights into product-relevant outcomes  
- Design scalable and explainable recommendation logic  

---

##  Problem Statement

Netflix hosts a large and diverse catalog of movies and TV shows across countries, genres, and time periods.

The objectives of this project are:
- To analyze content trends and patterns on the platform  
- To understand how Netflix’s catalog has evolved over time  
- To extract insights that could inform content strategy  
- To design a recommendation system that accounts for real-world constraints such as cold start and scalability  

---

##  Tools & Technologies Used

### Programming & Analysis
- Python  
- Pandas  
- NumPy  

### Visualization
- Matplotlib  
- Seaborn  

### Machine Learning & NLP
- TF-IDF Vectorization  
- Cosine Similarity  
- Latent Semantic Modeling (Truncated SVD)  
- Hybrid Recommendation Systems  

---

##  Project Breakdown

### 1️ Data Cleaning & Preprocessing

This was one of the most challenging phases of the project.

- Decluttered and restructured nested data:
  - Split multi-valued fields
  - Reframed them using titles to preserve relevance
  - Stacked and reindexed data
  - Renamed columns and removed redundant index levels
- Handled missing values in:
  - `director`
  - `cast`
  - `country`
- Converted date fields to `datetime`
- Standardized duration formats
- Ensured overall data consistency for downstream analysis and modeling

---

### 2️ Exploratory Data Analysis (EDA)

Key analyses included:
- Distribution of Movies vs TV Shows  
- Growth of Netflix content over time  
- Country-wise content trends  
- Genre-wise content trends  
- Analysis of:
  - Ratings
  - Content duration  
- Identification of dominant genres and release patterns  

These insights reveal **platform-level trends** and provide signals relevant to Netflix’s **content strategy**.

---

### 3️ SQL-Style Analytical Queries

The dataset was explored using SQL-style logic to answer business-driven questions such as:

- Which genres dominate Netflix’s catalog?
- How has content addition changed year over year?
- How does content distribution vary across regions?
- How do ratings and duration differ by content type?

This phase emphasizes **structured analytical thinking**, similar to real-world data analyst workflows.

---

## 4 Final Phase: Recommendation System Design

A **multi-layer recommendation system** was designed to reflect real-world constraints.

###  Phase 1: Content-Based Recommendation
- Used TF-IDF on metadata:
  - Genre
  - Description
  - Cast
  - Director
- Computed item-to-item similarity using cosine similarity
- Similarity was computed **on demand** to avoid O(n²) memory usage

###  Phase 2: Latent Content Modeling
- Applied Truncated SVD on TF-IDF vectors
- Learned latent semantic representations of titles
- Reduced noise and improved thematic similarity

###  Phase 3: Weighted Hybrid Recommendation
- Combined:
  - Surface-level TF-IDF similarity
  - Latent semantic similarity
- Used a weighted hybrid approach to balance precision and robustness
- Improved recommendation quality without relying on user interaction data

---

##  Key Takeaways

- Netflix’s content strategy shows strong temporal, regional, and genre-driven patterns
- Data cleaning and feature preservation are critical for reliable insights
- Latent semantic modeling improves recommendation quality beyond keyword overlap
- Hybrid recommendation systems outperform single-method approaches in practice
- Thoughtful system design matters as much as model choice

---

## Future Improvements

- Incorporate true user–item interaction data for personalization
- Add evaluation metrics such as:
  - Precision@K
  - Recall@K
- Tune hybrid weights dynamically
- Deploy the recommender as:
  - A lightweight API
  - A web-based demo application

---

##  Conclusion

This project demonstrates **end-to-end capability** across:
- Data analysis
- Business reasoning
- Feature engineering
- Recommendation system design

It reflects real-world workflows where **data quality, interpretability, and system robustness** are just as important as algorithmic sophistication.

  
