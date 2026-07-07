# Free-to-Paid Conversion Rate Analysis 📊

## Overview
This SQL project analyses student behaviour on a learning platform to determine conversion rates and engagement patterns.

## Objectives
*   Identify how quickly students watch content after registration.
*   Measure conversion from watching to purchasing.
*   Calculate the average time between key funnel milestones.

## Key Metrics Calculated
*   **Free-to-Paid Conversion Rate:** Percentage of students who purchased the course after watching a lecture.
*   **Average Registration-to-Engagement Time:** How long it takes students to watch their first lecture after signing up.
*   **Average Engagement-to-Purchase Duration:** How long students take to subscribe after their first lecture engagement.

---

## 🏗️ Project Flow: Funnel Stages

This project tracks student behaviour across three key stages:
1. **Registration:** Student signs up on the platform.
2. **First-Time Engagement:** Student watches their first lecture.
3. **Subscription Purchase:** Student buys a subscription to access full course content.

Using this flow, I performed a funnel analysis to calculate progression rates, drop-offs, and time gaps.

| **Funnel Stage** | **Data Analysed** | **What It Measures** |
| :--- | :--- | :--- |
| **1. Watched a Lecture** | Students with `first_date_watched` | Entry into the funnel |
| **2. Purchased Later** | Students with `first_date_purchased > first_date_watched` | Progression or Drop-off |
| **Output Metrics** | Count & % of converting students | Free-to-Paid Conversion Rate, Time Gaps |

---

## 🛠️ Tools Used
*   **SQL (MySQL)**
*   Aggregate functions, subqueries, and conditional logic
*   Funnel analysis concepts

## 📁 Files
*   **[`02_query.sql`](02_query.sql):** Main SQL query containing the funnel analysis.
*   **`query_output*.png`:** Outputs generated from the SQL execution.

---

## 📈 Query Outputs

### Output 1: Subqueries & Intermediate Setup
![Output 1](query_output1.png)

### Output 2: Initial Conversion Metrics
![Output 2](query_output2.png)

### Output 3: Time Gaps Analysis
![Output 3](query_output3.png)

### Output 4: Funnel Breakdown
![Output 4](query_output4.png)

### Output 5: Final Aggregated Metrics
![Output 5](query_output5.png)

### Output 6: Distribution of Engagement Delays
![Output 6](query_output6.png)
