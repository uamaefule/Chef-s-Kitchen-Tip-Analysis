

# Chef's Kitchen Tip Analysis: Understanding Customer Spending & Tipping Behavior

![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)
![Pandas](https://img.shields.io/badge/Pandas-1.3+-orange.svg)
![NumPy](https://img.shields.io/badge/NumPy-1.21+-yellow.svg)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.5+-green.svg)
![Seaborn](https://img.shields.io/badge/Seaborn-0.11+-red.svg)
![License](https://img.shields.io/badge/License-MIT-yellow.svg)

## Project Overview

This project analyzes tipping patterns at Chef's Kitchen, a popular restaurant in San Diego. By examining customer data, bill amounts, and tipping behavior across various demographics, this analysis aims to identify key trends and insights that can help the restaurant understand customer spending habits and optimize service strategies. The findings provide actionable recommendations for improving customer experience and maximizing revenue.

## Business Problem

Chef's Kitchen faces challenges in:
- Understanding the relationship between bill amounts and tipping behavior
- Identifying peak service times and customer patterns
- Optimizing staffing and service strategies based on customer demographics
- Maximizing revenue through strategic service enhancements

This analysis addresses these challenges by uncovering patterns in customer spending and tipping behavior across different times, days, and customer segments.

## Dataset Description

The analysis is based on transaction data from Chef's Kitchen, containing the following features:

| Feature | Description | Type |
|---------|-------------|------|
| **order_id** | Unique identifier for each order | Numerical |
| **day** | Day of the week (Thur/Fri/Sat/Sun) | Categorical |
| **time** | Time of day (Lunch or Dinner) | Categorical |
| **size** | Number of people at the table | Numerical |
| **smoker** | Whether the table included smokers (Yes/No) | Categorical |
| **sex** | Gender of the bill payer (Male/Female) | Categorical |
| **total_bill** | Bill amount in dollars | Numerical |
| **tip** | Tip amount in dollars | Numerical |

**Dataset Characteristics**:
- **Total Records**: 240 transactions
- **Time Period**: Thursday through Sunday
- **Service Types**: Lunch and Dinner
- **Customer Segments**: Various party sizes and demographics

## Key Findings

### 1. **Billing and Tipping Patterns**
- **Bill Amount Distribution**:
  - Range: $3 to $50
  - Average: Approximately $20
  - 50% of customers pay less than $20 for their total bill
- **Tip Amount Distribution**:
  - Range: $1 to $10
  - Mean and Median: Approximately $3
  - 50% of customers tip less than $3
- **Bill-Tip Relationship**:
  - Clear linear relationship between total bill amount and tip amount
  - Higher bills consistently correlate with higher tips
  - Tip percentage averages around 15% of total bill

### 2. **Time and Day Analysis**
- **Order Volume Patterns**:
  - Significantly higher order volume on weekends compared to weekdays
  - Dinner service generates more orders than lunch service
- **Bill Amount by Day**:
  - Median bill amounts are higher on Saturdays and Sundays
  - Weekend bills show greater variability than weekday bills
- **Tip Amount by Day**:
  - Median tip amounts are consistent on Friday, Saturday, and Sunday
  - Lower median tip amounts on Thursday
- **Service Time Comparison**:
  - Customers spend approximately $3 more during dinner ($19 median) compared to lunch ($16 median)
  - Dinner tips average about $1 higher than lunch tips
  - Dinner service shows greater bill and tip variability

### 3. **Demographic Insights**
- **Gender Distribution**:
  - Male bill payers (160) outnumber female bill payers (80) by a 2:1 ratio
  - Gender disparity is most pronounced on weekends
  - Median tip values are similar across genders
  - Male tippers show more variability with more outliers on the higher end
- **Smoking Status Patterns**:
  - Non-smoking tables outnumber smoking tables by approximately 60
  - Non-smokers are significantly more common on Thursdays and Sundays
  - Fridays are the only day when smokers outnumber non-smokers
  - Smoking status does not appear to influence tip amounts
- **Party Size Influence**:
  - Larger parties (4+ people) tend to have higher total bills
  - Tip amounts increase with party size but at a decreasing rate
  - Parties of 2 show the highest tip percentage relative to bill amount

## Methods Used

### 1. **Data Preprocessing**
- **Data Loading**: Imported transaction data using Pandas
- **Data Cleaning**: Verified completeness and handled any missing values
- **Data Type Conversion**: Optimized data types for efficient processing
- **Feature Engineering**: Created derived metrics like tip percentage

### 2. **Exploratory Data Analysis (EDA)**
- **Univariate Analysis**: Examined distributions of bill amounts, tips, and demographics
- **Bivariate Analysis**: Explored relationships between bills and tips, time and spending
- **Segment Analysis**: Compared patterns across days, times, and demographic groups

### 3. **Statistical Analysis**
- **Descriptive Statistics**: Calculated means, medians, and distributions
- **Comparative Analysis**: Compared spending patterns across different segments
- **Correlation Analysis**: Identified relationships between numerical variables

### 4. **Data Visualization**
- **Distribution Visualizations**: Histograms and box plots for bill and tip distributions
- **Comparative Visualizations**: Bar charts for day/time comparisons
- **Relationship Visualizations**: Scatter plots for bill-tip relationships
- **Demographic Visualizations**: Grouped plots for gender and smoking status comparisons

## Technologies

- **Programming Language**: Python 3.8+
- **Data Manipulation**: Pandas 1.3+, NumPy 1.21+
- **Data Visualization**: Matplotlib 3.5+, Seaborn 0.11+
- **Development Environment**: Jupyter Notebook
- **Version Control**: Git

## Project Outcomes

### 1. **Business Impact**
- Identified optimal service times for maximizing revenue (weekend dinners)
- Discovered demographic segments with distinct spending patterns
- Established baseline metrics for tipping behavior analysis
- Uncovered opportunities for service optimization based on party size

### 2. **Operational Improvements**
- Developed staffing recommendations based on peak service times
- Created framework for analyzing customer spending patterns
- Established metrics for evaluating service effectiveness
- Identified opportunities for menu optimization based on spending patterns

### 3. **Customer Experience Enhancements**
- Discovered key factors influencing tipping behavior
- Identified opportunities for personalized service based on demographics
- Established benchmarks for customer satisfaction through tipping patterns
- Created framework for monitoring changes in customer behavior over time


## How to Use This Repository

1. **Clone the repository**:
   ```bash
   git clone https://github.com/yourusername/chefs-kitchen-tip-analysis.git
   ```

2. **Navigate to the project directory**:
   ```bash
   cd chefs-kitchen-tip-analysis
   ```

3. **Install dependencies**:
   ```bash
   pip install -r requirements.txt
   ```

4. **Run the Jupyter Notebook**:
   ```bash
   jupyter notebook
   ```

5. **Open and execute**:
   - `Chefs_Kitchen_Tip_Analysis.ipynb` for complete analysis
   - Explore individual sections as needed

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🤝 Connect

- [LinkedIn](https://www.linkedin.com/in/ucheamaefule/)
- [Portfolio](https://github.com/uamaefule/Data-Analytics-Portfolio)
- [Email](ucheamaefule@ymail.com)

---

*This project demonstrates comprehensive data analysis capabilities in the restaurant industry, showcasing skills in data manipulation, statistical analysis, and visualization. The insights provide actionable recommendations for improving restaurant operations, enhancing customer experience, and maximizing revenue through data-driven decision making.*
