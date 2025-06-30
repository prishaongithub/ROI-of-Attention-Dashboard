# 📊 The ROI of Attention – Power BI Dashboard

This Power BI project analyzes how viewers invest their time and attention on YouTube, breaking it down into **productive** vs **entertainment-oriented** content. The aim is to explore whether our screen time adds value — or merely distracts.

## 🧠 Project Overview
**Title:** The ROI of Attention: Are We Investing or Escaping?  
**Tool Used:** Power BI Desktop  
**Pages:** Overview | Revenue Insights | Monthly Trends | Key Metrics | Glossary  
**Timeframe:** June 2025  

---

## 🔧 Data Transformation Summary

This project began with raw YouTube trending data. Key steps performed:

- ✅ **Removed duplicates** using `video_id` to keep only the latest trending entry per video.
- ✅ **Handled errors and nulls** in numeric columns such as `likes`, `views`, `comment_count`, and `video_duration`.
- ✅ **Converted date types** (text to proper date) for trend analysis.
- ✅ **Created `TrendingMonth`** column to group data by month (e.g., Jan 2019).
- ✅ **Mapped category IDs** to readable names using a custom `DATATABLE()` and relationship model.
- ✅ **Created a custom `Content_Type` column** to classify videos into:
  - 🎓 Productive
  - 🎥 Entertainment
  - 🤝 Neutral

- ✅ **Added calculated columns**:
  - `Estimated Watch Time` (views × video duration in minutes)
  - `Estimated Revenue (INR)` (views × estimated CPM)
  - `Video Length (Minutes)`

- ✅ **Modeled relationships** between category and video tables for interactive filtering/slicers.

---

## 📐 DAX Measures Created

- `Total Revenue (INR)`
- `Total Watch Hours`
- `% Productive Revenue`
- `% Productive Watch Hours`
- `Monthly Productive Video Count`
- `Best Performing Month`
- `Most Productive Month`
- `Estimated Watch Time (Minutes)`

---

## 📊 What This Dashboard Shows

- 🧾 Overall watch time and revenue generated
- 🔍 How much attention goes to *productive* vs *entertainment* content
- 📅 Trends across months: What kind of content trended when?
- 🧠 Key influencers for productive content revenue
- 🏆 Best performing months and categories

---
## 📈 Insights & Recommendations

### 📊 Summary Insights:

- **Only 13.81%** of total YouTube revenue comes from productive content — despite it being more educational or skill-based.
- **Productive content accounts for just 12.5%** of total watch hours.
- **Entertainment categories like Music, Comedy, and Blogs** dominate the attention economy.

### 🔎 From Key Influencers Visual:

Top factors influencing **Productive Revenue**:
- Belonging to **How-to** or **Science & Tech** categories
- Longer **video duration** (users spend more time on valuable content)
- High number of **comments** (suggesting community engagement)

---

### 💡 Recommendations to Increase Productive Revenue:

- Encourage **long-form content** that adds depth and value (10+ mins).
- Boost **engagement tactics** (e.g., ask viewers to comment or share thoughts).
- Focus on **science, education, in the form of how-to content** — these yield better monetization per view.
- Use insights from **monthly trends** to publish in high-performing months (e.g., March or June).

---

## 📘 Glossary & Terminology

The dashboard includes a **Glossary page** defining all KPIs and metrics for viewer clarity.

---

## 🖥️ Files in This Repo

- `ROI_of_Attention.pbix` – Power BI project file
- `README.md` – Project overview & documentation
- `datasets/` – https://www.kaggle.com/datasets/datasnaek/youtube-new
- `screenshots/` – preview visuals

---

## 📍 Live Dashboard

🔗 https://app.powerbi.com/groups/me/reports/1964237d-f1d0-4e9a-bf1d-2e22ebf2bad8/0bb83f7fb59d40d5da09?experience=power-bi

---
