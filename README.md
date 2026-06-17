# Airbnb-Market-Intelligence-Dashboard-PowerBI
Interactive Power BI dashboard analyzing Airbnb market performance, guest satisfaction, reviews, and host trust indicators across global cities using DAX, Power Query, and data storytelling.
# Airbnb Market Intelligence Dashboard

## Project Overview

The Airbnb Market Intelligence Dashboard is an end-to-end Business Intelligence project developed in Power BI to analyze Airbnb's global marketplace performance. The dashboard provides insights into listing growth, market share, pricing trends, guest satisfaction, review activity, and host trust indicators across major cities worldwide.

This project demonstrates the use of data modeling, DAX calculations, interactive visualizations, and storytelling techniques to transform raw Airbnb data into meaningful business insights.

---

## Business Objective

The primary goal of this project is to help stakeholders understand:

- Airbnb's growth trajectory over time
- Market dominance across major cities
- Property type distribution and pricing patterns
- Guest satisfaction and rating performance
- Review engagement and trust indicators
- Host verification and Superhost distribution

---

## Dashboard Pages

### Page 1: Market Overview

This dashboard provides a high-level overview of Airbnb's business performance and listing growth.
<img width="1198" height="895" alt="Screenshot 2026-06-17 162343" src="https://github.com/user-attachments/assets/45beff9d-8ac8-4abe-a056-4e496eb92e71" />



#### KPIs

- Total Listings: 279,712
- Total Reviews: 5.37 Million
- Total Hosts: 182,024
- Cities Covered: 10
- Property Types: 144

#### Key Visuals

- Listing Growth Trend
- Property Type Distribution
- New Listings Timeline
- Business Lifecycle Analysis

#### Key Insights

- Airbnb experienced rapid listing growth and reached its peak in 2015.
- Regulatory restrictions in key markets contributed to slower expansion during 2016 and 2017.
- The company achieved profitability in the second half of 2016.
- Growth momentum returned in 2018 before being disrupted by the COVID-19 pandemic.

---

### Page 2: Market Share & Guest Satisfaction

This dashboard focuses on city-level performance, ratings, and customer satisfaction.
<img width="1192" height="908" alt="Screenshot 2026-06-17 162400" src="https://github.com/user-attachments/assets/8b9a2fe3-ad11-45d6-a58e-e564ab7456e4" />


#### Key Visuals

- Market Share by City
- Property Type Analysis
- Average Rating by City
- Detailed Rating Breakdown

#### Key Insights

- Paris, New York, and Sydney collectively contribute nearly 50% of all listings and 59% of total reviews.
- Paris leads in both listing volume and customer engagement.
- Mexico City and Rio de Janeiro achieve the highest guest satisfaction scores.
- Hong Kong and Istanbul record comparatively lower ratings.
- Cleanliness and value for money consistently receive the lowest ratings across cities.

---

### Page 3: Reviews & Trust Overview

This dashboard analyzes customer engagement and trust-related indicators.
<img width="1192" height="905" alt="Screenshot 2026-06-17 162411" src="https://github.com/user-attachments/assets/30f95b9d-879f-4302-8a8d-6bd6b481a680" />


#### Key Visuals

- Average Ratings by City
- Host Verification by City
- Verified Host Distribution
- Superhost Distribution

#### Key Insights

- Paris records the highest review activity among all cities.
- Verified hosts represent the majority of listings across major markets.
- Host verification remains consistently strong, reinforcing guest confidence.
- Strong review activity and high host verification rates contribute to platform credibility.

---

## Key Performance Indicators

| KPI | Description |
|------|-------------|
| Total Listings | Total Airbnb listings available in the dataset |
| Total Reviews | Total customer reviews received |
| Total Hosts | Number of active hosts |
| Average Rating | Overall guest satisfaction score |
| Verified Hosts | Hosts with verified identities |
| Superhosts | Hosts recognized for exceptional hosting performance |

---

## Data Analysis Process

### 1. Data Preparation

