# 🎬 Netflix Content Analysis — Data Analyst Project

## 📌 Project Overview

This project analyzes Netflix's content catalog using **Excel, Power Query, SQL/MySQL, and Power BI**.

The objective is to transform raw Netflix data into a structured analytical solution that helps understand **content types, ratings, genres, release trends, and countries associated with content**, while also allowing users to explore individual titles.

---

## 📸 Dashboard Screenshots

### Overview Dashboard
![Overview Dashboard](images/image1.png)

### Single Title View
![Single Title View](images/image2.png)

---

## 🎯 Business Problem

Netflix has a large content catalog containing Movies and TV Shows with information such as genres, ratings, directors, cast, countries, and release years.

The raw data contains **missing values, inconsistent formats, and multi-valued fields**, making analysis difficult.

This project cleans, transforms, normalizes, and models the data to create an interactive dashboard for content analysis.

---

## 🔄 Project Workflow

```text
Raw Netflix Dataset
        ↓
Excel Power Query
        ↓
Data Cleaning & Transformation
        ↓
SQL / MySQL
        ↓
Data Normalization
        ↓
Relational Tables
        ↓
Power BI Data Modeling
        ↓
Interactive Dashboard
        ↓
Insights & Business Analysis
```

---

## 🧹 1. Data Cleaning & Transformation — Excel Power Query

The raw Netflix dataset was prepared using **Power Query in Excel**.

### Key activities

- Handled missing/null values
- Checked duplicate records
- Corrected data types
- Cleaned inconsistent values
- Split multi-valued fields where required
- Prepared the dataset for relational analysis

Power Query was used to create a cleaner and more consistent dataset before SQL processing and Power BI analysis.

---

## 🗄️ 2. SQL / MySQL Data Preparation

SQL was used for data validation, transformation, and analysis.

### Examples of analysis

- Counted Movies and TV Shows
- Analyzed content by rating
- Analyzed content by release year
- Grouped content by different categories
- Validated the cleaned data

### Example SQL

```sql
SELECT 
    type,
    COUNT(*) AS total_titles
FROM netflix_data_titles
GROUP BY type;
```

---

## 🔗 3. Data Normalization

The original dataset contained multiple values in single columns such as:

- Cast
- Directors
- Genres
- Countries

These multi-valued attributes were separated into related tables to make the data more structured and easier to analyze.

`show_id` was used as the common key to connect the related tables.

### Main Tables

- `netflix_data_titles`
- `netflix_data_netflix_cast`
- `netflix_data_netflix_directors`
- `netflix_data_netflix_listed_in`
- `netflix_data_countries_released`
- `netflix_data_description`

---

## 🔗 4. Power BI Data Modeling

The cleaned and normalized data was loaded into Power BI.

The **Titles table** acts as the central table, with related tables containing information about:

- Cast
- Directors
- Genres
- Countries
- Descriptions

Relationships were created using `show_id`.

This relational model allows the dashboard to filter and analyze information across different attributes.

---

## 📊 5. Power BI Dashboard

### Overview Dashboard

The dashboard provides analysis of:

### 🎞️ Content Type

Comparison between:

- Movies
- TV Shows

### 📅 Content Added Over Time

Shows how Netflix content additions have changed over time.

### ⭐ Rating Analysis

Analyzes the distribution of titles across different content ratings.

### 🎭 Top 10 Genres

Identifies the most represented genres in the Netflix catalog.

### 🌍 Countries Associated With Content

Shows the geographical distribution of countries associated with Netflix titles.

---

## 🔎 6. Single Title View

A separate **Single Title View** allows users to select an individual movie or TV show and explore its details.

The page displays:

- Title
- Type
- Release Year
- Rating
- Description
- Genres
- Director
- Cast
- Countries

This provides detailed title-level analysis in addition to the overall dashboard.

---

## 📌 KPIs

The dashboard focuses on key metrics such as:

- **Total Titles**
- **Total Movies**
- **Total TV Shows**
- **Content by Rating**
- **Content Added Over Time**

---

## 💡 Key Insights

The analysis helps identify:

- The overall balance between Movies and TV Shows
- Major genres represented in the catalog
- Distribution of content ratings
- Content addition trends over time
- Countries associated with Netflix content
- Characteristics of individual titles

---

## 💼 Business Impact

The analysis can support content-related decisions by helping stakeholders understand the existing Netflix content portfolio across **genres, ratings, time periods, and countries**.

These insights can support decisions related to:

- Content production
- Content acquisition
- Catalog planning
- Geographic expansion

---

## 🛠️ Tools & Technologies

| Tool | Purpose |
|---|---|
| **Microsoft Excel** | Initial data handling |
| **Power Query** | Data cleaning & transformation |
| **MySQL / SQL** | Data preparation, validation & analysis |
| **Power BI** | Data modeling & visualization |
| **Power BI Relationships** | Connecting normalized tables |

---


---

## 🚀 Project Outcome

The final solution converts raw Netflix data into a **clean, normalized, and interactive analytical dashboard**.

It allows users to move from **high-level content analysis to detailed individual-title exploration**.

---

## 👩‍💻 Skills Demonstrated

- Data Cleaning
- Data Transformation
- Excel Power Query
- SQL / MySQL
- Data Normalization
- Relational Data Modeling
- Power BI
- Data Visualization
- KPI Analysis
- Business Insights
- Analytical Thinking
