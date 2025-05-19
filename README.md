# 🏨🍽 Lodging Proximity and Yelp Restaurant Reviews

A data-driven exploration into how the **proximity of hotels and vacation rentals** impacts restaurant reviews on Yelp, using APIs, SQL, and geospatial analysis.

![Project Banner](https://img.shields.io/badge/Tech%20Stack-SQL%20%7C%20Python%20%7C%20PowerBI%20%7C%20Geopy%20%7C%20API-blue)

## 📌 Overview

This project investigates how the physical distance between lodging options (Airbnb, Hotels.com, etc.) and restaurants affects:

- ⭐ Yelp review ratings
- 📝 Number of reviews
- 💲 Restaurant pricing and sentiment trends

It is part of the **GB 760 Data Tech Course Project** at the Wisconsin School of Business.

## 💡 Business Questions

1. **How does proximity to lodging influence Yelp restaurant review ratings?**
2. **Do restaurants closer to Airbnb rentals or hotels receive more total reviews?**
3. **Does restaurant pricing affect reviews when controlling for proximity to lodging?**

## 🧪 Hypotheses

- Restaurants closer to Airbnbs will have **more positive ratings** than those closer to hotels.
- Restaurants near Airbnbs will have **more total reviews**.
- Restaurants near hotels and with **higher prices** will receive **better reviews**.

## 🗃️ Data Sources

- **Yelp Fusion API** – Restaurant names, stars, review counts, price level
- **Google Hotels API** – Coordinates, star ratings, hotel class, review counts
- **Google Vacation Rentals API** – Coordinates, overall ratings
- **Kaggle Airbnb Dataset** – Coordinates, prices, review scores

## 🛠️ Tools and Technologies

- SQL (Snowflake)
- Python (Pandas, Geopy, Matplotlib, WordCloud)
- Power BI (Visual dashboards)
- RESTful APIs
- ANOVA & OLS Regression for statistical testing

## 📍 Methodology

- **Data Collection:** Scraped/queried hotel, Airbnb, and Yelp data via APIs and Kaggle
- **Distance Calculation:** Used geopy to calculate distances between restaurants and nearby lodgings
- **Data Cleaning & Merging:** By ZIP codes and coordinates
- **Visualization:** Power BI for summary dashboards, charts, and insights
- **Modeling:** ANOVA and regression analysis to test hypotheses

## 📊 Key Visuals

- Average star rating across distance ranges
- Review count across proximity buckets
- Price vs. rating regression charts
- Sentiment word clouds from hotel reviews

## ✅ Results

- Restaurants located within **0.5 to 1.5 miles** of lodging had **higher average ratings**
- Total number of reviews dropped sharply when the restaurant was over **30 minutes away**
- **More expensive restaurants** generally received **higher ratings**, regardless of distance
- Hypotheses were partially supported, indicating nuanced trends

## ⚠️ Challenges

- Data inconsistencies between APIs (e.g., hotels vs. vacation rentals)
- Biased reviews and sponsored listings
- Limited granularity of some review metrics
- API rate limits and irrelevant matches (e.g., Brandon Burgers returning Kush Wynwood)

## 🔭 Future Work

- Sentiment analysis of both restaurant and hotel reviews
- Explore **temporal trends** in ratings
- Investigate the effect of **restaurant category** on review patterns
- Examine influence of hotel quality on restaurant pricing strategies

---