- Cleaned and transformed raw Airbnb data using Power Query.
- Removed inconsistencies and handled missing values.
- Standardized data formats for analysis.

### 2. Data Modeling

- Established relationships between Listings, Reviews, Hosts, and Location tables.
- Created a star-schema model for efficient reporting.

### 3. DAX Calculations

Developed custom measures for:

- Total Listings
- Total Reviews
- Average Ratings
- Verified Hosts
- Superhost Listings
- Market Share Analysis

### 4. Dashboard Development

Built interactive dashboards featuring:

- KPI Cards
- Bar Charts
- Donut Charts
- Matrix Tables
- Dynamic Insights

---

## Sample DAX Measures

### Total Listings

```DAX
Total Listings =
COUNTROWS(Listings)
```

### Total Reviews

```DAX
Total Reviews =
COUNT(Reviews[review_id])
```

### Average Rating

```DAX
Average Rating =
AVERAGE(Listings[overall_rating])
```

### Verified Host Percentage

```DAX
Verified Host % =
DIVIDE(
    CALCULATE(
        COUNTROWS(Listings),
        Listings[host_identity_verified] = "t"
    ),
    COUNTROWS(Listings)
)
```

---

## Tools & Technologies

- Power BI
- Power Query
- DAX (Data Analysis Expressions)
- Microsoft Excel
- Data Modeling
- Data Visualization

---

## Skills Demonstrated

### Data Analytics

- Exploratory Data Analysis (EDA)
- Data Cleaning
- Data Transformation
- Data Validation

### Power BI

- Data Modeling
- DAX Measures
- Interactive Visualizations
- KPI Development
- Dashboard Design

### Business Intelligence

- Market Analysis
- Customer Satisfaction Analysis
- Trust & Engagement Analysis
- Data Storytelling
- Executive Reporting

---

## Business Impact

This dashboard helps stakeholders:

- Monitor market performance across cities.
- Understand customer satisfaction drivers.
- Identify high-performing markets.
- Evaluate host trust indicators.
- Track platform growth trends.
- Support data-driven decision-making.

---

## Dashboard Preview

### Market Overview Dashboard

<img width="1198" height="895" alt="Screenshot 2026-06-17 162343" src="https://github.com/user-attachments/assets/e332a0f5-8276-44ac-b6fc-905a244053ce" />


### Market Share & Guest Satisfaction Dashboard

<img width="1192" height="908" alt="Screenshot 2026-06-17 162400" src="https://github.com/user-attachments/assets/f8ae527b-cbef-4c37-94ad-9ca2a9b195e4" />


### Reviews & Trust Dashboard

<img width="1192" height="905" alt="Screenshot 2026-06-17 162411" src="https://github.com/user-attachments/assets/4fd1dc92-6611-4652-a67f-4b0915b16092" />


---

## Repository Structure

```
Airbnb-Market-Intelligence-Dashboard/
│
├── Dashboard/
│   └── Airbnb_Market_Intelligence.pbix
│
├── Dataset/
│   └── Airbnb_Dataset.xlsx
│
├── Images/
│   ├── Dashboard_Page_1.png
│   ├── Dashboard_Page_2.png
│   └── Dashboard_Page_3.png
│
└── README.md
```

---

## Future Enhancements

- Geographic Map Visualizations
- Sentiment Analysis on Guest Reviews
- Predictive Occupancy Analysis
- Dynamic City Comparison Tool
- Revenue Performance Dashboard

---

## Author

### Anurag Poddar

Data Analyst | Bardaha Criholic Private Limited

### Connect With Me

- LinkedIn: https://www.linkedin.com/in/anurag-kumar-poddar-51239596/
- GitHub: https://github.com/anuragkumarpoddar-ui


---

## Conclusion

This project demonstrates the application of Business Intelligence techniques to analyze Airbnb's marketplace performance from multiple perspectives, including growth, market share, guest satisfaction, and trust indicators. Through interactive dashboards and actionable insights, the solution enables stakeholders to better understand customer behavior, host performance, and overall platform dynamics.
