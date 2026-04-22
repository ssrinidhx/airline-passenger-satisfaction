# Airline Passenger Satisfaction & Service Performance Analytics (Power BI)

## Project Overview

This project presents a **Business Intelligence (BI) dashboard built using Microsoft Power BI** to analyze airline passenger satisfaction, travel behavior, service quality, and operational performance. The analysis uses **data warehousing, OLAP techniques, and machine learning models** to generate meaningful insights from airline passenger data.

The dashboard helps identify factors affecting passenger satisfaction such as **flight delays, service quality, travel class, and customer loyalty**.

# Dataset

**Dataset:** [Airline Passenger Satisfaction Dataset](https://www.kaggle.com/datasets/teejmahal20/airline-passenger-satisfaction)
**Source:** Kaggle
**Records:** ~25,977 passengers
**Features:** Passenger demographics, travel details, service ratings, and delay information.

# Tools & Technologies Used

* **Microsoft Power BI**
* **Python (Power BI Python visuals)**
* **DAX (Data Analysis Expressions)**
* **Machine Learning Algorithms**
  * K-Means Clustering
  * Logistic Regression
  * Linear Regression

# Data Model (Star Schema)

The project implements a **data warehouse star schema** consisting of one fact table and multiple dimension tables.

**Fact Table**

* `Fact_Passenger_Flights`

  * Flight Distance
  * Arrival Delay
  * Departure Delay
  * Satisfaction

**Dimension Tables**

* `Dim_Passenger`

  * Gender
  * Age Group
  * Customer Type

* `Dim_Travel`

  * Travel Type
  * Class

* `Dim_Service`

  * Seat Comfort
  * Wifi Service
  * Cleanliness

* `Dim_Delay`

  * Delay Category

This structure enables **efficient multidimensional analysis using OLAP operations**.

# Dashboard Pages Overview

## 1. Executive Dashboard

The executive dashboard provides a **high-level overview of airline passenger statistics**.

Key metrics displayed include:

* Total Passengers
* Satisfied Passengers
* Satisfaction Rate
* Average Delay

It also highlights passenger distribution across travel classes and includes alert indicators for **delay control and service quality monitoring**. 

## 2. Passenger Demographics Analysis

This page analyzes **passenger characteristics and demographic patterns**.

Visual insights include:

* Passenger distribution by age group
* Gender vs satisfaction comparison
* Loyal vs disloyal customers
* Satisfaction levels across different age groups

These insights help understand **customer profiles and satisfaction trends**. 

## 3. Travel & Flight Analysis

This dashboard explores **travel patterns and operational metrics**.

Key analyses include:

* Passenger distribution by travel type
* Passenger distribution by travel class
* Average flight distance by class
* Delay category distribution
* Travel type vs satisfaction comparison

These insights help evaluate **flight operations and passenger travel behavior**. 

## 4. Service Quality Analysis

This page evaluates **airline service performance and customer experience**.

It analyzes passenger ratings for:

* Seat Comfort
* Inflight Wifi Service
* Cleanliness

The dashboard also shows how service ratings impact passenger satisfaction, helping identify **areas where airlines can improve service quality**. 

## 5. Customer Satisfaction Analysis

This page focuses on identifying **factors influencing passenger satisfaction**.

Key insights include:

* Overall passenger satisfaction distribution
* Impact of flight delays on satisfaction
* Satisfaction across travel classes
* Customer loyalty vs satisfaction
* Travel type vs passenger satisfaction

The analysis highlights that **service quality and delays significantly affect passenger satisfaction levels**. 

## 6. Predictive & Data Mining Analysis

This page applies **machine learning techniques** to analyze passenger behavior.

### K-Means Clustering

- Passengers are grouped into clusters based on travel behavior such as **flight distance and arrival delay**, helping identify different passenger segments.

### Logistic Regression (Classification)

- Logistic regression predicts whether a passenger is **satisfied or dissatisfied** using service features such as seat comfort, cleanliness, wifi service, and delay metrics.

### Linear Regression

- Linear regression analyzes the relationship between **flight distance and arrival delay**. The results indicate a **weak correlation**, suggesting delays are influenced more by operational factors.

Key insights from the predictive models are summarized directly in the dashboard. 

## 7. OLAP Analysis

This page demonstrates **Online Analytical Processing (OLAP) operations** for multidimensional data analysis.

Implemented OLAP operations include:

* **Roll-Up:** Aggregating passenger data at higher levels such as travel class.
* **Drill-Down:** Exploring detailed levels such as travel type within each class.
* **Slice:** Filtering data based on a single dimension (e.g., customer type).
* **Dice:** Applying multiple filters such as delay category and seat comfort.
* **Pivot:** Rotating the data cube using matrix visualizations to compare satisfaction across travel classes.

These operations enable **interactive exploration of passenger data across multiple dimensions**. 

# Key Insights

* Passenger satisfaction is strongly influenced by **service quality and travel class**.
* **Business class passengers show higher satisfaction levels** compared to economy passengers.
* **Flight delays significantly impact passenger satisfaction**.
* Clustering reveals distinct passenger travel behavior groups.
* Regression analysis shows that **flight distance has minimal impact on arrival delays**.

# Conclusion

This project demonstrates how **Business Intelligence tools such as Power BI can transform raw airline data into meaningful insights**. By integrating **data warehousing, OLAP analysis, and machine learning techniques**, the dashboard provides valuable insights into passenger behavior, service quality, and operational performance.

Such analytics can help airlines **improve customer experience, optimize services, and make data-driven decisions**.
