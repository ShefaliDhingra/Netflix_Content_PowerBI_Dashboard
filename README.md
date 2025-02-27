# 📊 Netflix Content Analysis

## 📝 Introduction

### 🎯 Objective
This project analyzes Netflix’s content strategy by evaluating IMDb ratings, audience engagement, genre trends, and country-specific content distribution. The goal is to determine whether Netflix prioritizes quality over quantity and how factors like genre, country, and release year influence content performance.

### 📂 Dataset Source
- The dataset was sourced from **Kaggle** and merged with **IMDb** data.
- The data was **normalized** into various sub-tables for dashboard visualization in **Power BI**.

### 📖 Storyline
Netflix has significantly expanded its content library in recent years. This analysis investigates:
- Whether Netflix maintains high-quality standards or focuses solely on content volume.
- How different genres, countries, and time periods contribute to content success.

---

## 🔍 Problem Statements & Analysis

### 📈 How have IMDb ratings for Netflix content changed over time?
- IMDb ratings have fluctuated over the years.
- No clear upward trend suggests a mixed approach to content strategy.

### 🎥 Is Netflix adding more high-quality content or just increasing volume?
- The number of new releases has significantly increased.
- IMDb ratings have remained **relatively stable**, indicating a focus on **quantity** rather than consistent improvement in quality.

### 📊 Do certain genres consistently receive higher ratings?
- **International Movies, Dramas, and Comedy** tend to receive **higher** ratings.
- **Reality Shows** often have **lower** average ratings.

### 🌍 Which countries produce the highest-rated Netflix content?
- **United States, United Kingdom, and Canada** have the highest-rated Netflix titles.
- **South Korea and Spain** also contribute significantly to highly-rated content.

### 📌 Does Netflix’s content strategy favor specific genres or regions?
- Netflix invests heavily in **high-performing genres** like **International Movies and Dramas**.
- Strong regional expansions in **Asia and Europe**.

### 🎭 Has there been a shift towards more mature or family-friendly content?
- Increasing trend in **mature-rated** content (**TV-MA, R**), indicating a focus on an **adult audience**.

---

## 🛠 Data Preparation & Normalization

### 🔄 Key Data Transformations
- **Multi-Value Attributes Handling:** Created separate tables for `Genres` and `Countries`.
- **Categorical Normalization:** Introduced an `Age Ratings` lookup table.
- **Redundant Data Removal:** Removed non-essential fields (`Director`, `Cast`, `Description`).
- **Bridge Tables:** Used mapping tables for `Title-Genre` and `Title-Country` relationships.

### 📋 Final Data Structure

| Table Name           | Purpose                                | Key Field       |
|----------------------|----------------------------------------|----------------|
| `Main_Titles.xlsx`   | Core dataset with title details       | Title_ID       |
| `Genres.xlsx`        | Unique list of genres                 | Genre_ID       |
| `Countries.xlsx`     | Unique list of countries              | Country_ID     |
| `Age_Ratings.xlsx`   | Unique list of age ratings            | Age_Rating_Code |
| `Genre_Mapping.xlsx` | Bridge table linking Titles & Genres  | Title_ID, Genre_ID |
| `Country_Mapping.xlsx` | Bridge table linking Titles & Countries | Title_ID, Country_ID |

---

## 📊 Key Insights & Visualizations

### **📌 Page 1: Overview**  
General summary of Netflix content distribution.

### **📈 Page 2: Ratings Trends**  
- **IMDb Ratings Over Time** (Line Chart)  
  - Insight: Ratings have not significantly increased despite content expansion.
- **Top 5 Highest-Rated Netflix Titles** (Bar Chart)  
  - Insight: High-rated content spans multiple genres.

### **🌎 Page 3: Genre & Country Analysis**  
- **Content Distribution** (Map Visualization)  
  - Insight: **United States & India** have the **largest** number of Netflix titles.

### **🎬 Page 4: Movie Durations & TV Show Seasons**  
- **Tree Map** (Movie Duration) & **Funnel Chart** (TV Show Seasons)  
  - Insight: Most movies are **90-120 minutes** long.  
  - TV shows are often **limited series (1 season)**.

### **👨‍👩‍👧‍👦 Page 5: Audience Targeting**  
- **Age Ratings Breakdown** (Stacked Bar Chart)  
  - Insight: **TV-MA (Mature)** is the most common rating.
  - Family-friendly content is present but lower in volume.

---

## 📌 Conclusion & Recommendations

### 🔎 Findings
- **Quality vs. Quantity:** Netflix is **expanding its library** without a consistent improvement in IMDb ratings.
- **Regional Strengths:** High-rated content comes from **United States, UK, and South Korea**.
- **Audience Preferences:** **TV-MA-rated** content dominates, indicating a shift toward mature audiences.
- **Engagement & Ratings:** **Higher IMDb votes** correlate with **better ratings**.

### ✔️ Recommendations
✅ Maintain a **balance** between **content volume and quality**.  
✅ Focus on **high-performing genres** to **enhance audience satisfaction**.  
✅ Expand **high-rated regional content** (South Korea, Spain).  
✅ Leverage **audience insights** (IMDb votes & ratings) for better content decisions.

---

## 🚀 Author
👩‍💻 **Shefali Dhingra**  
