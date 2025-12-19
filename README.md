# 🌐 Website Performance Analysis Using Python

A complete **end-to-end website analytics project** built using **Python**, focusing on understanding user behavior, traffic sources, engagement quality, and time-based usage patterns. 

---

## 📌 Project Overview

Web analysis plays a crucial role in understanding how users interact with a website. This project analyzes **session-level website data** to answer key business questions such as:

* How website traffic and users evolve over time?
* Which marketing channels bring the most users?
* Which channels drive *high-quality* traffic?
* How engagement rate differs across channels?
* What time of day drives maximum traffic per channel?
* Does high traffic always means high engagement rate?

The analysis is entirely done using **Python-based data analysis and visualization libraries**.

---

## 📂 Dataset Description

The dataset contains **hourly website performance data** with the following key fields:

| Column                              | Description                                   |
| ----------------------------------- | --------------------------------------------- |
| channel group                       | Traffic source (Direct, Organic Social, etc.) |
| DateHour                            | Date & hour of activity (YYYYMMDDHH format)   |
| Users                               | Number of users                               |
| Sessions                            | Number of sessions                            |
| Engaged Sessions                    | Sessions with meaningful engagement           |
| Average engagement time per session | Avg. time spent per session                   |
| Engaged sessions per user           | Engagement intensity                          |
| Events per session                  | User interactions per session                 |
| Engagement rate                     | Ratio of engaged sessions                     |
| Event count                         | Total events                                  |

---

## 🧹 Data Cleaning & Preprocessing

### 1️⃣ Column Fixing

* The dataset initially had misplaced headers and unnamed columns.
* Correct column names were extracted from the first row and reassigned.

### 2️⃣ Data Type Conversion

* `DateHour` converted from string to `datetime`
* All numerical columns converted from `object` to numeric
* Invalid values handled using `coercion`

### 3️⃣ Feature Engineering

* Extracted **Hour** column from `DateHour` column to analyze hourly traffic patterns

✅ Result: A clean, structured dataframe with **3182 records** and **11 validated columns** ready for analysis.

---

## 📊 Exploratory Data Analysis (EDA)

### 🔹 1. Sessions & Users Over Time

**Line Chart**

* Shows how website traffic changes day by day and hour by hour.

📌 *Insight:* Website traffic is stable with clear time-based variations

---

### 🔹 2. Total Users by Channel

**Bar Chart**

* Direct and Organic Social channels contribute the highest number of users

📌 *Insight:* High-traffic channels can be leveraged as benchmarks to improve underperforming sources.

---

### 🔹 3. Average Engagement Time by Channel

**Bar Chart**

* Some channels attract fewer users but with **higher engagement time**
* Indicates content relevance and user intent vary by channel

📌 *Insight:* Traffic volume ≠ content effectiveness.

---

### 🔹 4. Engagement Rate Distribution by Channel

**Box Plot**

* Highlights engagement variability across channels
* Some channels show wide spread → inconsistent user quality, Others have tighter distributions → stable engagement

📌 *Insight:* Channels differ not just in traffic but in engagement consistency.

---

### 🔹 5. Engaged vs Non-Engaged Sessions

**Grouped Bar Chart**

* Compares quality of traffic per channel
* Reveals which channels drive meaningful interactions

📌 *Insight:* Certain channels generate high session counts but lower engagement proportions.

---

### 🔹 6. Traffic by Hour & Channel

**Heatmap**

* Visualizes peak traffic hours for each channel
* Different channels dominate at different times of day

📌 *Insight:* Helps in scheduling campaigns and content publishing.

---

### 🔹 7. Engagement Rate vs Sessions Over Time

**Dual Line Chart**

* Sessions and engagement rate do not always rise together
* High traffic periods sometimes show lower engagement

📌 *Insight:* Traffic spikes can dilute engagement quality.

---

## 📈 Key Business Insights

* **High traffic does not guarantee high engagement**
* **Channel quality matters more than volume**
* **User engagement varies significantly by time and source**
* **Data-driven timing can improve marketing ROI**

---

## 🚀 Project Takeaways

This project demonstrates:

- ✔ End-to-end data cleaning & validation
- ✔ Real-world website analytics use cases
- ✔ Strong EDA & visualization skills
- ✔ Business-focused interpretation of data

It closely mirrors how **data analysts analyze website performance data** in real industry settings.

---

## 🛠️ Tools & Libraries Used

* **Python**
* **Pandas** – data manipulation & cleaning
* **NumPy** – numerical operations
* **Matplotlib** – basic visualizations
* **Seaborn** – advanced statistical plots

---

## ▶️ How to Run This Project

```bash
pip install pandas numpy matplotlib seaborn
jupyter notebook
```

Then:
- 1. Open Website Performance Analysis.ipynb
- 2. Run cells from top to bottom

---

## 📬 Author

**Muskan Garg**
Aspiring Data Analyst | Python | Data Visualization | Analytics

---

⭐ *If you found this project helpful, feel free to star the repository!*

