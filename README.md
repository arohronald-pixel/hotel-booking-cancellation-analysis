#  Hotel Booking Cancellation Prediction & Customer Segmentation

A full end-to-end data science capstone project analysing hotel booking data to predict cancellations and segment customers by behaviour using Machine Learning and Clustering techniques.

---

## 📌 Project Overview

Hotel cancellations cost the hospitality industry millions in lost revenue every year. This project uses real-world booking data to:
- **Predict** which bookings are likely to be cancelled
- **Segment** customers into behavioural groups to help hotels make smarter business decisions

---

## 📊 Dataset

- **Source:** [Hotel Booking Demand — Kaggle](https://www.kaggle.com/datasets/jessemostipak/hotel-booking-demand)
- **Size:** 100,000+ hotel booking records
- **Features:** Lead time, customer type, market segment, country, ADR, previous cancellations, and more

---

## 🔧 Tools & Technologies

| Tool | Purpose |
|------|---------|
| Python | Core programming language |
| Pandas | Data manipulation and cleaning |
| SQLite | SQL querying and business insights |
| Scikit-learn | Machine learning models |
| Seaborn & Matplotlib | Data visualisation |
| KaggleHub | Dataset loading |

---

## 🗂️ Project Structure

### Part 1 — Data Foundation
- Loaded dataset directly from Kaggle using KaggleHub
- Pushed data into SQLite database
- Ran SQL queries to extract business insights:
  - Average daily rate (ADR) by hotel type
  - Top booking countries
  - Cancellation rate by customer type

### Part 2 — Feature Engineering
- Created new features: Total Guests, Total Nights Stayed, ADR per Guest
- Encoded categorical variables for ML

### Part 3 — Exploratory Data Analysis (EDA)
- Analysed distribution of cancellations, lead time, market segment, customer type
- Identified key drivers of cancellation behaviour

### Part 4 — Machine Learning Models
- Built and compared classification models including **Random Forest** and **Logistic Regression**
- Handled class imbalance using **SMOTE**
- Selected **Random Forest (threshold = 0.35)** as the best model for deployment

### Part 5 — Customer Segmentation (Clustering)
- Applied **KMeans Clustering** with K = 3, 5, and 7
- Identified 3 customer personas:

| Persona | Cancellation Rate | Description |
|---------|------------------|-------------|
| 🟢 Loyal Guests | ~14–25% | Reliable customers who rarely cancel |
| 🟡 Uncertain Planners | ~25–45% | Sometimes cancel depending on plans |
| 🔴 High-Risk Bookers | ~60–100% | Frequently cancel bookings |

### Part 6 — Business Recommendations
- Target high-cancellation segments with stricter deposit policies
- Reward loyal repeat guests with incentives
- Optimise pricing based on stay duration and booking patterns
- Use predictive models to reduce revenue loss

---

## 📈 Key Results

- Random Forest achieved strong recall for cancellation detection
- KMeans clustering (K=5) provided the most actionable customer segments
- Cancellation rates varied from **14% to 99%** across clusters — confirming clear behavioural patterns

---



## 🚀 How to Run

```bash
# Clone the repository
git clone https://github.com/YourUsername/hotel-booking-cancellation-analysis.git

# Install dependencies
pip install kagglehub pandas scikit-learn seaborn matplotlib sqlite3

# Open the notebook
jupyter notebook Group_040__Capstone.ipynb
```

---

## 📬 Connect with Me

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Ronald%20Aroh-blue)](https://www.linkedin.com/in/ronald-aroh-a30a92180)
