# Bank Marketing Analysis — Power BI

## 📊 Project Overview

This project analyzes a bank's marketing campaign data to understand customer demographics, campaign effectiveness, loan behavior, and factors associated with term-deposit subscriptions.

The project was developed using **Power BI, Power Query, and DAX** and includes interactive dashboards, advanced campaign analysis, Row-Level Security (RLS), and Power BI Service deployment.

---

## 🎯 Business Objectives

The main objectives of this project are to:

* Analyze customer demographic characteristics
* Understand campaign performance
* Identify effective contact methods
* Analyze housing and personal loan behavior
* Identify customer segments with higher subscription rates
* Analyze previous campaign outcomes
* Measure campaign conversion performance
* Build an interactive management dashboard
* Implement Row-Level Security
* Publish and configure the report in Power BI Service

---

## 🛠️ Tools & Technologies

* **Power BI Desktop**
* **Power Query**
* **DAX**
* **GitHub**

---

## 📁 Project Structure

```text
Bank-Marketing-Analysis-PowerBI/
│
├── README.md
├── Dataset/
│   └── bank-full.csv
│
├── PowerBI/
│   └── Bank_Marketing_Analysis.pbix
│
├── Screenshots/
│   ├── Campaign_Overview.png
│   ├── Customer_Loan_Analysis.png
│   └── Advanced_Campaign_Analysis.png
│
└── Documentation/
    ├── Business_Insights.md
    ├── DAX_Measures.md
    └── RLS_Documentation.md
```

---

## 🔄 Data Transformation

Power Query was used to:

* Import the bank marketing dataset
* Clean and standardize text fields
* Set appropriate data types
* Handle `unknown` categorical values
* Create customer age groups
* Create campaign success categories
* Create housing and personal loan status fields
* Identify previously contacted customers
* Handle `pdays = -1` as customers who were not previously contacted

---

## 📈 Dashboard Pages

### 1. Campaign Overview

The dashboard provides:

* Total Clients
* Subscribed Clients
* Subscription Rate
* Average Balance
* Average Campaign Contacts
* Subscription by Contact Method
* Monthly Subscription Rate
* Subscription by Age Group
* Subscription by Job
* Campaign Success Distribution

### 2. Customer & Loan Analysis

This page analyzes:

* Customer age distribution
* Job types
* Marital status
* Education
* Average balance by marital status
* Average balance by education
* Housing loan behavior
* Personal loan behavior
* Loan status versus subscription

### 3. Advanced Campaign Analysis

This page analyzes:

* Contact method effectiveness
* Campaign contact frequency
* Previous campaign outcomes
* Previous contact status
* Contact duration
* Subscription rate by month
* Job-level subscription performance
* Campaign performance matrix

---

## 📌 Key Insights

* The overall term-deposit subscription rate was approximately **11.7%**.
* Cellular was the strongest major contact method, with a subscription rate of approximately **14.9%**.
* Customers with a previous successful campaign outcome had a substantially higher subscription rate.
* Customers aged 60+ showed a comparatively high subscription rate.
* Tertiary-educated customers had a higher subscription rate than primary- or secondary-educated customers.
* Customers without housing or personal loans showed higher subscription rates.
* Successful customers had substantially longer average contact durations.
* Unsuccessful customers received more campaign contacts on average, suggesting that increasing contact frequency does not necessarily improve conversion.

> These findings represent associations observed in the dataset and should not automatically be interpreted as causal relationships.

---

## 🔐 Row-Level Security

RLS was implemented in Power BI Desktop using predefined roles based on the `job` field.

Example roles:

* `Management_Role`
* `Student_Role`
* `Retired_Role`

The roles were tested using Power BI's **View as** functionality.

For a production banking environment, RLS would normally be implemented using an actual branch, region, or user-access mapping table.

---


## 📊 Business Recommendations

Based on the analysis:

1. Prioritize effective contact channels such as cellular communication.
2. Give higher priority to customers with previous successful campaign outcomes.
3. Use customer segmentation instead of applying a single campaign strategy to all customers.
4. Review campaign contact frequency to avoid unnecessary repeated contacts.
5. Improve the quality of contact information to reduce unknown contact categories.
6. Analyze campaign volume together with conversion rate before selecting the best campaign period.

---

## 👨‍💻 Author

**Lokesh Kumar**

Data Analyst Portfolio Project

Skills demonstrated:

**Power BI | Power Query | DAX | Data Visualization | Business Analysis | RLS**
