🎓 Online Learning Analytics Dashboard

Python • Power BI • Data Cleaning • Data Visualization

This repository contains the full workflow and deliverables for the Online Learning Trends & Course Performance Dashboard, built using Python for data preparation and Power BI for analytics and visualization.

The objective of this project is to consolidate data from multiple online learning platforms — Coursera, FutureLearn, Udacity, Simplilearn — into a unified dataset and extract insights about global e-learning trends.

📌 Project Overview

Online learning platforms have grown massively, but each uses different structures, categories, and metrics.
This project solves that by:

Integrating multiple datasets into a single unified model

Cleaning and transforming inconsistent fields

Creating interactive analytics dashboards

Identifying trends in course content, pricing, and user engagement

🔧 1. Data Cleaning & Preparation (Python)

All preprocessing steps are implemented in courses-notebook.ipynb.

✔ Dataset Integration

Data was loaded from four sources:

Coursera

FutureLearn

Udacity

Simplilearn

Processing included:

Standardizing column names

Detecting platform-specific attributes

Merging into a single clean dataset

✔ Data Cleaning Steps
🟦 Numeric Fields

Converted into numeric format:

Rating

Number of viewers

Courses

Price (unified field for all platforms)

Removed:

$, €, text, symbols

Non-numeric characters

🟩 Duration Cleanup

Extracted a unified numeric field:

Duration_hours

Handled diverse formats:

“4 months to complete”

“2 weeks”

“40 minutes”

“Approx. 10 hours to complete”

“Estimated 4 months”

🟨 Missing Data

Missing numeric values converted to NaN

No essential columns removed

Platform-unique fields preserved

📊 2. Power BI Dashboard

The dashboard is organized into two analytical pages, each with a unique focus.

📍 Page 1 — Overview & Key Insights

Purpose: Provide a high-level view of the online learning ecosystem.

🔹 Visuals Included

KPIs

Total Courses

% Free Courses

Top 5 Most Viewed Courses (Treemap)

Price vs Rating (Scatter Plot)

Top 10 Categories by Number of Courses (Bar Chart)

🔹 Filters / Slicers

Category

Site

Level

Price Range

📍 Page 2 — Skills & Instructor Insights

Purpose: Analyze course content depth and instructor performance.

🔹 Visuals Included

Median Price (KPI)

Average Rating (KPI)

Course Distribution by Site (Pie Chart)

Top 10 Instructors (Bar Chart — Coursera)

Average Duration by Course Type (Bar Chart)

🔹 Filters

Category

Site

Language

Price Range

🧮 3. DAX Measures Used

The dashboard uses the following key measures:

| **Measure**                  | **Description**                                |
| ---------------------------- | ---------------------------------------------- |
| **Total Courses**            | Counts all courses in the dataset              |
| **Average Rating**           | Computes mean rating across courses            |
| **Median Price**             | Calculates median course price                 |
| **Average Duration (hours)** | Average of the cleaned Duration_hours          |
| **% Free Courses**           | Percentage where *Course Type = "Free Course"* |


👤 Author

Rania Ben Hmida
💼 Data Analyst | BI Developer | ML Enthusiast
